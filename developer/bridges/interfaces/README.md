# Interfaces

Bridges interfaces are solidity [Interfaces](https://docs.soliditylang.org/en/latest/contracts.html?highlight=Interfaces#interfaces) that standardize IndexPool bridges according to their purpose. 

1. Bridges inherit from interfaces.
2. Interfaces have events that have to be used to have a consistent UI / UX for our users.

Current interfaces and its purposes are given below:

| Interface | For bridges implementing... | Bridge examples |
| :--- | :--- | :--- |
| ISwap | swap operations | QuickswapSwapBridge.sol |
| ILiquidity | add/remove liquidity operations | QuickswapLiquidityBridge.sol |
| IStake | staking operations | AaveV2DepositBridge.sol |
| IWrap | wrapping / unwrapping MATIC | WMaticBridge.sol |
| IFarmPoolId |  |  |



