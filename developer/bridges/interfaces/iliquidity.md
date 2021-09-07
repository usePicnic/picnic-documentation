# ILiquidity

## Functions

### AddLiquidity

Deposits ERC20 tokens into a liquidity pool protocol.

| Input Name | Description |
| :--- | :--- |
| tokens | List of n - token that will have liquidity added to pool |
| percentages | List of n - percentages of the balance of ERC20 tokens that will be added to the poolminAmounts \(100000 = 100%\) |
| minAmounts | List of n - minimum amounts of the ERC20 tokens required to add liquidity |

```javascript
 function addLiquidity(
        address[] calldata tokens,
        uint256[] calldata percentages,
        uint256[] calldata minAmounts
    ) external;
```

### AddLiquidityETH

Deposits ERC20 token\(s\) and ETH \(Matic\) into a liquidity pool protocol. _Please note that function is not payable but it uses the Wallet ETH balance for the swap._

| Input Name | Description |
| :--- | :--- |
| ethPercentage | Percentage of the balance of input ETH \(Matic\) that will be added to liquidity pool |
| minAmountEth | Minimum amount of the input token required to add liquidity |
| tokens | List of n - token that will have liquidity added alongside ETH \(Matic\) |
| percentages | List of n - percentage of the balance of the ERC20 token that will be added to pool |
| minAmounts | List of n - minimum amount of the ERC20 token required to add liquidity |

```javascript
function addLiquidityETH(
        uint256 ethPercentage,
        uint256 minAmountEth,
        address[] calldata tokens,
        uint256[] calldata percentages,
        uint256[] calldata minAmounts
    ) external;
```

## Events



