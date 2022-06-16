# 什么是矿工费？

矿工费（Gas Fee）也称为网络费，顾名思义就是支付给矿工的手续费，当您在区块链上进行转账时，矿工（或节点）需要把您的转账交易打包并放上区块链，才能使交易完成，在这过程中会消耗区块链的运算资源，因此产生矿工费用。

在EVM兼容链中，手续费是由Gas Price（单价）和消耗的 Gas Limit（数量）来确定的，其中计算公式如下：\
矿工费 = Gas Limit \* Gas Price

Gas Limit数量主要受根据智能合约的内容操作复杂程度影响。操作越多，Gas limit越高。Gas Price是由发起方设置的，发起方设置的Gas Price的价格越高，其发起的交易就能越快被打包。

注： \
以太坊(Ethereum)的网络费为ETH; \
币安智能链(BNBChain)的网络费为BNB;\
波场(TRON)的网络费为TRX;\
马蹄(Polygon/Matic)的网络费为MATIC;\
Solana的网络费为SOL;\
OKExChain的网络费为OKT;

网络用不完是可以退回的。

转账网络收取的矿工费（网络费）会根据网络的情况而有所不同，<mark style="color:red;">**一旦确定交易，不管交易是否成功，矿工费都无法退回。**</mark>

<mark style="color:red;">**矿工费是由您所选取的转账网络进行收取，TokenPocket钱包不收取任何费用！**</mark>

观看视频，了解更多关于转账以及矿工费的知识！

{% embed url="https://www.bilibili.com/video/BV1t54y1f7ft" %}
