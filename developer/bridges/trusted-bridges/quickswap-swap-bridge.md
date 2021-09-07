---
description: "\U0001F44B Welcome to Pods' docs. This documentation aims to provide a high-level overview of the protocol and its existing components."
---

# QuickswapSwapBridge

## FromETHToToken

Swaps from ERC20 token to ERC20 token. _Please note that function is not payable but it uses the Wallet ETH balance for the swap._

| Input Name | Description |
| :--- | :--- |
| amountInPercentage | Percentage of the balance of input ETH \(Matic\) that will be swapped |
| amountOutMin | Minimum amount of the output token required to execute swap |
| path | The swap route determined by the path. The first element of path is the input token, the last is the output token, and any intermediate elements represent intermediate pairs to trade through \(if, for example, a direct pair does not exist\). |

```javascript
function tradeFromETHToToken(
        uint256 amountInPercentage,
        uint256 amountOutMin,
        address[] calldata path
    ) external;
```

## FromTokenToETH

Swaps from ERC20 token to ETH \(Matic\).

| Input Name | Description |
| :--- | :--- |
| amountInPercentage | Percentage of the balance of the input ERC20 token that will be swapped |
| amountOutMin | Minimum amount of output ETH \(Matic\) required to execute swap |
| path | The swap route determined by the path. The first element of path is the input token, the last is the output token, and any intermediate elements represent intermediate pairs to trade through \(if, for example, a direct pair does not exist\). |

```javascript
function tradeFromTokenToETH(
        uint256 amountInPercentage,
        uint256 amountOutMin,
        address[] calldata path
    ) external;
```

## FromTokenToToken

Swaps from ERC20 token to ERC20 token.

| Input Name | Description |
| :--- | :--- |
| amountInPercentage | Percentage of the balance of the input ERC20 token that will be swapped |
| amountOutMin | Minimum amount of the output token required to execute swap |
| path | The swap route determined by the path. The first element of path is the input token, the last is the output token, and any intermediate elements represent intermediate pairs to trade through \(if, for example, a direct pair does not exist\). |

```javascript
function tradeFromTokenToToken(
        uint256 amountInPercentage,
        uint256 amountOutMin,
        address[] calldata path
    ) external;
```

