# 官网正版钱包验证方法

App Store版本验证方法：[<mark style="color:blue;">**点击查看**</mark>](AppStore.md)

Google Play版本验证方法：[<mark style="color:blue;">**点击查看**</mark>](google.md)

### <mark style="color:blue;">MD5、SHA256验证工具</mark>

文件哈希验证工具是通过计算文件内容哈希值的工具。通过工具可以快速计算文件的哈希值，计算出来的 Hash 值与官方给出的 Hash 值进行对比，可以验证文件内容是否被篡改。

### <mark style="color:blue;">MD5、SHA256验证的目的</mark>

去中心化自托管钱包是我们导入私钥或助记词以管理链上资产的平台，所以对于平台的选择和使用尤为重要。TokenPocket作为用户众多的去中心化自托管钱包自然也受到了不法分子的“惦记”，他们通过反编译的方式将正版APK中植入可以导入私钥，助记词的设置，然后打包发布到其他网站中“守株待兔”，当用户通过搜索引擎或者他人推荐的方式下载和使用了钱包，那么他的私钥助记词将发生泄露，从而丢失所有资产。

近期从邮件和社区的渠道反馈的情况来看，假钱包盗币的案例有所上升，所以我们专门制作本期教程，通过验证MD5\sha256值，利用在线工具，pc端和移动端多个平台验证，希望能提高大家的安全意识，学会合理使用工具来保护自己的链上资产安全。

请认准TokenPocket唯一官网地址：www.tokenpocket.pro

### <mark style="color:blue;">MD5和SHA256算法的区别</mark>

**相同点：**

1、都是密码散列函数，加密不可逆。

2、都可以实现对任意长度对象加密，都不能防止碰撞。

**安全性方面：**

1、SHA256（称SHA2）的安全性最高，但是耗时要其他两种多一些。

2、md5相对来说比较容易碰撞，安全性没这么高。

### <mark style="color:blue;">**官方钱包APK的MD5、SHA256参数：**</mark>

<mark style="color:red;">**后续MD5和SHA256将通过官网进行同步,请点击下方进入官网查看**</mark>

{% embed url="https://verify.tpwallet.io/" %}

