# 如何查看/取消恶意Approve（授权）？

Approve即授权。它允许持有 Token 的用户，通过调用 Approve 方法，授权给指定账户一定额度，赋予该账户自由支配额度内 Token 的权力。如果授权给恶意账户，那么授权资产就会有极大风险。

在本教程开始前，请点击以下文字，了解什么是Approve（授权）？

[about-approve.md](about-approve.md "mention")

**---移动端操作教程---**

1）打开TokenPocket APP，首先在资产页面选择对应的钱包网络，在\[发现页面]输入【DeBank】或【[https://debank.com/](https://debank.com)】，进入DeBank DApp，点击【连接钱包】，选择您所需要查询的钱包地址，点击下方【授权】按钮，进入授权管理页面；

<mark style="color:red;">**注：DeBank目前暂不支持TRON授权管理查询，请在本文最下方查阅取消TRON恶意授权操作教程。**</mark>

![](<../../.gitbook/assets/1 (22) (1) (1).png>)

2）以BSC地址为例，授权页面会出现钱包余额，其中Token总敞口为Token的总价值；点击价格旁边的小三角形，会出现该代币的相关授权信息：

<mark style="color:orange;">合约：授权的DApp/合约地址；</mark>

<mark style="color:orange;">授权额度：当授权额度为“Infinite”时，即为无限授权，允许把该代币余额全部授权给对方；</mark>

<mark style="color:orange;">风险敞口：授权代币的数量。</mark>

![](<../../.gitbook/assets/1 拷贝 (2).png>)

3）如您的钱包地址未进行过任何授权行为，则会显示【无匹配】；

![](<../../.gitbook/assets/1 拷贝 2.png>)

4）点击右方\[...]，点击【Cancel Approve】，支付取消授权所需要的矿工费；至此，您已完成取消恶意授权的操作。

![](<../../.gitbook/assets/1 拷贝 3拷貝.png>)

**----TRON授权查询---**

****

1.使用电脑打开TRON区块浏览器[https://tronscan.io/#/](https://tronscan.io/#/)，选择【连接钱包】，根据提示连接钱包

![](<../../.gitbook/assets/1 拷贝 11.png>)

2.进入「账户」页面。点击【授权列表】，即可查看钱包地址的授权情况；

![](<../../.gitbook/assets/1 拷贝 12.png>)

3.点击【取消授权】，由于TRON取消授权需要用到TronLink插件，因此点击取消授权后，请根据TronLink指引进行。

&#x20;

**如何确认恶意授权地址？**

**恶意授权地址有如下几个特征：**

特征一：来路不明的空投引诱

1.任意点开一个授权地址，点击【通证余额】，点开任意代币进行「通证转账」查看；

![](<../../.gitbook/assets/1 拷贝 13.png>)

2.在部分转账中，盗币者会附上备注，以空投为诱饵，让用户通过第三方的DApp来进行兑换。这是最常见的一种获取用户授权的方法，请注意防范！！切勿不要相信任何来路不明的空投，避免因小失大！！

![](<../../.gitbook/assets/1 拷贝 14.png>)

特征二：授权地址发行多个同类型代币

1.经过授权地址查看，发现该地址发行有多个TRC10的Token内容如下：

![](<../../.gitbook/assets/1 拷贝 15.png>)

2.这么多TRC10类型的Token，又不能在Swap中兑换，那肯定是另有他用，逐个点开查看Token得到以下内容：

![](<../../.gitbook/assets/1 拷贝 16.png>)

注：除此之外还有盗币者利用假的收款界面和用户进行转账交易，利用Approve恶意授权来达到盗币目的，所以一定要谨慎和他人交易。
