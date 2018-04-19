# web3j-example

Web3j web3 = Web3j.build(new HttpService("network address"));// 创建Web3J

Credentials credentials = WalletUtils.loadCredentials("123456", "wallet file");// 加载钱包

Daibi_sol_TokenERC20 keySCode = Daibi_sol_TokenERC20.load("合约地址",web3, credentials, BigInteger.valueOf(27000000000L), BigInteger.valueOf(210000));// 加载合约

TransactionReceipt receipt = keySCode.transfer("account address", BigInteger.valueOf(代币数量*10^小数点位数)).send();//转账
