# Eth 2.0服务协议

《Eth 2.0质押宝服务协议》（以下简称“本协议”）是TokenPocket钱包（以下简称“本平台”）用户协议的补充部分。本平台的用户协议及其他条款继续适用于本平台所有用户。在您通过本平台继续下一步操作前，请您务必仔细阅读并透彻理解本协议。如您通过本平台继续下一步操作，或以任何方式使用平台服务，视为您已经谨慎阅读并理解且同意本协议。

本协议在任何时候都可以被本平台修改、更改或更新，而无需事先通知您。您应该经常检查，以确认您对本协议的复制和理解是及时和准确的。在任何修改、更改或更新的生效日期之后，如您继续选择使用本网站的任何服务，即视为您对新修改、更改或更新后的本协议的接受。

本网站所有内容，为便利用户，提供多个语言版本，若有冲突或遗漏等情况，以中文内容为准。

特别提示：虚拟货币存在较高风险，质押宝仅进行节点质押的简化服务，不鼓励也不提倡您以任何形式购买ETH币进行质押。

#### 一、定义

1. 以太坊（Eth）是一个工作量证明（POW）的区块链网络。Eth 2.0，即以太坊2.0，是以太坊主网的权益证明（PoS）版本。它引入了分片技术，整个过程分为Phase0（信标链）、Phase 1（分片）、Phase 2（智能合约）、Phase 3（链侠状态存储）、Phase 4（分片智能合约）等阶段。
2. Eth 2.0 Staking是Eth权益证明的实现机制。在信标链上，用户可以投注32个ETH作为验证者。在阶段0中，验证者只需管理信标链即可；而从阶段1开始，验证者在管理信标链的同时，还将管理1024条分片链。信标链以及每一条分片链将使用Casper FFG算法完成出块。FFG是一种权益证明算法（Proof of Stake），用于对链上不良行为实施Slash罚没（即削减权益）。验证者抵押的32ETH直到进入Phase 2阶段才可以解锁。
3. Eth 2.0质押宝是基于Eth 2.0系统Staking基础上进行简化的服务。没有强制性质押32ETH的要求，同时也对锁仓的ETH进行了流动性释放。
4. 服务费是指本平台代用户运行Eth 2.0节点，享有用户节点质押奖励的15%及区块链可提取价值的20%作为平台服务费。 1.5 手续费是指用户使用本平台提供的ETH退出功能，须向平台支付一定的费用，当前收取1%。

#### 二、Eth 2.0质押宝规则

您在本平台进行的质押、退出或以任何方式使用平台服务的行为，都视为您已经谨慎阅读并理解且同意产品规则。质押宝服务分为自托管质押和联合质押，规则如下：

1. TokenPocket将收取用户一定的节点奖励作为节点运营费，用户每日收到的质押奖励为扣除节点运营费之后的数量。
2. 实际收益以Eth 2.0主网实际质押情况而定。
3. 由TokenPocket运营不当导致的Slash（节点惩罚）由TokenPocket承担，由于ETH官方提供的Eth 2.0节点运行客户端或Eth 2.0合约Bug导致的Slash不在承担范围之内。
4. 质押奖励收益每隔一个epoch（理论为6.4分钟）进行一次结算。

**自托管质押补充规则：**

* 自托管质押存在双密钥原则，用户持有“提款密钥”（可以管理资金），TokenPocket仅持有“验证者密钥”。提款密钥由用户自身创建及保管，一旦丢失或遗忘，则会导致节点资金无法取回。该责任将由用户自行承担。
* 自托管质押需用户提供32 ETH进行生成节点，TokenPocket将收取0.05 ETH费用作为节点维护费用，节点持续运行过程中不再额外收取。
* 自托管质押发起节点质押后，节点生效时间与当前链上质押排队状态相关。
* 自托管质押退出节点生效时间与链上退出排队状态相关，自托管质押不可参与快速赎回活动。

**联合质押补充规则：**

