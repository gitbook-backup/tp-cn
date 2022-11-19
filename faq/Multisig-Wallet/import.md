# 多签钱包导入教程

### <mark style="color:orange;">什么是多签钱包：</mark> <a href="#shen-me-shi-duo-qian-qian-bao" id="shen-me-shi-duo-qian-qian-bao"></a>

与多签钱包对应的是单签钱包，我们要往区块链上发送一笔转账操作，需要用钱包生成一个签名，我们自己签好名把交易发送出去，这就是典型的单签钱包，也是我们平时常用的钱包。多签钱包，顾名思义，就是需要多个人去签名执行某个操作的钱包。使用多签钱包进行转账，往往需要 >= 1 个人去签名发送交易，转账操作才可以完成。使用多签钱包时，我们可以指定 m/n 的签名模式，就是 n 个人里面有 m 个人签名即可完成操作。比如 2/3 签名模式，就是 3 个人里面有两个人签名就可以。ETH/ERC20 (包括 BSC/BEP20 等EVM链）的多签采用轻量智能合约（smart contract）方式。

**适用场景：**

1\. 用于需要多人管理资产，避免资产被个人挪用；

2\. 通过多签对资产进行多重加密，增强资产安全性；

3.其他安全应用场景。

### <mark style="color:orange;">多签钱包导入：</mark> <a href="#duo-qian-qian-bao-chuang-jian" id="duo-qian-qian-bao-chuang-jian"></a>

多签钱包的导入非常简单，只需要导入生成的多签钱包地址，就可以自动识别出钱包的管理钱包、最少确认签名数等信息。

1、打开TokenPocket点击右上角第一个图标，添加多签钱包。

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

2、导入多签钱包界面中，顶部需要填入创建的多签钱包地址，如果填入非多签钱包地址则会提示无法导入的提示，填入了多签地址后，下方会自动识别你所创建的公链网络、最少确认签名数和管理钱包等信息，操作就像使用观察钱包一样简单，当然他甚至也可以作为一个观察钱包来使用。

一切设置完毕后，点击【确认】就可以导入到多签钱包中。

<figure><img src="../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>