<table><thead><tr><th width="98.42857142857139" align="center">版本号</th><th width="276.57142857142867" align="center">MD5值</th><th align="center">SHA256值</th></tr></thead><tbody><tr><td align="center">1.7.7</td><td align="center">a541123d07cbd3a470bb0677fd504416</td><td align="center">e9199faec736c78854ad894c83b1ebe66e4ecaba6869ccc481e893ae8ab095c4</td></tr><tr><td align="center">1.7.6</td><td align="center">f62a4febd1413f9c8d2b8bfafcc61e2c</td><td align="center">d7161c60d29c1743a254ec54b657fbe13aa3187b0863f45de9910812c3b8b10d</td></tr><tr><td align="center">1.7.5</td><td align="center">b963703ad2e2301b1aac4d449dfedb41</td><td align="center">0496c0ecb5a719a642279a8233405a71e09867e1978d5aed38f6fc45973d057b</td></tr><tr><td align="center">1.7.4</td><td align="center">e943ca5b2ff356e9e1fe0133b90a22fb</td><td align="center">81cd881a8c3aace2d76d9247e174db48cec4fe50d2e7e5289c9ff20eaf056b52</td></tr><tr><td align="center">1.7.3</td><td align="center">1894510ae8b325d148f3a02f2e3f57f8</td><td align="center">41007ee8cdc96f179a05400ef34aa44d541feda23ebe95b1248b868242625fe9</td></tr><tr><td align="center">1.7.2</td><td align="center">9262f28f781e61852a34b97d23f6acd1</td><td align="center">97935dbb3c0ce607a3d0bf8d66fe18d5a17213cef8758a6f067fcf2823bc9db5</td></tr><tr><td align="center">1.7.1</td><td align="center">39a61a17e5b3b0de501c29ee8d2d5d22</td><td align="center">3ece643ba4599a00be1ae5f580814dcabaf4daa8f292d21b92c5724a2a28a006</td></tr><tr><td align="center">1.7.0</td><td align="center">e2bbf4e2a9dfb1f52e079028a61f3d7c</td><td align="center">d46b6a2d90715dd21329ae071f03b4098eef172eae7cc998fbe4c805c338f7bc</td></tr><tr><td align="center">1.6.9</td><td align="center">357d37f7d57b6e5efb3d43c250272c79</td><td align="center">2519682c8793e6730aa6fa58b3373995d07b7e1c44da5c740c4254d49b393bd3</td></tr><tr><td align="center">1.6.8</td><td align="center">93cee34fb006c1fec1f907f563f1bde1</td><td align="center">57b4ede95f6ea09bac2efcbe921fbee07fccf1c7f6b93a0c3ead58d01dd9c020</td></tr><tr><td align="center">1.6.7</td><td align="center">656e5cb41674a7cb3d0429a87c47da5a</td><td align="center">fbd7757f8ff344eb9bf2d9f6c7a01f93281921d818c402b62fb5204059d4c6db</td></tr><tr><td align="center">1.6.6</td><td align="center">b7743e84040df7d5bef6f141621eaf9d</td><td align="center">44172fa9d715a35abf9dd4cad22031e20b5f2ac4514ba56d07e7ced11f75522b</td></tr><tr><td align="center">1.6.5</td><td align="center">65b6a3472335b71b3818bbe2d35a706b</td><td align="center">b281d49fd4a0c40e62af58960554414627788e858ab716ada242ec028fd95d0a</td></tr><tr><td align="center">1.6.4</td><td align="center">f1d22c3f3c5f7c567727a54ae7d68eae</td><td align="center">4c0f0ee20a96f1f4594fc8defbbd7d68ecb1d13080b627e3daf3b233b87baa97</td></tr><tr><td align="center">1.6.3</td><td align="center">1c0dd378f9fa6cd4e3c645380ae314b9</td><td align="center">3147424a71f6df65f63c3e92564cf7d55e8b748c79546d929a2938fe47ffdcb7</td></tr><tr><td align="center">1.6.2</td><td align="center">593210fc806f37fc9e6b979909414d52</td><td align="center">77063b71a05c12b0d3328ae983417f8b27fe3d2f038a03e0a098266a31659651</td></tr><tr><td align="center">1.6.1</td><td align="center">2b5c73f176a895135dbfb6ab9337eabb</td><td align="center">d959026cc4442dac8f835701c48fe75d029edd5ed9b94b8740f2022c3b8b6eda</td></tr><tr><td align="center">1.6.0</td><td align="center">4985a5d4a8a45f98ccfdf1d039ecf926</td><td align="center">761cb44ca6be823e11b6e0301fa818aa7fbb4d8b277e8c8e6ba1f7dfe0cf2ae0</td></tr><tr><td align="center">1.5.9</td><td align="center">f4c74ec4d08e26c53ccbcfcdb20c35b3</td><td align="center">cc7daf17bd4a8ac52ee00f1eec49f87a4f081568b42c56280318b804ac744971</td></tr><tr><td align="center">1.5.8</td><td align="center">4903a5900f0e55daa2bcbb1d5207f4d0</td><td align="center">dfbfcf2ad563fc6aaec87380732bea159f6cf648b13f9397218fd3694b7744e3</td></tr><tr><td align="center">1.5.7</td><td align="center">343daaecd1618922b9ef9c2811ce61d7</td><td align="center">24d46dd0a2e899b5ec047ba860375f5d07ff9d4ecc75e914d34f8a423d2af143</td></tr><tr><td align="center">1.5.6</td><td align="center">b90aca7a51d0b01d21530d987ed5d564</td><td align="center">1861aa2a7afdc5430f2517e9286a65ccbd1a8de42e9d6596b687ae8aa4b43da3</td></tr><tr><td align="center">1.5.5</td><td align="center">0e2668727560344978dd523925a75a4b</td><td align="center">76bc787cd5933f6f2cd40b7cc227038995c7717985ebaf9031fa61154b0f6360</td></tr><tr><td align="center">1.5.4</td><td align="center">f510204c4fa7533b05e729b902ebec59</td><td align="center">84e5382013fd5625d684d02836f001d126c31196635e5b1630bc36710ef7afe7</td></tr><tr><td align="center">1.5.3</td><td align="center">4ebc793117ce677fb07602e31256e7cc</td><td align="center">4b35d2b8237b9708b12d1386527b3a6c233a641a989f7c63b9512cdc522af219</td></tr><tr><td align="center">1.5.2</td><td align="center">10e6f64debae79bf1e40bd830c6a819e</td><td align="center">f357cf564293ad09026170949e7b69e13342b47e57880200b6575c0e596c4e99</td></tr><tr><td align="center">1.5.1</td><td align="center">c30cbf152acc15c5cffafaf7a7a387ad</td><td align="center">f1eb4e4571c9c1e08771ffcd896c6aaab63097e2ddda0d00232754d114dc9313</td></tr><tr><td align="center">1.5.0</td><td align="center">aed562118bd5d8c64578f3b52a7b2460</td><td align="center">cf2e8aa6a324f2059b5ec5035ed7fbe27f2ea2d2c7f3792672a803900aa2e37c</td></tr><tr><td align="center">1.4.9</td><td align="center">bbe46949fcc243ad113c45ec19ce9215</td><td align="center">d8f605a142c6140905cf25a829f0be10d402e232ce1717013553aaec443d6946</td></tr><tr><td align="center">1.4.8</td><td align="center">5c5cb0676c72c8d554091ad5a7608471</td><td align="center">5dedd0c8c793c5f22a3d8d4703e31a6fc5e8d483159b31a1fe64265eefc1f7c3</td></tr><tr><td align="center">1.4.7</td><td align="center">618c2017ce7f9f75bbdfe09ae06a4467</td><td align="center">02182af2d93d3c3d63985986c2a0b8c9506223abe15a59278caf67e84f2efece</td></tr></tbody></table>

