# ⚡ Overview

## Intro

DeFi Basket allows you to compose an investment basket with different assets and build it with a single transaction. You may allocate different types of assets, like native tokens, liquidity pools, and virtually any other type of ERC-20 tokens.&#x20;

In this section we'll introduce you to our basic functionalities and characteristics, like cloning, creating, editing and managing a basket. If you want to have a more detailed understanding of how to use our product, please refer to our [How To Use DeFi Basket](broken-reference) section.&#x20;

## Clone a Basket or Create your Own

Our product allows you to create your basket in two different ways:

**Discover and clone a basket**

Through a list of basket already created you're able to find one that matches your expectation regarding possible returns and risk appetite. Once you find and select to clone a basket, you'll then define the deposit asset and DeFi Basket will distribute your funds into the allocation of the selected basket. This generates your own basket, completely separated from the original basket, only mimicking its asset selection and allocation percentages. Your portfolio is under your custody and only you can manage it.&#x20;

**Create your own basket from scratch**

If you already know what and how you want to invest, you may use DeFi Basket to save yourself time and effort to implement your trade with a single transaction. You simply select the assets to perform your allocation, deposit your funds and approve the transaction. Important to notice that the assets listed in our tool are those available on the protocols already integrated (see [below](overview.md#listed-assets) for more details).

## Protocols Integration

Only assets from integrated protocols are available for you to invest in through DeFi Basket. The integration makes assets from selected protocols available for you to build your allocation. The mechanism used for communication between DeFi Basket and the integrated protocol is called [Bridge](../technical-ref/bridges/).&#x20;

We have two different types of integrations:

#### **Token integrations**

Usually refer to protocols where we deposit tokens, usually to earn transaction fees and rewards. These protocols usually give in return tokens that reflect the deposit you made with them.&#x20;

Examples are liquidity pools from Quickswap and liquidity mining vaults from Harvest or Autofarm.

#### **Swap integrations**

These are mostly to allow our mechanism of a single transaction to work. For us to get to the point where we are able to deposit in a liquidity mining protocol like pools at Quickswap or vault at Harvest, we must perform several swaps from your deposit token to the desired allocation tokens.&#x20;

Therefore, you will only be able to select assets listed within DeFi Basket from the protocols that we have already integrated. Soon you will be able to vote and participate in our community to select the next integrations.&#x20;

#### List of Integrated Protocols

As of March 2022, the following protocols have been integrated:&#x20;

* Aave (token)
* Apeswap (swap)
* Autofarm (token)
* Balancer (token & swap)
* Dfyn (swap)
* Harvest (token)
* Jarvis (token & minting)
* Kyberswap (swap)
* Quickswap (swap)
* Uniswap (swap)
