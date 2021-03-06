# Dapp授权诈骗

在日常操作例如DEX平台，涉及到币币兑换的时候就会用到授权的功能，只有首次操作授权（Approve）后才可以进行Swap的币币兑换，这个只是应用场景之一。由于Approve操作本质上是将你的部分Token的行使权限授予了另一普通地址或智能合约地址，因此有些骗子利用二维码或者链接的方式来恶意让用户执行Approve操作。例如空投给用户的代币中留下链接，声称可以使用空投的代币来兑换其他代币，用户打开链接并执行兑换的过程中就完成了骗子特定的Dapp恶意授权，从而导致用户资产会被该Dapp随意划转。

**如何判断approve是否安全？**

Approve产品是否开源是否开源  
代码开源可以让用户更好的知道Approve的权限，即该产品在什么情况下可以转走用户的资产。

Approve产品是否开源是否经过审计   
经过审计的项目比未审计的安全性更高。

Approve产品是否来历不明   
来历不明的产品必须警惕，而例如Uniswap这类知名产品让大家更为放心。

**如何查询我的approve操作，怎么取消approve？**  
目前市面上针对普通用户的approve查询工具有Etherscan、CoinTool、Approved、Approve.sh等等，用户可以查询自己的approve情况，还可以取消approve操作。

