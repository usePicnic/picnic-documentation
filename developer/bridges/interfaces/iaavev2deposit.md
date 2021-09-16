# IAaveV2Deposit

## Deposit

Deposits a ERC20 token into the protocol.

| Input Name | Description |
| :--- | :--- |
| assetIn | Address of the asset to be deposited |
| percentageIn | Percentage of the balance of the asset that will be deposited  \(100000 = 100%\) |

```javascript
function deposit(address assetIn, uint256 percentage) external;
```

## Harvest

Claim rewards from the protocol.

| Input Name | Description |
| :--- | :--- |
| asset | Address of the asset that will be harvested |

```javascript
function harvest(address asset) external;
```

## Withdraw

Withdraws from the protocol.

| Input Name | Description |
| :--- | :--- |
| assetOut | Address of the asset to be withdrawn |
| percentageOut | Percentage of the balance of the asset to be withdrawn \(100000 = 100%\) |

```javascript
function withdraw(address assetOut, uint256 percentageOut) external;
```



