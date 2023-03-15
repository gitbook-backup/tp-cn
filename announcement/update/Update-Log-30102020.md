# 版本更新日志（30/10/2020）

**【版本更新详情】**

Android最新版本号：1.1.2

iOS pro/+/++ 3.1.2(63) plus 3.1.3(63)

**【主要更新内容】**

1 支持币安智能链WalletConnect方式

2 货币单位优化

3 波场DAppFeeLimit 提示

4 以太坊交易状态优化

5 iOS支持DApp浮窗

**【版本更新方式】**

安卓：在APP内更新或在www.tokenpocket.pro 官网下载覆盖安装即可。0.9.9版本用户需要通过官网下载覆盖更新。

苹果：Pro/Plus版本需要配合testflight下载或更新（[**下载教程**](https://www.yuque.com/tokenpocket/gz8u7f/ktgryh)）

注：近期部分用户反馈testflight打开会报错，这里提供一个解决方法：打开苹果手机，点击桌面--选择设置 --点击wifi --点击当前连接wifi右侧的小叹号，下拉选择配置DNS 点击选择手动，下方DNS服务器删除其他项 添加8.8.4.4的谷歌DNS 保存后再次打开Testflight使用即可。（[**电梯直达**](https://www.yuque.com/tokenpocket/gz8u7f/fzigb3)）

**【更新功能介绍】**

**#1** 支持智能链WalletConnect，这里需要说明的是：我们用的是智能链的chainId，DApp识别不出来（因为DApp没支持），个别钱包给的是eth的chainId，DApp识别的也是eth的chainId ！哪怕是链接上，也是无法显示余额和正常操作的。等DApp开始支持的时候，这项功能就可以用了，这里只是先开发出来待用。

![](<../../.gitbook/assets/image (8) (1) (1).png>)

**#2** 货币单位进行优化，加入中文备注和多货币（法币单位）支持。

![](<../../.gitbook/assets/image (6) (1) (1).png>)

**#3** 波场DAppFeeLimit 提示 ，弹出授权窗口点击左下角【关于网络费相关说明】即可查看相关介绍内容。

![](<../../.gitbook/assets/image (11) (1).png>)

**#4** 以太坊交易订单状态优化，主要是针对例如Pending订单在被其他成交订单所替换后的【打包中】的状态进行优化。

**#5** iOS支持DApp浮窗，这个需要等待Testflight版本更新后再做图片展示。
