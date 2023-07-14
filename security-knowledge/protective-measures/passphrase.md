# 使用Passphrase功能创建“隐藏钱包”

### <mark style="color:orange;">Passphrase是什么</mark> <a href="#c7ydi" id="c7ydi"></a>

当创建隐藏钱包时，Passphrase是一种用于加密和保护钱包的重要工具。它通常是一个由单词或短语组成的字符串，用于创建钱包的私钥或种子短语。

Passphrase的目的是增加钱包的安全性，确保只有持有正确Passphrase的人能够访问和控制钱包中的资产。如果没有正确的Passphrase，就无法恢复或重建钱包，因此保管好Passphrase非常重要。

### <mark style="color:orange;">使用Passphrase时需要注意的安全事项</mark> <a href="#eizea" id="eizea"></a>

**保密性：**不要将Passphrase泄露给他人。确保只有您知道和持有Passphrase。避免在社交媒体、聊天应用或公共场所中透露Passphrase。

**复杂性：**选择一个足够复杂的Passphrase。它应该包含随机的单词或短语，并避免使用容易被猜测的内容，如常见的短语、日期、个人信息等。使用随机密语（密码短语）生成器来创建强密语可以提高安全性。

**备份：**确保正确备份Passphrase。将其写在纸上，并将纸本备份存放在安全的地方，远离网络和物理威胁。不要仅仅依赖于电子设备或在线存储，因为它们可能会遭受数据丢失、故障或黑客攻击。

**定期更换：**定期更换Passphrase是一个好的安全实践，尤其是如果您怀疑Passphrase可能已经泄露或不再安全。Passphrase更换，也意味着您的钱包地址跟着更换了！

**谨防钓鱼攻击：**注意钓鱼攻击，不要点击来自未知来源或可疑网站的链接，以防止被诱导输入Passphrase。

<mark style="color:red;">请记住，助记词和Passphrase必须同时持有才可以顺利导入“隐藏钱包”；Passphrase设置后无法二次导出，请务必正确记录。</mark>

<mark style="color:red;">我们建议在首次使用Passphrase方式创建钱包后一定要进行二次验证，例如重新在钱包中导入助记词，并使用passphrase方式导入钱包查看是否提示钱包已存在；或者删除创建的新钱包后重新导入并核对创建和后导入地址的一致性。</mark>

### <mark style="color:orange;">Passphrase使用教程</mark> <a href="#wli5l" id="wli5l"></a>

#### **使用Passphrase方式创建钱包**

1、打开2.1.1版本的TP Wallet，点击右上角第一个图标【新增钱包】，随意选择了以太坊公链做演示。

<figure><img src="../../.gitbook/assets/1 (8).png" alt=""><figcaption></figcaption></figure>

2、因为是首次使用Passphrase功能，所以需要【创建钱包】。需要说明的是TP Wallet使用了全局统一密码，也就是说如果你创建过一个钱包后，那么后续的钱包地址的密码都会和第一个相同。

<figure><img src="../../.gitbook/assets/2 (14).png" alt=""><figcaption></figcaption></figure>

3、Passphrase带来的变化就是在界面底部多了【高级设置】，打开后可以设置Passphrase，请认真查看Passphrase的介绍内容，熟悉它的特点和注意事项。

<figure><img src="../../.gitbook/assets/3 (4).png" alt=""><figcaption></figcaption></figure>

4、备份和验证助记词的界面不再演示。创建好钱包后，点击【收款】在这里可以看到通过Passphrase方式创建的钱包地址。

<figure><img src="../../.gitbook/assets/4 (6).png" alt=""><figcaption></figcaption></figure>

#### **使用Passphrase方式导入钱包**

在这个演示中，我们会使用普通的助记词导入方式和使用Passphrase方式导入助记词到钱包做一个比对。

1、默认助记词导入，和日常的导入方式一样，填入助记词后直接点击【确定导入】，导入后查看钱包地址如下图。

<figure><img src="../../.gitbook/assets/5 (18).png" alt=""><figcaption></figcaption></figure>

2、在导入助记词界面中点击【高级模式】，即可看到Passphrase的设置界面，输入正确的内容后点击【确定导入】。这时查看钱包收款地址和开始使用Passphrase方式创建钱包的地址相同。（使用错误的Passphrase内容导入钱包会得到不同的地址）

<figure><img src="../../.gitbook/assets/6 (6).png" alt=""><figcaption></figcaption></figure>
