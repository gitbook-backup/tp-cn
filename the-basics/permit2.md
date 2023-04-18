# 什么是Permit2

Uniswap Labs发布了两个新的智能合约 Permit2 和 Universal Router，Permit2 有着更好的链上使用体验，让我们一起了解Permit2 带来的变化，以及它的优缺点。

### <mark style="color:orange;">**关于Permit2**</mark> <a href="#about" id="about"></a>

Uniswap 发布了新的Token授权标准 Permit2，区别于传统的 ERC20 和 EIP-2612, Permit2 协议具有节省 gas、可批量操作授权/转账且比传统 ERC20 approve 更灵活，并且支持一站式的授权管理。

Permit2 协议让其他应用可以从整合这些合约中大大受益。Uniswap 本身致力于建设公共基础设施，因此设计了这些合约，提供整个开发者生态系统使用，包括广泛的文档、SDK。

为了说明 Permit2 的革命性，让我们回顾一下之前的解决方案，以合约需要移动 Alice 的Token为例。

### <mark style="color:orange;">**传统授权模式**</mark> <a href="#tradition" id="tradition"></a>

传统的执行方式是如下图所示的执行过程。

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FZCSGxZxDUFXGuknjRHbB%2Fuploads%2F9APh5PNStCAlcssu4SUg%2Fimage.png?alt=media&#x26;token=ee47c2b4-91d1-42a0-aa6b-a2b3cfadcf40" alt=""><figcaption></figcaption></figure>

1.Alice调用ERC20上的approve()来授予合约的支配限额。

2.Alice在合约上调用一个交互函数，该函数又在ERC20 Token合约上调用transferFrom()，移动她的Token。

显然，这个模型是可行的(它是普遍存在的)，并且最终可以非常灵活，因为协议通常会不间断地长期访问用户的Token。

授权合约默认获取最大数量支配Token的权限，并且没有时间的限制，不同的DApp首次执行都需要授权一次，具有很大风险。

<mark style="color:blue;">**但它面临着两个现实问题:**</mark>

* 糟糕的用户体验：用户必须授权他们打算使用的每个Token上的每个新协议，而这几乎总是一个单独的事务（例如在uniswap中执行了某个Token授权，但是如果使用 transit 依然需要重新进行approve）。
* 糟糕的安全性：合约通常都会要求无限的授权额度，并且每使用一个swap或者其他合约都用都需要执行一次approve。这意味着，如果该协议被利用，每个用户授权该协议消费的Token都有可能把用户的授权Token全部转移。（例如我们经常会遇到的Token使用授权，例如操作DeFi需要授权，进行兑换需要授权，不同的DApp首次使用都需要授权）

### <mark style="color:orange;">**permit（EIP-2612）模式**</mark> <a href="#eip-2612" id="eip-2612"></a>

EIP-2612 对Token的授权进行了迭代。用户可以通过在他们的交互中附加一个授权签名（Permit）信息来与应用合约交互，而不需要事先授权。

让我们看看 ERC20 的 EIP-2612 扩展所启用的方法，它通常是这样的：

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FZCSGxZxDUFXGuknjRHbB%2Fuploads%2FqsueYCqpcNIuIIboOFlp%2Fimage.png?alt=media&#x26;token=49f43286-484d-4c87-8a88-8bb032863eaa" alt=""><figcaption></figcaption></figure>

1. Alice签署一个链外的 "permit(签名授权)" 信息，表示她希望授予一个合约一个（EIP-2612）Token的使用权。
2. Alice提交签署的消息，作为她与所述合约交互的一部分。
3. 合约调用Token上的 "permit()" 方法，它会使用签名授权信息和签名，同时授予合约一个授权。
4. 合约现在有了授权，所以它可以在Token上调用transferFrom()，转账由 Alice 持有的Token。

由于Permit (EIP-2612) 需要把相关方法写入ERC20Token合约内，所以已经部署的ERC20合约无法进行支持。

<mark style="color:blue;">**这解决了典型 ERC20 授权方法的两个问题：**</mark>

* 用户不需要额外提交一个链上的approve()交互。
* 由于省掉了一笔链上操作所以可以通常可以选择一个更合理的授权额度，而不是无限大，更重要的是在签名授权消息时可以设置一个到期时间。      \


虽然 EIP-2612 使Token授权更加安全，但在 EIP-2612 之前推出的Token并不支持签名授权功能，而且并非所有较新的Token都采用该功能。因此该协议很难大范围的使用。

### <mark style="color:orange;">**Permit2 授权模式**</mark> <a href="#approve" id="approve"></a>

