ETH Hangzhou Hackathon Project

## WeiWallet基于权重值的多签合约钱包

本项目合约主要分为工厂合约和多签权重值合约。

### MultiSignatureFactory工厂合约

本合约的主要功能是：
1. 创建权重值类型的多签钱包。
2. 根据创建合约钱包所需要的salt值预测出部署的多签合约钱包地址。
3. 获取创建成功后的多签钱包的创建时间和salt值。
4. 分页获取指定用户的创建过的多签列表。

### MultiSignatureWeight权重值钱包合约

该合约先部署为逻辑合约，然后工厂合约创建出来的新钱包合约。

该合约的功能有：
1. 维护一个nonce值，用来记录当前多签合约执行多少笔交易，并且防止签名被复用。
2. 读取当前多签钱包中成员的数量。
3. 读取指定成员的权重值。
4. 读取当前的权重门限值，即达到多少权重执行交易。
5. 判断指定地址是否是多签钱包成员。
6. 获取多签钱包所有成员地址。
7. 添加成员并修改各个成员的权重值。
8. 移除成员并修改各个成员的权重值。
9. 替换成员。
10. 修改各个成员的权重值。
11. 修改权重门限值。
12. 转账交易。
13. 调用合约交易。
14. 取消交易。




# ETH-HangZhou-Hackathon-WeiWallet
