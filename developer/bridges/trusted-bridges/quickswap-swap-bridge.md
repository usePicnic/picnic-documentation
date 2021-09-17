---
description: "\U0001F44B Welcome to Pods' docs. This documentation aims to provide a high-level overview of the protocol and its existing components."
---

# QuickswapSwapBridge

Inherits from [IUniswapV2Swap](https://docs.indexpool.org/developer/bridges/interfaces/iuniswapv2swap). See code on [github](https://github.com/indexpool/indexpool-contracts/blob/main/contracts/bridges/trusted/QuickswapSwapBridge/QuickswapSwapBridge.sol).

## SwapTokenToToken

Swaps from ERC20 token to ERC20 token.

| Input Name | Description |
| :--- | :--- |
| amountInPercentage | Percentage of the balance of the input ERC20 token that will be swapped |
| amountOutMin | Minimum amount of the output token required to execute swap |
| path | The swap route determined by the path. The first element of path is the input token, the last is the output token, and any intermediate elements represent intermediate pairs to trade through \(if, for example, a direct pair does not exist\). |

```javascript
function swapTokenToToken(
        uint256 amountInPercentage,
        uint256 amountOutMin,
        address[] calldata path
    ) external;
```

