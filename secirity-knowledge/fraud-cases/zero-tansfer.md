# 警惕“零金额”转账骗局

恶意授权是通过Approve操作，给某个代币授权在一定数量范围内可以调用的权限，恶意授权通常会盗取授权代币的所有余额。

**那么如果一个普通的地址没有执行过Approve操作是否也可以被调用呢？**

近期越来越多的用户反馈，在自己的USDT转账列表中会看到有**“0USDT”**被转出的记录，如下

<div>

<figure><img src="data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%27454%27%20height=%27404%27/%3e" alt=""><figcaption></figcaption></figure>

 

<figure><img src="https://mirror.xyz/_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2FDgPm8cN3RlAW0rq_DuQ7a.png&#x26;w=1080&#x26;q=90" alt=""><figcaption></figcaption></figure>

</div>

大部分看到自己的地址被调用转出资产，第一反应会认为自己可能会有被恶意授权的风险，于是打开权限检测工具或浏览器查看自己的授权记录。

然而，浏览器上只出现了“已取消”的提示，如下图，

<div>

<figure><img src="data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%271375%27%20height=%27510%27/%3e" alt=""><figcaption></figcaption></figure>

 

<figure><img src="https://mirror.xyz/_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2F2fW22F2FGcFKcKfVL5-Pe.png&#x26;w=3840&#x26;q=90" alt=""><figcaption></figcaption></figure>

</div>

在授权列表中发现了一条授权记录，但是在右侧发现【已取消】的提示，点击箭头查看授权和取消的记录

<div>

<figure><img src="data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%271375%27%20height=%27497%27/%3e" alt=""><figcaption></figcaption></figure>

 

<figure><img src="https://mirror.xyz/_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2F4gMC2r7fSdt6cxyF3wZFA.png&#x26;w=3840&#x26;q=90" alt=""><figcaption></figcaption></figure>

</div>

查询后发现，授权变更记录中的内容也是空白的，**这个时候用户彻底陷入迷茫中。**

### 别担心! 让我们一起来还原这一操作。

1、打开波场浏览器，找到USDT合约地址，点击【合约】--【编写合约】--【8.transferFrom】

<div>

<figure><img src="data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%27640%27%20height=%27198%27/%3e" alt=""><figcaption></figcaption></figure>

 

<figure><img src="https://mirror.xyz/_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2FIBAn_djt0UqSr6WMIT4CC.png&#x26;w=1920&#x26;q=90" alt=""><figcaption></figcaption></figure>

</div>

2、在这里分别填入发送地址、接收地址和数量，然后点击【Send】利用插件钱包完成签名后就可以看到底部绿色的【true】说明执行成功，如果这里的数量设置其他，那么会提示已发送的内容，但是因为对方并没有可以调用的数量，所以无法执行成功。这里消耗的TRX由对方来买单，这个可以放心。

<div>

<figure><img src="data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%271338%27%20height=%27395%27/%3e" alt=""><figcaption></figcaption></figure>

 

<figure><img src="https://mirror.xyz/_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2FvVmpTa23p3ACIVdiB8bIC.png&#x26;w=3840&#x26;q=90" alt=""><figcaption></figcaption></figure>

</div>

3、执行成功后，我们继续查看这个地址的授权信息，果然是又增加了一条空白的记录。

<div>

<figure><img src="data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%271369%27%20height=%27502%27/%3e" alt=""><figcaption></figcaption></figure>

 

<figure><img src="https://mirror.xyz/_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2FTn_XLX0QpLcOS-itnLQy_.png&#x26;w=3840&#x26;q=90" alt=""><figcaption></figcaption></figure>

</div>

到这里，相信大家应该对这种问题发生的原因有了充分了解，说明任何地址都可以被拿来调用，只是这种方法是徒劳的。

**它并不会让我们的资产有任何的风险**，它只会让不明白原因的小白受惊一场，他们的最终目的还是想让你使用错误的地址来触发误转账来谋取利益。**同时你也可以了解关于 ”**[**精准伪装地址**](https://mirror.xyz/0x21Ca5ED8bDc391f852F3A056aa74F6aFf5669636/UZzHZqZOsefyjrxxWsHBf0mhDk0Ru\_Eik\_VsCreNhvY)**“的盗币方式**

这种调用在_**其他EVM链**_上同样适用，之前的高仿尾号地址诈骗方式是主动转入的方式，现在的这种调用是一个转出的方式，对于触发误操作的迷惑性会更强。骗子的骗术更新很快，大家要多注意。

### 针对大家比较疑惑的几个问题进行下解读：

1、为什么我的资产会被调用？

这种操作是直接通过USDT代币的 TransferFrom 功能执行的，任何地址都可以被调用并在钱包中生成一个记录，在授权记录中生成一个空白的记录。

2、出现这种情况，我的资产还安全吗？

_**这种操作目的就是为了模拟从用户地址转出的记录，结合伪装地址的方式来诱导用户误操作进行转账，它并不能对你的资产产生任何风险，但是请一定要注意这种可能误操作的执行。**_