Permit2 结合了这两种模式，将 EIP-2612 的用户体验和安全优势扩展到也涵盖了普通的 ERC20 Token。

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FZCSGxZxDUFXGuknjRHbB%2Fuploads%2FVmfM9ezm3LlxGsp120JK%2Fimage.png?alt=media&#x26;token=217e3616-fd01-4baa-8243-5b43e6417ece" alt=""><figcaption></figcaption></figure>

1. Alice 在一个 ERC20 上调用approve()，典型的方式为的 Permit2 合约授予一个无限的授权。
2. Alice 签署一个链下permit2 消息，该消息表明协议合约被允许代表她转账代Token。
3. Alice 在协议合约上调用一个交互函数，将签署的 permit2 消息作为参数传入。
4. 协议合约在 Permit2 合约上调用 permitTransferFrom()，而 Permit2 合约又使用其授权（在 1 中授予）在 ERC20 合约上调用 "transferFrom()"，转账 Alice 持有的Token。

将授权给与Permit2后，使用了Permit2协议的DApp 只需要进行一次712的本地签名就可以，不需要额外的链上approve，降低了Gas费用，增加了易用性和安全性。授权具有时限性，例如授权一个月，那么一个月时间过期后下次使用同样只需要一次712签名即可。

协议不会直接调用 ERC20 Token上的transferFrom()来执行转账，而是调用规范的 Permit2 合约上的permitTransferFrom()。Permit2 位于协议和 ERC20 Token之间，跟踪和验证 permit2 消息，然后最终使用其授权直接在 ERC20 上执行transferFrom()调用。这种间接性使得 Permit2 可以将类似于 EIP-2612 的好处扩展到每一个现有的 ERC20 Token上。

### <mark style="color:orange;">**传统模式和Permit2 模式的执行对比**</mark> <a href="#contrast" id="contrast"></a>

传统授权模式，默认最大数量授权给DApp执行合约，授权后即可进行兑换操作。

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FZCSGxZxDUFXGuknjRHbB%2Fuploads%2F8Zuk1P9zwMuA8PPENbkl%2Fimage.png?alt=media&#x26;token=df3f6979-bb43-4603-be01-dbc71f4c04a3" alt=""><figcaption></figcaption></figure>

首次授权会授权给Permit2 合约，授权后需要用户进行一次签名（链下），前两步执行成功后才可以进行兑换。

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FZCSGxZxDUFXGuknjRHbB%2Fuploads%2FoZjtEufIS31SL54bj61M%2Fimage.png?alt=media&#x26;token=153b86ce-0d71-43cf-89ab-93409045fe56" alt=""><figcaption></figcaption></figure>

### <mark style="color:orange;">**Permit2 可能存在的风险**</mark> <a href="#risk" id="risk"></a>

Permit2 衍生于 EIP 2612，属于一种拓展的 EIP 20 协议，所以归根到底，Permit2 只是 ERC20 的一种补充，而不是取代。毕竟 Permit2 并没有可以直接继承现有所有的 ERC20 数据，所谓的一站式管理，本质上还是需要调用 ERC20 合约的 approve 操作来完成一些初始的操作。

**Permit2 完整的流程应该是**

1. 用户将 ERC20 Token的最大授权给到 Permit2合约。
2. 用户通过 permit函数对 Permit2合约中的具体授权进行管理。
3.  第三方协议和用户可以根据 Permit2 中已有的授权信息通过 Permit2 合约作为中间人实现Token的转移。



**Permit2 协议具有的优点**

1. 统一的Token管理。
2. 可控制的授权时间。
3. 不用每次都多发一笔交互来进行授权。

### <mark style="color:orange;">**Permit2 协议可能存在的风险**</mark> <a href="#risk2" id="risk2"></a>

1. 号称解决了 infinity approval 的问题，但实际只是把授权对象从需要交互的 DApp 转变成了 Permit2 合约，集中管理授权对  Permit2 合约的安全性有着更高的要求。
2. 虽然说Token授权有过期时间，但是这个时间依旧可以无限大，还是需要各个Dapp合理的设置过期时间。
3. 由于调用 permit 函数的过程可以不发送交互而是只提供签名给第三方代发，如果是做钓鱼的话可以做得更加隐蔽，用户检查签名消息的成本提升，某些第三方钱包可能不会对签名信息进行解码展示，导致用户被攻击的风险更高。

优点和风险同时存在，这就需要我们具有一定的辨别能力，具体到钱包方也需要对后续可能大范围支持Permit2 有一个提前的防范，（现在TokenPocket 还没支持 Permit2 的解析，后面很快会支持。）例如TokenPocket 现在的授权风险提示等弹窗，就可以很好的把风险内容进行展示，从而避免因为钓鱼或第三方恶意授权等风险。

不要随意打开不明来历的网站并执行，一定要使用正规的DApp并尽可能的控制好授权给合约的Token数量，时常用授权检测工具进行检查。
