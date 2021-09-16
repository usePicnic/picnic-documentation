---
description: Bridges to DeFi protocols
---

# Bridges

## What are bridges?

Bridges are smart contracts that basically wrap a DeFi protocol or an action inside that protocol. For example we have AaveV2DepositBridge, which interacts with Aave's LendingPool in order to make deposits, withdrawals and harvests from the Aave protocol.

Approvals of tokens and other steps necessary to interact with the protocol all happen inside bridges. Bridges are where all protocol specific rules reside.

We also use bridges to generate events that are processed so we have all the data we need to build our backend easily.

## Why bridges?

Bridges coupled with delegate calls enable us to extend functionality to the IndexPool contract. This means that will be able to integrate with protocols and interfaces that might be very different from the ones we are using now.

This is specially appealing as we can guarantee that if liquidity shifts from one protocol to another, we can still offer a really good user experience, as we can just shift which bridges we are using to route our orders in a way that is most efficient for our users.

## Interfaces

Interfaces are abstract structures that define how bridges should behave depending on the type they belong to.

## Trusted Bridges

These are bridges reviewed by us.

