# 官网正版钱包验证方法

App Store版本验证方法：[<mark style="color:blue;">**点击查看**</mark>](AppStore.md)<mark style="color:blue;">****</mark>

Google Play版本验证方法：[<mark style="color:blue;">**点击查看**</mark>](google.md)<mark style="color:blue;">****</mark>

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

<mark style="color:blue;">****</mark>[<mark style="color:blue;">**www.tokenpocket.pro**</mark>](https://www.tokenpocket.pro)<mark style="color:blue;">****</mark>

|  版本号  |               MD5值               |
| :---: | :------------------------------: |
| 1.5.5 | 0e2668727560344978dd523925a75a4b |
| 1.5.4 | f510204c4fa7533b05e729b902ebec59 |
| 1.5.3 | 4ebc793117ce677fb07602e31256e7cc |
| 1.5.2 | 10e6f64debae79bf1e40bd830c6a819e |
| 1.5.1 | c30cbf152acc15c5cffafaf7a7a387ad |
| 1.5.0 | aed562118bd5d8c64578f3b52a7b2460 |
| 1.4.9 | bbe46949fcc243ad113c45ec19ce9215 |
| 1.4.8 | 5c5cb0676c72c8d554091ad5a7608471 |
| 1.4.7 | 618c2017ce7f9f75bbdfe09ae06a4467 |

|  版本号  |                              SHA256值                             |
| :---: | :--------------------------------------------------------------: |
| 1.5.5 | 76bc787cd5933f6f2cd40b7cc227038995c7717985ebaf9031fa61154b0f6360 |
| 1.5.4 | 84e5382013fd5625d684d02836f001d126c31196635e5b1630bc36710ef7afe7 |
| 1.5.3 | 4b35d2b8237b9708b12d1386527b3a6c233a641a989f7c63b9512cdc522af219 |
| 1.5.2 | f357cf564293ad09026170949e7b69e13342b47e57880200b6575c0e596c4e99 |
| 1.5.1 | f1eb4e4571c9c1e08771ffcd896c6aaab63097e2ddda0d00232754d114dc9313 |
| 1.5.0 | cf2e8aa6a324f2059b5ec5035ed7fbe27f2ea2d2c7f3792672a803900aa2e37c |
| 1.4.9 | d8f605a142c6140905cf25a829f0be10d402e232ce1717013553aaec443d6946 |
| 1.4.8 | 5dedd0c8c793c5f22a3d8d4703e31a6fc5e8d483159b31a1fe64265eefc1f7c3 |
| 1.4.7 | 02182af2d93d3c3d63985986c2a0b8c9506223abe15a59278caf67e84f2efece |

<mark style="color:blue;">**Google Play**</mark>

|  版本号  |               MD5值               |
| :---: | :------------------------------: |
| 1.5.4 | 53936f73be5c90dce02ea06919f29fb0 |
| 1.5.3 | 24a1df1bc85cdb1c34c780c217ee9c1d |
| 1.5.2 | 938e9252cb21fef1c40fac3c4c9492c6 |
| 1.5.1 | f879845afd51d51fabf42e653011da79 |
| 1.5.0 | a951c032f8723cc1711f0d3b3256725d |
| 1.4.9 | 4b88e2ffa2b3d84fbc2f099e1034fb86 |
| 1.4.7 | feab610e82a1ed694d24994487f3e38c |

|  版本号  |                              SHA256                              |
| :---: | :--------------------------------------------------------------: |
| 1.5.4 | d4edad4a5277efc29fc896fcabe71a8f17de1fbf69944e340b52a0709dab9695 |
| 1.5.3 | 30d50fc1f9f008bbfb3bb33fd5d04f6dcd6e3fb1c9b37ab5ec1815d6c9391bed |
| 1.5.2 | dfaf358d6f30ead51b52193a5aab8259fd52ac5d8372b47a97951c799842b988 |
| 1.5.1 | a4162187fac4a623ab5762d15953ae17e659e3c6fa518615a70d8046d2f01355 |
| 1.5.0 | c7f8b8a603d8725ba1df631cf03f2c63dc4c428b5ffe1f3ae3eec400bf3d121b |
| 1.4.9 | 37b571b7644e456be7260e3d1d93ce59d9e38f694215c85e29e4a1476b6bf634 |
| 1.4.7 | b023f39e496ac6a38cc0ef121470cc7c2142f393c75aea504bc8ab979285dffd |

### <mark style="color:blue;">**在线验证MD5、sha256工具**</mark>

在线验证md5\sha256值的工具有很多，他们的使用也都是大同小异，只需要将下载到pc上的apk文件拖入或者加载到验证平台中即可等待结果，得到的结果和TokenPocket官网公布的正版APP的md5或sha256值做比对即可验证。<mark style="color:red;">（在线工具页面中可能存在广告等内容，请使用主要验证功能，其他的不做任何推荐）</mark>

工具一：打开链接[<mark style="color:blue;">**https://www.dute.org/file-hash-validator**</mark>](https://www.dute.org/file-hash-validator) <mark style="color:blue;">****</mark> 选择哈希算法，通常使用比较广泛的是md5，最安全的算法是sha256，其他的哈希算法也可以进行尝试。在顶部选择或拖入下载的APK文件后底部会很快得到计算结果，只需要复制结果和官方公布的md5或sha256哈希值进行对比即可完成验证。

![](../../.gitbook/assets/256-2.png)

工具二：打开链接[<mark style="color:blue;">**http://www.metools.info/code/c92.html**</mark>](http://www.metools.info/code/c92.html)  <mark style="color:blue;">****</mark>  选择文件和哈希算法，点击计算，即可在结果中查看到结果。

![](../../.gitbook/assets/256-1.png)

工具三：打开链接[<mark style="color:blue;">**https://oktools.net/file-hash**</mark>](https://oktools.net/file-hash)  <mark style="color:blue;">****</mark>  这款工具可以快捷的选择多个哈希算法来验证，只需要勾选哈希算法，导入APK文件后即可查看到结果，非常方便。

![](../../.gitbook/assets/256-3.png)

### <mark style="color:blue;">**PC端MD5、SHA256验证工具**</mark>

MD5工具：打开工具的官网[<mark style="color:blue;">**https://www.winmd5.com/**</mark>](https://www.winmd5.com/) <mark style="color:blue;">****</mark> 点击【Download】下载工具

![](../../.gitbook/assets/Snipaste\_2022-06-20\_21-24-51.png)

下载完成后，打开工具，此工具只可验证md5值，点击【browse】选择下载的APK文件，导入后即可看到下方提示的md5值。

![](../../.gitbook/assets/Snipaste\_2022-06-20\_21-31-00.png)

SHA256工具：

这个工具是我们熟悉的压缩/解压缩工具7-Zip，通过它也可以非常便捷的得到文件的SHA256值

打开官网[<mark style="color:blue;">**https://www.7-zip.org/**</mark>](https://www.7-zip.org/) <mark style="color:blue;">****</mark> 点击【Download】下载对应的版本并安装

![](../../.gitbook/assets/Snipaste\_2022-06-20\_21-29-07.png)

安装完成后，只需要在下载的APK文件上点击右键，选择【7-Zip】--【CRC SHA】--【SHA-256】

![](../../.gitbook/assets/Snipaste\_2022-06-20\_21-38-02.png)

即可看到SHA256哈希值。

![](../../.gitbook/assets/Snipaste\_2022-06-20\_21-40-10.png)

### <mark style="color:blue;">**移动端MD5、SHA256验证工具**</mark>

虽然在电脑端可以使用多种工具多种渠道来查看md5或sha256哈希值，但是我们日常使用最多的移动端如何进行验证呢。这里来介绍下移动端的工具。

工具一：点击这里[<mark style="color:blue;">**下载工具**</mark>](https://d-13.winudf.com/b/APK/Y29tLmdhbWUubGl0dGxldHJpY2tzdHVkaW8ubWQ1Y2hlY2tlcl8xMV9jNGNjM2U1Ng?\_fn=TUQ1IENoZWNrZXJfdjEuM19hcGtwdXJlLmNvbS5hcGs&\_p=Y29tLmdhbWUubGl0dGxldHJpY2tzdHVkaW8ubWQ1Y2hlY2tlcg\&am=PGLTTfIPJr33xxAxPVydqQ\&at=1655734447\&download\_id=otr\_1705904481071926\&k=3919882866ce239957fb9d9a76fd5b6762b1d230\&r=https%3A%2F%2Fapkpure.com%2Fcn%2Fmd5-checker%2Fcom.game.littletrickstudio.md5checker) <mark style="color:blue;">****</mark> 安装后，打开验证工具，点击选择打开系统自带的文件管理器，找到需要验证的的APK文件，导入后点击【MD5】就可以计算出md5哈希值，可以和官方提供的参数进行对比。

![](<../../.gitbook/assets/1 (27) (1).png>)

工具二：点击[<mark style="color:blue;">**下载工具**</mark>](https://cr5.198254.com/com.hobbyone.hashdroid.apk) <mark style="color:blue;">****</mark> 这款工具的功能更加强大，支持md5、sha256等多种哈希算法验证。同样的安装打开后，点击切换到【HASH A FILE】，点击【Select a hash function】选择例如sha256，点击【CLICK HERE TO SELECT THE FILE TO HASH】来找到需要验证的apk，加载后点击【CALCULATE】即可计算出apk的sha256哈希值用于和官方的参数进行对比。

![](<../../.gitbook/assets/2 (20).png>)