<mark style="color:blue;">**Google Play**</mark>

<table><thead><tr><th width="101" align="center">版本号</th><th width="276" align="center">MD5值</th><th align="center">SHA256值</th></tr></thead><tbody><tr><td align="center">1.7.7</td><td align="center">8209c2cb87b445d42f5195096a8b638c</td><td align="center">83944469998e7ab804fa4c49e8413c5b2f52cb968a93c64036432c25c9f2ce4e</td></tr><tr><td align="center">1.7.6</td><td align="center">6f49b9bced7b9518c0c743fec275b02c</td><td align="center">9a662df82d0395ce2b1ddeb7ad2820704c2fa2e7aa90ea995278806af2f8695c</td></tr><tr><td align="center">1.7.5</td><td align="center">68a869eaec857d67099a153802f039a1</td><td align="center">bfd445455d0f6f926aba9a0db332070d3399e2fa20454af5cb6d7f4c574f8f6d</td></tr><tr><td align="center">1.7.4</td><td align="center">a3db8395c1a6f9896032c3f239f94e48</td><td align="center">1e08dfbfb1ae6f343cc742e1b0bb36f1fc1005439aadc386b215a7765fa39b70</td></tr><tr><td align="center">1.7.3</td><td align="center">19904e8d6a3a64029e24cb3d1376390b</td><td align="center">683efdffcdcf7463f876f239093f259cbb0d202e7517c9ff7ded722a2e776be6</td></tr><tr><td align="center">1.7.2</td><td align="center">ea468f2ba3ccf4319eeae2fe5c7b07c1</td><td align="center">3a630581244f49fcd317c363d61d19e265906de8d1b2d6bbd66615832333a61f</td></tr><tr><td align="center">1.7.1</td><td align="center">e8d383a622eda37d07933cf80b647fc2</td><td align="center">da92c35440b0ef344b8cbccd543503440649fb0c14e3020c64574b534d39620a</td></tr><tr><td align="center">1.7.0</td><td align="center">d441edf5c94e57adab597e3245c1a74a</td><td align="center">6b310e3b8f97e9f36b52adbbe43ddb810e043db4db3fa94644f764ae3768095a</td></tr><tr><td align="center">1.6.9</td><td align="center">ec200454c69b687a7b7dd54c59acf56b</td><td align="center">b6baf6792caa7baf0b1740f33b23b07e922e8299c7e9c02f53b9f80b7b80ee5a</td></tr><tr><td align="center">1.6.8</td><td align="center">8175797b8739dfd27f6f25a55bdce6d3</td><td align="center">a49f4843269d88445532f982c893a41dc069922b51d4ea9b36a6a9c191a405f1</td></tr><tr><td align="center">1.6.7</td><td align="center">8c3c5e706f9b03cca0f0458417f202c3</td><td align="center">8c96b54ea00f8c826e2be84e25b0446864e013de9b270d4fe9b6f60ed40be400</td></tr><tr><td align="center">1.6.6</td><td align="center">73501df3c495a38b9b2c6ff24eeeba1e</td><td align="center">e75e6dd6afcb87bfb78e983be6b2c2eddb42fccba70f6d0bf41cbb87648c121b</td></tr><tr><td align="center">1.6.5</td><td align="center">89ad8d584810046a1b261e8ad555ec82</td><td align="center">ae97bf1f7d3bb5917b46bfeb3d052830c7f5ee584c6486ecbc65e1693f9fe359</td></tr><tr><td align="center">1.6.4</td><td align="center">951dfeb5d7265fa7c132eeeceb780864</td><td align="center">3afd9ac7c74424d475bd4cf00ac2b6a662a5ae5a5d562529d3aaf2f4fd729311</td></tr><tr><td align="center">1.6.3</td><td align="center">c60ab2f42f48c379ab36f761daf3589e</td><td align="center">b979b36df3839edf51e8c15dbedcf0367359c55008403ebb5b662a473b35f64b</td></tr><tr><td align="center">1.6.2</td><td align="center">f8df3cef27738ecd4e195e6fed7fe8d0</td><td align="center">dde7014d51df68b8de3905174c666331c307e1ed96dbe9cd51e0a8da00bc6abd</td></tr><tr><td align="center">1.6.0</td><td align="center">66bceb6daeb4b40f736d15f6b38b0d9e</td><td align="center">003d5141a4f442772a9e8a8ede57b543054b72d746df050aa48d7a5349c3c479</td></tr><tr><td align="center">1.5.9</td><td align="center">88c4d55959c9da313db6acc73ea0d656</td><td align="center">59ad89d7dbf09a27b5a37e94dd9063178fbb69614367e5b10dfb3944d266249a</td></tr><tr><td align="center">1.5.8</td><td align="center">f744d05688acf4a67509c14639829545</td><td align="center">0c2fd1998d10f364e83749a12c388f681acc6fad85212c7441a9cb7b54649460</td></tr><tr><td align="center">1.5.7</td><td align="center">a1ef0ae6f7a616a85e3cc2645723b07e</td><td align="center">6ce904535ab4035bf1a4ea5ef001c1f82baf9ead660a880b2b4a2244b48f95d8</td></tr><tr><td align="center">1.5.6</td><td align="center">fe1eed863c1214c508d41293537944e8</td><td align="center">f49e4516c547d2f7a6f4d2a577332d5d63ee0b36ea5a73b7d813452d22b2ce5f</td></tr><tr><td align="center">1.5.5</td><td align="center">10e6d8860e2b0a1253a3fc9a541ac3a9</td><td align="center">95ca32929a294f90de3a2f62ceb792cc4fa442ee632e5df810a6d2bd8b44325d</td></tr><tr><td align="center">1.5.4</td><td align="center">53936f73be5c90dce02ea06919f29fb0</td><td align="center">d4edad4a5277efc29fc896fcabe71a8f17de1fbf69944e340b52a0709dab9695</td></tr><tr><td align="center">1.5.3</td><td align="center">24a1df1bc85cdb1c34c780c217ee9c1d</td><td align="center">30d50fc1f9f008bbfb3bb33fd5d04f6dcd6e3fb1c9b37ab5ec1815d6c9391bed</td></tr><tr><td align="center">1.5.2</td><td align="center">938e9252cb21fef1c40fac3c4c9492c6</td><td align="center">dfaf358d6f30ead51b52193a5aab8259fd52ac5d8372b47a97951c799842b988</td></tr><tr><td align="center">1.5.1</td><td align="center">f879845afd51d51fabf42e653011da79</td><td align="center">a4162187fac4a623ab5762d15953ae17e659e3c6fa518615a70d8046d2f01355</td></tr><tr><td align="center">1.5.0</td><td align="center">a951c032f8723cc1711f0d3b3256725d</td><td align="center">c7f8b8a603d8725ba1df631cf03f2c63dc4c428b5ffe1f3ae3eec400bf3d121b</td></tr><tr><td align="center">1.4.9</td><td align="center">4b88e2ffa2b3d84fbc2f099e1034fb86</td><td align="center">37b571b7644e456be7260e3d1d93ce59d9e38f694215c85e29e4a1476b6bf634</td></tr><tr><td align="center">1.4.7</td><td align="center">feab610e82a1ed694d24994487f3e38c</td><td align="center">b023f39e496ac6a38cc0ef121470cc7c2142f393c75aea504bc8ab979285dffd</td></tr></tbody></table>

