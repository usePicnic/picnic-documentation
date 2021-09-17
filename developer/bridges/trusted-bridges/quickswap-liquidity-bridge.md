# QuickswapLiquidityBridge

Inherits from [IUniswapV2Liquidity](https://docs.indexpool.org/developer/bridges/interfaces/iuniswapv2liquidity). See code on [github](https://github.com/indexpool/indexpool-contracts/blob/main/contracts/bridges/trusted/QuickswapLiquidityBridge/QuickswapLiquidityBridge.sol).

## AddLiquidity

Deposits ERC20 tokens into a liquidity pool protocol.

| Input Name | Description |
| :--- | :--- |
| tokens | List of two - token that will have liquidity added to pool |
| percentages | List of two - percentages of the balance of ERC20 tokens that will be added to the pool \(100000 = 100%\) |
| minAmounts | List of two - minimum amounts of the ERC20 tokens required to add liquidity |

```javascript
 function addLiquidity(
        address[] calldata tokens,
        uint256[] calldata percentages,
        uint256[] calldata minAmounts
    ) external;
```

## RemoveLiquidity

Deposits ERC20 tokens into a liquidity pool protocol.

| Input Name | Description |
| :--- | :--- |
| tokens | List of two - token that will be removed from the pool |
| percentage | Percentage of the balance of the ERC20 LP token that will be converted out of the pool \(100000 = 100%\) |
| minAmounts | List of two - minimum amounts of the ERC20 tokens to succeed in removing liquidity |

```javascript
 function removeLiquidity(
        address[] calldata tokens,
        uint256 calldata percentage,
        uint256[] calldata minAmounts
    ) external;
```

