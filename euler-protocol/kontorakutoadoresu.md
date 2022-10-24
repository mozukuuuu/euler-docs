# コントラクトアドレス

## アドレス

Eulerの他に、スマートコントラクトは、EULトークン所有者が管理するGovernanceを介してアップグレード可能です（つまり、実装コントラクトは定期的にアップグレードされます）。したがって、コントラクトのやり取りには、プロキシスマートコントラクトのアドレスを使用してください。

例えば、 [web3.js](https://web3js.readthedocs.io/en/v1.2.11/web3-eth-contract.html) を使って Markets の契約とやり取りする場合、Markets の契約 ABI を使用しますが、Markets の契約プロキシのアドレスをターゲット契約として設定します。

```javascript
const markets = new Contract(MarketsABI, Markets_Proxy_Address); // proxy address
```

### ネットワーク

現在、Eulerプロトコルは以下のネットワークに展開されています。

#### Mainnet

| Contract    | Proxy Address                              | Etherscan (Proxy)                                                                    | Etherscan (Implementation)                                                           | Source Code                                                                                          |
| ----------- | ------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------- |
| Euler       | 0x27182842E098f60e3D576794A5bFFb0777E025d3 |                                                                                      | [Etherscan](https://etherscan.io/address/0x27182842E098f60e3D576794A5bFFb0777E025d3) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/Euler.sol)               |
| Markets     | 0x3520d5a913427E6F0D6A83E07ccD4A4da316e4d3 | [Etherscan](https://etherscan.io/address/0x3520d5a913427E6F0D6A83E07ccD4A4da316e4d3) | [Etherscan](https://etherscan.io/address/0xE5d0A7A3ad358792Ba037cB6eE375FfDe7Ba2Cd1) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/Markets.sol)     |
| Liquidation | 0xf43ce1d09050BAfd6980dD43Cde2aB9F18C85b34 | [Etherscan](https://etherscan.io/address/0xf43ce1d09050BAfd6980dD43Cde2aB9F18C85b34) | [Etherscan](https://etherscan.io/address/0xAed37a234cc880a9e3D9Fd9022013eE0A419493e) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/Liquidation.sol) |
| Exec        | 0x59828FdF7ee634AaaD3f58B19fDBa3b03E2D9d80 | [Etherscan](https://etherscan.io/address/0x59828FdF7ee634AaaD3f58B19fDBa3b03E2D9d80) | [Etherscan](https://etherscan.io/address/0x14cBaC4eC5673DEFD3968693ebA994F07F8436D2) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/Exec.sol)        |
| Swap        | 0x7123C8cBBD76c5C7fCC9f7150f23179bec0bA341 | [Etherscan](https://etherscan.io/address/0x7123C8cBBD76c5C7fCC9f7150f23179bec0bA341) | [Etherscan](https://etherscan.io/address/0xf40e8314143B4CF1764CCCd22588a8794a00d8Ca) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/Swap.sol)        |
| SwapHub     | 0x542ACC8E1db037d6008587aBfB1B7fB44014c629 | [Etherscan](https://etherscan.io/address/0x7123C8cBBD76c5C7fCC9f7150f23179bec0bA341) | [Etherscan](https://etherscan.io/address/0x542ACC8E1db037d6008587aBfB1B7fB44014c629) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/SwapHub.sol)     |
| Governance  | 0xAF68CFba29D0e15490236A5631cA9497e035CD39 | [Etherscan](https://etherscan.io/address/0xAF68CFba29D0e15490236A5631cA9497e035CD39) | [Etherscan](https://etherscan.io/address/0x554ee3d9ed7E9ec21E186c7dd636430669812f73) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/Governance.sol)  |

#### Goerli

| Contract           | Proxy Address                              | Etherscan (Proxy)                                                                           | Etherscan (Implementation)                                                                  | Source Code                                                                                                                    |
| ------------------ | ------------------------------------------ | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| Euler              | 0x931172BB95549d0f29e10ae2D079ABA3C63318B3 |                                                                                             | [Etherscan](https://goerli.etherscan.io/address/0x931172BB95549d0f29e10ae2D079ABA3C63318B3) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/Euler.sol)                                         |
| Markets            | 0x3EbC39b84B1F856fAFE9803A9e1Eae7Da016Da36 | [Etherscan](https://goerli.etherscan.io/address/0x3EbC39b84B1F856fAFE9803A9e1Eae7Da016Da36) | [Etherscan](https://goerli.etherscan.io/address/0xeE28839fde1e462C8e0b80DE618cB98dB3c017F8) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/Markets.sol)                               |
| Liquidation        | 0x66326c072283feE63E1C3feF9BD024F8697EC1BB | [Etherscan](https://goerli.etherscan.io/address/0x66326c072283feE63E1C3feF9BD024F8697EC1BB) | [Etherscan](https://goerli.etherscan.io/address/0x849f5CC81d12887BC0e4e42D8C87AbA896bDCAC0) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/Liquidation.sol)                           |
| Exec               | 0x4b62EB6797526491eEf6eF36D3B9960E5d66C394 | [Etherscan](https://goerli.etherscan.io/address/0x4b62EB6797526491eEf6eF36D3B9960E5d66C394) | [Etherscan](https://goerli.etherscan.io/address/0x6C933044542d6cAF8927E516B9A99632697bD4C0) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/Exec.sol)                                  |
| Swap               | 0xA0AAb1Ddd165cE80AE2b9bC9bBE3b6EEFBB2300c | [Etherscan](https://goerli.etherscan.io/address/0xA0AAb1Ddd165cE80AE2b9bC9bBE3b6EEFBB2300c) | [Etherscan](https://goerli.etherscan.io/address/0x034FCa46b265b4805e00E109A5ABA3E976625B1D) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/Swap.sol)                                  |
| Governance         | 0x496A8344497875D0D805167874f2f938aEa15600 | [Etherscan](https://goerli.etherscan.io/address/0x496A8344497875D0D805167874f2f938aEa15600) | [Etherscan](https://goerli.etherscan.io/address/0xc9314acCF0d3754A38DdE280D24c51D280C33D16) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/master/contracts/modules/Governance.sol)                            |
| ERC20 Token Faucet | 0x1215396CB53774dCE60978d7237F32042cF3a1db |                                                                                             | [Etherscan](https://goerli.etherscan.io/address/0x1215396CB53774dCE60978d7237F32042cF3a1db) | [GitHub](https://github.com/euler-xyz/euler-contracts/blob/smart-contract-deployments/contracts/test/TestERC20TokenFaucet.sol) |

注：_Governanceスマートコントラクトは、現在、リスクガードのローンチ（メインネットローンチのフェーズ1）に使用されており、フェーズ2でコミュニティ主導のガバナンスを構築しています。_