### <mark style="color:blue;">**在线验证MD5、sha256工具**</mark>

在线验证md5\sha256值的工具有很多，他们的使用也都是大同小异，只需要将下载到pc上的apk文件拖入或者加载到验证平台中即可等待结果，得到的结果和TokenPocket官网公布的正版APP的md5或sha256值做比对即可验证。<mark style="color:red;">（在线工具页面中可能存在广告等内容，请使用主要验证功能，其他的不做任何推荐）</mark>

工具一：打开链接[<mark style="color:blue;">**https://www.dute.org/file-hash-validator**</mark>](https://www.dute.org/file-hash-validator) 选择哈希算法，通常使用比较广泛的是md5，最安全的算法是sha256，其他的哈希算法也可以进行尝试。在顶部选择或拖入下载的APK文件后底部会很快得到计算结果，只需要复制结果和官方公布的md5或sha256哈希值进行对比即可完成验证。

![](../../.gitbook/assets/256-2.png)

工具二：打开链接[<mark style="color:blue;">**http://www.metools.info/code/c92.html**</mark>](http://www.metools.info/code/c92.html)  选择文件和哈希算法，点击计算，即可在结果中查看到结果。

![](../../.gitbook/assets/256-1.png)

工具三：打开链接[<mark style="color:blue;">**https://oktools.net/file-hash**</mark>](https://oktools.net/file-hash)  这款工具可以快捷的选择多个哈希算法来验证，只需要勾选哈希算法，导入APK文件后即可查看到结果，非常方便。

![](../../.gitbook/assets/256-3.png)

### <mark style="color:blue;">**PC端MD5、SHA256验证工具**</mark>

MD5工具：打开工具的官网[<mark style="color:blue;">**https://www.winmd5.com/**</mark>](https://www.winmd5.com/) 点击【Download】下载工具

![](../../.gitbook/assets/Snipaste\_2022-06-20\_21-24-51.png)

下载完成后，打开工具，此工具只可验证md5值，点击【browse】选择下载的APK文件，导入后即可看到下方提示的md5值。

![](../../.gitbook/assets/Snipaste\_2022-06-20\_21-31-00.png)

SHA256工具：

这个工具是我们熟悉的压缩/解压缩工具7-Zip，通过它也可以非常便捷的得到文件的SHA256值

打开官网[<mark style="color:blue;">**https://www.7-zip.org/**</mark>](https://www.7-zip.org/) 点击【Download】下载对应的版本并安装

![](../../.gitbook/assets/Snipaste\_2022-06-20\_21-29-07.png)

安装完成后，只需要在下载的APK文件上点击右键，选择【7-Zip】--【CRC SHA】--【SHA-256】

![](../../.gitbook/assets/Snipaste\_2022-06-20\_21-38-02.png)

即可看到SHA256哈希值。

![](../../.gitbook/assets/Snipaste\_2022-06-20\_21-40-10.png)

### <mark style="color:blue;">**移动端MD5、SHA256验证工具**</mark>

虽然在电脑端可以使用多种工具多种渠道来查看md5或sha256哈希值，但是我们日常使用最多的移动端如何进行验证呢。这里来介绍下移动端的工具。

工具一：点击这里[<mark style="color:blue;">**下载工具**</mark>](https://m.apkpure.com/cn/md5-checker/com.game.littletrickstudio.md5checker/download) 安装后，打开验证工具，点击选择打开系统自带的文件管理器，找到需要验证的的APK文件，导入后点击【MD5】就可以计算出md5哈希值，可以和官方提供的参数进行对比。

![](<../../.gitbook/assets/1 (27) (1).png>)

工具二：点击[<mark style="color:blue;">**下载工具**</mark>](https://cr5.198254.com/com.hobbyone.hashdroid.apk) 这款工具的功能更加强大，支持md5、sha256等多种哈希算法验证。同样的安装打开后，点击切换到【HASH A FILE】，点击【Select a hash function】选择例如sha256，点击【CLICK HERE TO SELECT THE FILE TO HASH】来找到需要验证的apk，加载后点击【CALCULATE】即可计算出apk的sha256哈希值用于和官方的参数进行对比。

![](<../../.gitbook/assets/2 (20) (2).png>)

