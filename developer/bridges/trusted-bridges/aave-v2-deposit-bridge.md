---
description: "\U0001F44B Welcome to Pods' docs. This documentation aims to provide a high-level overview of the protocol and its existing components."
---

# AaveV2DepositBridge

## Deposit

Deposits a ERC20 token into the Aave protocol.

| Input Name | Description |
| :--- | :--- |
| assetIn | Address of the asset to be deposit into the Aave protocol \(DAI, WETH, WBTC...\) |
| percentageIn | Percentage of the balance of the asset that will be deposited  \(100000 = 100%\) |

```javascript
function deposit(address assetIn, uint256 percentage) external;
```

## Harvest

Claim rewards from the Aave protocol.

| Input Name | Description |
| :--- | :--- |
| asset | Address of the asset that will be harvested \(DAI, WETH, WBTC...\) |

```javascript
function harvest(address asset) external;
```

## Withdraw

Withdraws from the Aave protocol.

| Input Name | Description |
| :--- | :--- |
| assetOut | Address of the asset to be withdrawn from the Aave protocol \(DAI, WETH, WBTC...\) |
| percentageOut | Percentage of the balance of the asset to be withdrawn \(100000 = 100%\) |

```javascript
function withdraw(address assetOut, uint256 percentageOut) external;
```



