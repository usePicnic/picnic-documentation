# Interfaces

Bridges interfaces are solidity [Interfaces](https://docs.soliditylang.org/en/latest/contracts.html?highlight=Interfaces#interfaces) that standardize IndexPool bridges according to their purpose. 

1. Bridges inherit from interfaces.
2. Interfaces have events that have to be used to have a consistent UI / UX for our users.

Current interfaces and its purposes are given below:

| Interface | For bridges implementing... | Bridge examples |
| :--- | :--- | :--- |
| IAaveV2Deposit | Aave deposit/withdraw/harvest | [AaveV2DepositBridge](https://docs.indexpool.org/developer/bridges/trusted-bridges/aave-v2-deposit-bridge) |
| IAutofarmDeposit | Autofarm deposit/withdraw/harvest | [AutofarmDepositBridge](https://docs.indexpool.org/developer/bridges/trusted-bridges/autofarm-deposit-bridge) |
| IUniswapV2LiquidityA | Add/remove liquidity from UniswapV2 | [QuickswapLiquidityBridge](https://docs.indexpool.org/developer/bridges/trusted-bridges/quickswap-liquidity-bridge) |
| IUniswapV2Swap | Swapping ERC20 tokens with Uniswap V2 | [QuickswapSwapBridge](https://docs.indexpool.org/developer/bridges/trusted-bridges/quickswap-swap-bridge) |
| IWMaticWrap | Wrapping / Unwrapping MATIC  | WMaticWrapBridge |



