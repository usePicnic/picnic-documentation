# Bridges

## What are bridges?

Bridges are smart contracts that basically wrap a DeFi protocol or an action inside that protocol. For example we have AaveV2DepositBridge, which interacts with Aave's LendingPool in order to make deposits, withdrawals and harvests from the Aave protocol.

Approvals of tokens and other steps necessary to interact with the protocol all happen inside bridges. Bridges are where all protocol specific knowledge resides.

We use it to generate events that are processed so we have all the data we need to build our backend quite easily.

## List of Trusted Bridges

