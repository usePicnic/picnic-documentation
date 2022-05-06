# AaveV2DepositBridge

Inherits from [IAaveV2Deposit](https://docs.indexpool.org/developer/bridges/interfaces/iaavev2deposit). See code on [github](https://github.com/indexpool/indexpool-contracts/blob/main/contracts/bridges/trusted/AaveV2DepositBridge/AaveV2DepositBridge.sol).

## Deposit

Deposits a ERC20 token into the Aave protocol.

| **Input Name** | **Description**                                                                |
| -------------- | ------------------------------------------------------------------------------ |
| assetIn        | Address of the asset to be deposit into the Aave protocol (DAI, WETH, WBTC...) |
| percentageIn   | Percentage of the balance of the asset that will be deposited  (100000 = 100%) |

```javascript
function deposit(address assetIn, uint256 percentage) external;
```

## Withdraw

Withdraws from the Aave protocol.

| **Input Name** | **Description**                                                                  |
| -------------- | -------------------------------------------------------------------------------- |
| assetOut       | Address of the asset to be withdrawn from the Aave protocol (DAI, WETH, WBTC...) |
| percentageOut  | Percentage of the balance of the asset to be withdrawn (100000 = 100%)           |

```javascript
function withdraw(address assetOut, uint256 percentageOut) external;
```
