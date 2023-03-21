# revoke.cash授权管理工具使用

1、打开TokenPocket，点击【发现】，App Store版本的用户需要在顶部的地址栏中填入[<mark style="color:blue;">https://revoke.cash</mark>](https://revoke.cash)链接打开，如果是安卓用户可以直接搜索revoke.cash打开使用。

<figure><img src="../../.gitbook/assets/1 (1) (1).png" alt=""><figcaption></figcaption></figure>

2、工具打开后点击标记1处选择需要管理授权的公链，然后点击【Connect Wallet】连接钱包，如果是App Store用户，建议您点击右上角的【...】菜单收藏日常使用的DApp链接到发现界面中。

<figure><img src="../../.gitbook/assets/2 (1) (1).png" alt=""><figcaption></figcaption></figure>

3、连接钱包后，可以看出自动扫描的代币历史授权记录，revoke.cash可以查询Token和NFT的授权信息。

界面中看到显示0的信息说明是可以更新授权数量的记录，只需要点击【Update】在钱包中会弹出【即将执行授权管理】的提示，因为我们操作的授权管理原理上就是重新调用授权过的合约地址，然后对它的授权数量进行清零或者自定义数量设置，达到管理授权的目的。

<mark style="color:red;">**如果是访问第三方的DApp看到执行授权的提示就一定要谨慎，往往恶意授权链接都会通过授权USDT代币来达到盗币的目的。**</mark>

<figure><img src="../../.gitbook/assets/3 (1) (2) (1).png" alt=""><figcaption></figcaption></figure>

4、在弹出的【交易详情】界面中可以看到，授权地址就是我们已经授权过的合约地址，代币的数量为0（也可以自定义数量），确认信息后点击【确认支付】这个过程会消耗一定Gas（矿工费），完成授权后可以看到顶部的成功提示信息，这时候授权列表里的操作清零的授权记录会消失，授权管理操作完成。

<figure><img src="../../.gitbook/assets/4 (5).png" alt=""><figcaption></figcaption></figure>
