# 通过自定义Nonce发送数据

在BTC、EVM等公链中，Gas的设置尤为重要，因为一旦设置了较低的Gas，那么就意味着这笔订单不会被 优先处理，而是处于pending的状态，就是我们俗称“卡住”了；那么遇到这种问题的时候，我们可以很方便的利用TokenPocket插件钱包中的自定义nonce来完成订单的取消或者是加速。

TokenPocket移动端默认支持订单的加速或取消功能，后续也会增加自定义nonce的功能。

### <mark style="color:orange;">如何设置自定义Nonce开关</mark> <a href="#1" id="1"></a>

打开TokenPocket插件钱包，点击右上角【菜单】，选择【设置】功能、

<figure><img src="../../.gitbook/assets/1 (1) (1).png" alt=""><figcaption></figcaption></figure>

在设置界面中点击【高级】选择自定义nonce，打开开关，就可以完成功能的启用。

<figure><img src="../../.gitbook/assets/2 (2) (5) (1).png" alt=""><figcaption></figcaption></figure>

### <mark style="color:orange;">使用自定义nonce设置转账</mark> <a href="#2" id="2"></a>

当遇到因为转账时支付了较少的Gas导致上链订单的pending状态时，就可以利用插件钱包自定义nonce功能来重新发送一笔和panding订单相同nonce值的转账，从而进行覆盖。

1、找到卡住的交易订单，并记录nonce值并记录，例如下图订单中的7。

<figure><img src="../../.gitbook/assets/3 (4) (2).png" alt=""><figcaption></figcaption></figure>

2、正常的填入转账参数，点击【下一步】，在GWEI中提高一定比例，例如百分之二十的数量，然后进行自定义nonce设置。

<mark style="color:red;">**需要注意的是：**</mark>

收款地址为自己的地址，增加gwei，设置自定义nonce后执行，相当于取消卡住的订单。

收款地址为其他地址，增加gwei，设置自定义nonce后相当于覆盖卡住的订单，并转出到对应的地址中。

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

自定义nonce中填入7，然后点击【确认】即可完成卡住订单（相同nonce值）的覆盖。

<figure><img src="../../.gitbook/assets/4 (1) (2).png" alt=""><figcaption></figcaption></figure>
