# 我往合约转账了怎么办？

智能合约是由一个地址和该地址对应存储的代码构成的。例如在以太坊上发ERC20的Token，本质上就是创建了一个Token的智能合约，智能合约的代码决定了这个地址里的Token的所有内容。

由于智能合约没有私钥，**一旦转入合约地址，则有可能再也无法转出**。（有些合约预留了可以转走Token的代码，也有坊间认为此举为匿名项目方故意留下的“后门”，存在隐患。）

所以在转账或者交易所提Token时千万不要直接转到该Token的合约地址。

