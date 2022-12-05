# 警惕精准伪装地址



在之前介绍的盗币方式中，盗币者一般会采用一些技术手段来开发恶意的链接来想办法诱导用户进行执行授权，从而盗取授权过的这个代币。这种方式的实施范围比较广泛。

近期TokenPocket技术团队发现了一种**新型的盗币方式（“精准伪装”）**。

这种方式从根本上来说是用了比较“原始”的方法执行，例如在链上观察到一个钱包地址经常会有大资金的usdt往来记录，那么就对这个钱包进行监控，找到其经常收款的地址，利用“靓号生成器”生成和收款地址非常相似的地址（一般是前几位，或者后几位基本一样），**多次的转入小额的数量到监控的这个钱包地址中（例如0.001USDT)**。用户在进行转账时，可能会复制之前的转账收款记录的转账地址来进行重新转账，如果这个时候复制到了错误的（高度相似）地址，那么就会导致转账发生错误，从而导致了代币的丢失。

<div>

<figure><img src="data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%27512%27%20height=%27455%27/%3e" alt=""><figcaption></figcaption></figure>

 

<figure><img src="https://mirror.xyz/_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2FWcGAivxKGTPGhbT6rtFBH.png&#x26;w=1080&#x26;q=90" alt=""><figcaption></figcaption></figure>

</div>

> _**建议经常有的资金往来业务的用户，在转账的时候核对好收款地址，对收款地址做一个完整的验证；其次，使用钱包地址簿转账的功能，将日常使用的钱包地址在通讯录中收录，转账时直接选择地址即可。**_

### 如何使用TokenPocket地址簿功能？

打开TokenPocket，点击【转账】--【地址簿转账】。

<div>

<figure><img src="data:image/svg+xml,%3csvg%20xmlns=%27http://www.w3.org/2000/svg%27%20version=%271.1%27%20width=%271280%27%20height=%271137%27/%3e" alt=""><figcaption></figcaption></figure>

 

<figure><img src="https://mirror.xyz/_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2FC4ILm5TGUphFnOaKqR6Uu.png&#x26;w=3840&#x26;q=90" alt=""><figcaption></figcaption></figure>

</div>
