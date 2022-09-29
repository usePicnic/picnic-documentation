# Interfaces

Bridges interfaces are solidity [Interfaces](https://docs.soliditylang.org/en/latest/contracts.html?highlight=Interfaces#interfaces) that standardize Picnic's bridges according to their inputs and outputs. The main use case for this are project forks, but it may be used in case there are protocols that are very similar.

1. Bridges inherit from interfaces.
2. Interfaces have events that have to be used to have a consistent UI / UX for our users.

Current interfaces and its purposes are given below:

| **Interface**                                                                                      | **For bridges implementing...**       | **Bridge examples**                                                                                                 |
| -------------------------------------------------------------------------------------------------- | ------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| [IAaveV2Deposit](https://docs.indexpool.org/developer/bridges/interfaces/iaavev2deposit)           | Aave deposit/withdraw/harvest         | [AaveV2DepositBridge](https://docs.indexpool.org/developer/bridges/trusted-bridges/aave-v2-deposit-bridge)          |
| [IAutofarmDeposit](https://docs.indexpool.org/developer/bridges/interfaces/iautofarmdeposit)       | Autofarm deposit/withdraw/harvest     | [AutofarmDepositBridge](https://docs.indexpool.org/developer/bridges/trusted-bridges/autofarm-deposit-bridge)       |
| [IUniswapV2Liquidity](https://docs.indexpool.org/developer/bridges/interfaces/iuniswapv2liquidity) | Add/remove liquidity from UniswapV2   | [QuickswapLiquidityBridge](https://docs.indexpool.org/developer/bridges/trusted-bridges/quickswap-liquidity-bridge) |
| [IUniswapV2Swap](iuniswapv2swap.md)                                                                | Swapping ERC20 tokens with Uniswap V2 | [QuickswapSwapBridge](https://docs.indexpool.org/developer/bridges/trusted-bridges/quickswap-swap-bridge)           |
| [IWMaticWrap](iwmaticwrap.md)                                                                      | Wrapping / Unwrapping MATIC           | [WMaticWrapBridge](https://docs.indexpool.org/developer/bridges/trusted-bridges/wmaticwrapbridge)                   |

