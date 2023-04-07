# 警惕助记词分享诈骗

近期社区中看到有多人反馈波场钱包在转账是遇到了错误，经过对比发现他们有一定的共同之出。经过深入了解，他们是从网络上获取到公开的私钥或助记词，用户导入波场钱包后可以看到或多或少持有的资产，再转入TRX后进行转账会遇到错误，无论是哪种代币的转账都会报错，下面就将这个我们称之为钓鱼钱包的骗局的本质和大家进行说明。



案例剖析：

1、使用公開的私鑰或助記詞導入到錢包中，在Gas（礦工費）足夠的情況下選擇例如USDT的轉賬，填入收款地址，設置數量，在輸入密碼轉賬後會提示一堆代碼的錯誤提示。

{% embed url="https://1241502402-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FMr66Ca6n3UR4Xw7gcij2%2Fuploads%2F5Vlzi6jYIdJHrDCgTtoH%2F01.png?alt=media&token=143ad3f2-241f-4b5d-a03f-8db9a2487716" %}

2、点击上图的收款地址，记录好这个地址后面会用到，打开波场内存块链浏览器：[<mark style="color:blue;">**https://tronscan.io/#**</mark>](https://tronscan.io)填入收款地址进行查询，为了直观的展示内容，这里选择了PC端的浏览器内容演示。

{% embed url="https://1241502402-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FMr66Ca6n3UR4Xw7gcij2%2Fuploads%2FsvIe7CYi8iM5XlCWYwCg%2F2.png?alt=media&token=c8559b40-b037-4cd7-aaa1-e32147b5ba40" %}

在【账户权限】中可以看到owner和active两个活动权限都为同一个地址，但是这个地址和钱包的收款地址不同，这个就很明显的可以解释为什么所有导入的资产都无法进行转账。

这里简单的说明一下，波场公链整合了以太坊和EOS的一些特性，所以它和EOS的权限设置基本相同，分为owner、active、权重、阈值等内容，具体的功能说明和操作可以参考官方的多签说明文档：[<mark style="color:blue;">**https://cn.developers.tron.network/docs/multi-signature**</mark>](https://cn.developers.tron.network/docs/multi-signature)

在这里再次提示大家，天上不会掉馅饼，这种骗取Gas（矿工费）的骗局是一种比较早期的骗局，用户最多损失一些手续费，但是如果遇到【恶意授权】或【合约调用盗币】等方式，那么损失就会比较大了。
