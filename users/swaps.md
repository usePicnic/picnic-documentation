# Swaps

## How swaps are made?

Currently all swaps `(ERC20 -> ERC20)` are done on QuickSwap using `WMATIC`, `USDC`, `USDT`, `WETH` and `QUICK` as possible intermediaries for the routes. Route selection is based on whichever path is more liquid.

## How swaps will be made?

We will soon add routing using the QuickSwap SDK and for Q1 of 2022 we will add a smart routing feature, using a service like 1inch choosing the optimal route accross DEXes.

