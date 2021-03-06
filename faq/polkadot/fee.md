# 什么是转账的小费？

小费为一种可选的交易费用，在 Polkadot 和 Kusama 网络中，用户可以添加该费用以提高交易的优先级。使交易快速成功。

**说明：**

1.小费为可选项，用户根据自身情况选择是否支付小费。

2.在相同情况下，矿工优先打包支付小费的交易

## **Polkadot & Kusama 转账矿工费计算公式**

Polkadot & Kusama 网络中的转账矿工费由以下三个参数计算得出：

**a.按字节收费（也称为“长度费”）：**

长度费是每字节费用与交易体积大小（以字节为单位）的乘积。

**b.权重费（weight）**

权重费：权重是一个固定数字，旨在管理验证区块所花费的时间。每笔交易都包含基本权重和派遣权重。基本权重说明了交易包含的开销（例如签名验证），派遣权重则说明了执行交易的时间。总权重乘以每权重的费用，就可以计算出交易的权重费用。

**c.小费（可选）：**

是一种可选的交易费用，用户可以添加小费提高交易的优先级。

这三项费用构成了交易费用。在执行交易之前，从用户的帐户中扣除。一部分费用将归区块生产者所有，其余部分将归财政部所有。在波卡的创世中，这一比例分别设置为 20% 和 80%。

