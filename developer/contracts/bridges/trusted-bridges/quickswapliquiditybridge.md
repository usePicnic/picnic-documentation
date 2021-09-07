# QuickswapLiquidityBridge

## AddLiquidity

Deposits a ERC20 token into the Autofarm protocol.

| Input Name | Description |
| :--- | :--- |
| tokens | List of two - token that will have liquidity added to pool |
| percentages | List of two - percentages of the balance of ERC20 tokens that will be added to the poolminAmounts \(100000 = 100%\) |
| minAmounts | List of two - minimum amounts of the ERC20 tokens required to add liquidity |

```javascript
 function addLiquidity(
        address[] calldata tokens,
        uint256[] calldata percentages,
        uint256[] calldata minAmounts
    ) external;
```

## AddLiquidityETH

Claim rewards from the Autofarm protocol.

| Input Name | Description |
| :--- | :--- |
| ethPercentage | Percentage of the balance of input ETH \(Matic\) that will be added to liquidity pool |
| minAmountEth | Minimum amount of the input token required to add liquidity |
| tokens | List of one - token that will have liquidity added alongside ETH \(Matic\) |
| percentages | List of one - percentage of the balance of the ERC20 token that will be added to pool |
| minAmounts | List of one - minimum amount of the ERC20 token required to add liquidity |

```javascript
function addLiquidityETH(
        uint256 ethPercentage,
        uint256 minAmountEth,
        address[] calldata tokens,
        uint256[] calldata percentages,
        uint256[] calldata minAmounts
    ) external;
```

