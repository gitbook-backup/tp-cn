# 什么是权限变更

#### 什么是Aptos私钥（权限）变更

私钥变更，是指账号可以用另一个私钥替换当前私钥，意味着您的账户权限将发生变化，替换成功后对方可以获得当前地址的所有控制权，原私钥将无法再操作该账号。

<mark style="color:red;">**所以遇到此类权限提升提示内容请务必停止授权并关闭当前操作**</mark>，将操作诈骗链接发送给service@tokenpocket.pro 。

### <mark style="color:blue;">**知识延伸：**</mark>

正常情况下，Aptos一个私钥对应一个地址。 例如：私钥A对应地址A，私钥B对应地址B。 假设现在地址A执行了恶意链接，那恶意链接可以把地址A的私钥A变更为私钥B，变更后私钥A就被废弃，无法再操作该账号，所有地址A的交易签名都用私钥B。 对于私钥B来说，除了能给自己的地址B签名，还能给地址A签名，相当于私钥B管理两个地址(钱包)
