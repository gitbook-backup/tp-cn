# TokenPocket授权管理工具使用教程

一、打开TokenPocket，点击【发现】在顶部的地址栏中填入：[<mark style="color:blue;">**https://approval.tokenpocket.pro/**</mark>](https://approval.tokenpocket.pro/)打开使用，如果是安卓用户可以直接通过新品区打开授权检测工具。

<figure><img src="../../.gitbook/assets/0 拷贝.png" alt=""><figcaption></figcaption></figure>

二、工具打开后会根据当前的钱包公链进行识别和连接，暂时支持ETH和BSC公链，其他公链会在后续的更新中逐渐支持。我们可以通过地址栏使用自己的地址或者他人的地址进行查询。

查询分类中可以支持当前的【代币】和【NFT】的检测，界面检测结果也很直观，右上角可以切换深色模式。授权信息显示的内容如下：

1、授权的合约地址，可以点击查看链上数据；

2、授权的数量通常会默认无限制；

3、授权合约的时间；

4、授权合约的哈希值信息，点击查看链上数据。

<figure><img src="../../.gitbook/assets/1 (4).png" alt=""><figcaption></figcaption></figure>

三、点击【取消授权】会弹出执行授权操作的提示，授权管理的原理就是二次调用这个授权过的合约地址，将授权数量修改为0就达到了权限清理的目的。如果使用其他第三方链接访问时出现这个授权提示窗口就一定要谨慎，因为很可能会是有风险的授权，只有在你确认操作的链接是安全的，授权的合约也是正常调用后，才可以记录执行，否则遇到恶意授权链接，将会导致你授权过的代币全部被盗。

<figure><img src="../../.gitbook/assets/2 (5) (1).png" alt=""><figcaption></figcaption></figure>

四、确认支付后，会看到界面中【正在取消中】的提示，当完成数据执行后这条数据就会自动清理。

<figure><img src="../../.gitbook/assets/3 (3).png" alt=""><figcaption></figcaption></figure>
