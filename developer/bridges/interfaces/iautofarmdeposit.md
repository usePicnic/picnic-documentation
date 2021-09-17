# IAutofarmDeposit

## Deposit

Deposits a ERC20 token into the Autofarm protocol.

| Input Name | Description |
| :--- | :--- |
| poolId | Autofarm pool id |
| percentageIn | Percentage of the balance of the asset that will be deposited  \(100000 = 100%\) |

```javascript
function deposit(uint256 poolId, uint256 percentage) external;
```

## Withdraw

Withdraws from the Autofarm protocol.

| Input Name | Description |
| :--- | :--- |
| poolId | Autofarm pool id |
| percentageOut | Percentage of the balance of the asset to be withdrawn \(100000 = 100%\) |

```javascript
function withdraw(uint256 poolId, uint256 percentageOut) external;
```

