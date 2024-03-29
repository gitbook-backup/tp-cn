# 什么是多签

与多签对应的是单签，我们要往区块链上发送一笔转账操作，需要用钱包生成一个签名，我们自己签好名把交易发送出去，这就是典型的单签方式，也是我们平时常用的钱包执行方式。

多签，顾名思义，就是需要多个人去签名执行某个操作的方式。使用多签进行转账，往往需要 >= 1 个人去签名发送交易，转账操作才可以完成。使用多签钱包时，我们可以指定 m/n 的签名模式，就是 n 个人里面有 m 个人签名即可完成操作。比如 2/3 签名模式，就是 3 个人里面有两个人签名就可以。

ETH/ERC20 (包括 BSC/BEP20 等EVM链）的多签采用轻量智能合约（smart contract）方式。

**适用场景：**&#x20;

1\. 用于需要多人管理资产，避免资产被个人挪用；&#x20;

2\. 通过多签对资产进行多重加密，增强资产安全性；

3.其他安全应用场景。