* 最低投入0.1 ETH。
* 每日22:00 UTC+8前抵押的用户将被记为今日抵押，预计T+1开始计算收益，即明日的22:00 UTC+8开始产生收益。每日22:00 UTC+8以后抵押的用户将记录为第二日抵押，即后日的22:00 UTC+8开始产生收益。实际收益时间受节点激活限制，如存在大量节点排队激活，则收益时间可能往后推移（"T+1"用于计算用户奖励，具体奖励时间与节点激活时间有关，抵押的越早，得到的回报就越早）。
* 每个用户每天最少退出额度为0.1 ETH，最多可退出额度为10 ETH。申请退出后，每24小时集中处理一次退款，全部用户可退出的总ETH数量由流动性基金决定。使用退出功能需要支付一定的手续费。最终用户收到的ETH=允许退出的ETH数量-退出手续费-转账GAS费用。
* 平台提供流动性基金，即平台整合行业资源为质押用户提供一定额度的快速赎回功能。快速赎回已获得收益归属用户，快速赎回部分不再享有质押奖励。只支持本金赎回，不支持质押奖励提前赎回。快速赎回手续费为赎回资金的1%。 流动性基金补充说明：流动性基金本金不定期退出，采取先到先得的模式。

#### 三、质押争议处理

1. 用户丢失私钥、助记词、密码或账号私钥泄露等情况，导致失去账号控制权而无法退出或领取奖励，由用户自身承担损失。
2. 用户不了解Eth 2.0机制或未仔细阅读协议，而导致对产品规则的误解，提出规则以外利益申诉的情况，平台有权驳回申请。
3. 产品实际收益与Eth 2.0主网质押情况以及开发进度相关。若因Eth 2.0主网出现重大漏洞或开发停滞等情况，可能导致用户资产受损，由用户自行承担损失。

#### 四、责任声明和责任免除

1. 本平台仅向您提供Eth 2.0节点代运营服务。您充分了解Eth 2.0及Eth 2.0 Staking机制可能存在的风险和瑕疵。本平台将通过尽可能稳定的节点运营服务保障代运营的节点质押收益。鉴于Eth 2.0发展需要的周期较长，可能存在多种风险的特点，您应谨慎判断。
2. 基于数字资产的特殊性，数字资产价格波动较大，零售和商业市场使用相对较少，数字资产交易存在极高风险。全天不间断交易，没有涨跌限制，价格容易受环境和全球政策的影响而大幅波动。由此数字资产价格变动可能带来投资收益受损的情况，由用户自行承担。我们不建议也不提倡您购买数字资产，更不建议您购买ETH进行质押。
3. 禁止使用本平台从事洗钱、走私、商业贿赂等一切非法交易活动或违法行为。若发现任何涉嫌非法交易或违法行为，本站将采取各种手段，包括但不限于冻结账户，通知相关权力机关等。我们不承担由此产生的所有责任，并保留向相关人士追究责任的权利。
4. 您的行为使本平台遭受损失（包括自身的直接经济损失、商誉损失及对外支付的赔偿金、和解款、律师费、诉讼费等间接经济损失），您应赔偿本网站的上述全部损失。如您的行为使本平台遭受第三人主张权利，本网站可在对第三人承担金钱给付等义务后就全部损失向您追偿。
5. 数字资产交易具有极高风险，并不适合绝大部分人士。您了解和理解此投资有可能导致部分或全部损失，所以您应该以能承受的损失程度来决定投资金额。您了解和理解数字资产会产生衍生风险，如有任何疑问，建议先寻求理财顾问的协助。此外，除了上述提及的风险外，还会存在未能预测的风险。如果您不属于本平台提供服务范围内的用户，请不要参与本平台提供的服务。若因您个人参与本平台服务而导致的相关后果，由您个人承担所有责任。您应慎重考虑并以清晰的判断能力评估自己的财政状况和上述各项风险，再作出任何买卖数字资产的决定，并承担由此产生的全部损失。平台对此不承担任何责任。
