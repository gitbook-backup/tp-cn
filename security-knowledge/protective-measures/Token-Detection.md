# 代币合约安全检测工具使用指引

在DEX中完成代币交易是我们日常中经常使用的一个功能，因为代币交易平台去中心化的开放性，可以允许任何人或者团队上线不同类型的代币，在这个过程中有些不法分子就会在代币合约中做手脚，例如无法交易（貔貅）代币、有增发功能的代币等。这个时候就需要用到代币合约安全检测工具，虽然工具的检测无法保证百分之百的准确，但是它可以在很大程度上排除一些风险，选择更安全的代币进行交易。

1、打开TokenPocket，点击任意需要检测的代币，打开的界面中点击右上角【项目详情】。

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FMr66Ca6n3UR4Xw7gcij2%2Fuploads%2FtLVpvUAohgSOrAMJm449%2F1%20%E6%8B%B7%E8%B4%9D.png?alt=media&token=2f387dba-129e-476d-9967-dbb6a241814b" %}

2、在详情界面中可以看到代币的合约地址和发行量等数据，在下半部分可以看到代币的风险提示内容，一般分为【危险警告】和【安全提示】其中危险警告的等级最高，点击【查看更多安全信息】可以跳转到合约检测详情，在这里可以查看代币合约地址的安全检测详情内容。

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FMr66Ca6n3UR4Xw7gcij2%2Fuploads%2F8p5o5LAS8MsGGcpLiJJU%2F2%20%E6%8B%B7%E8%B4%9D.png?alt=media&token=ae33b7d5-5ef7-4528-b701-6ef7c0d5d850" %}

3、在安全检测详情界面的开头部分是内嵌的一个小工具，点击左侧的公链选项可以选择工具支持的公链，当前已支持：以太坊、bsc、polygon、avalanche、arbitrum、heco、okc、fantom、harmony、cronos更多的公链也正在陆续支持中。

切换公链后填入合约地址点击【检测】即可完成代币的合约检测。

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FMr66Ca6n3UR4Xw7gcij2%2Fuploads%2Fx4rrbMgf3AH7Vo7374EK%2F3%20%E6%8B%B7%E8%B4%9D.png?alt=media&token=d7cc4326-7c1f-4254-85a8-0f68bc7d659d" %}

4、熟悉了代币合约查看工具的入口和功能，下面带大家简单介绍下常见的一些【危险警告】和【安全提示】内容。

代理合约：代币合约代码里有绑定另一个合约，合约能控制他的增发，交易开关等功能，危险性较高。

貔貅代币：无法卖出代币，那么代币将没有任何价值。

白名单功能：加入白名单的人才可以买卖代币。

防巨鲸功能：防止大量资金买入获取代币的控制权。

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FMr66Ca6n3UR4Xw7gcij2%2Fuploads%2FQToxUYfh3abNiszMQPTZ%2F4%20%E6%8B%B7%E8%B4%9D.png?alt=media&token=bcbbb7da-1c92-4c80-b815-d4baa7c11e93" %}

黑名单功能：被加入黑名单的地址无法卖出代币，这种设置可以和杀机器人功能想配合。

增发功能：增加代币发行的功能，例如有些挖矿类的项目用来挖矿或者一些恶意的项目增加发行砸盘。

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FMr66Ca6n3UR4Xw7gcij2%2Fuploads%2FllY3uUkSrbbtdkLfJvre%2F5%20%E6%8B%B7%E8%B4%9D.png?alt=media&token=8fa5357a-4080-407f-ba85-b0edc2c6c7e2" %}

代币合约地址安全检测工具的推出可以在很大程度上规避一些恶意的代币，工具只是一个辅助的作用，它的准确率无法保证百分之百，后续功能会加入到行情界面的代币详情中。



3、独立版合约检测工具

打开TokenPocket，点击【发现】新品区可以找到独立检测工具，也可以单独打开链接[<mark style="color:blue;">**https://tokensecurity.tokenpocket.pro/?utm\_source=tokenpocket#/**</mark>](https://tokensecurity.tokenpocket.pro/?utm\_source=tokenpocket#/) 使用。

工具打开后可以点击左上角选择不同的公链，中间的位置可以填入需要检测的合约地址并点击检测。

![](<../../.gitbook/assets/01 拷贝.png>)

检测结果会分为几个大类显示，可以根据检测的结果来进行甄别。

![](<../../.gitbook/assets/03 .png>)
