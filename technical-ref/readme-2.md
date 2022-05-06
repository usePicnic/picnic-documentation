---
description: >-
  This is the interface to use the protocol, it mints NFTs and routes all
  functions call through Wallets and Bridges.
---

# DeFi Basket

## CreatePortfolio

Mints a new NFT and allocates deposited funds to this new NFT. Deposited funds can either be ERC20 tokens or ETH.&#x20;

| **Input Name**     | **Description**                                                |
| ------------------ | -------------------------------------------------------------- |
| inputs             | ERC20 token addresses and amounts that will enter the contract |
| bridgeAddresses    | Addresses of deployed bridge contracts                         |
| bridgeEncodedCalls | Encoded calls to be passed on to delegate calls                |

```javascript
function createPortfolio(
    IPDataTypes.TokenData calldata inputs,
    address[] calldata bridgeAddresses,
    bytes[] calldata bridgeEncodedCalls
) payable external;
```

## DepositPortfolio

Adds more funds into an existing NFT and rearrange allocation inside the portfolio. Deposited funds can either be ERC20 tokens or ETH. _Only the NFT owner can add funds into the NFT._

| **Input Name**     | **Description**                                                |
| ------------------ | -------------------------------------------------------------- |
| nftId              | NFT Id that will have funds deposited into                     |
| inputs             | ERC20 token addresses and amounts that will enter the contract |
| bridgeAddresses    | Addresses of deployed bridge contracts                         |
| bridgeEncodedCalls | Encoded calls to be passed on to delegate calls                |

```javascript
function depositPortfolio(
        uint256 nftId,
        IPDataTypes.TokenData calldata inputs,
        address[] calldata bridgeAddresses,
        bytes[] calldata bridgeEncodedCalls
    ) payable external;
```

## EditPortfolio

Rearrange allocation inside the portfolio. You can't deposit or withdraw funds with this function, just rearrange whatever is inside. _(The bridges would be capable to withdraw funds to accounts different than your own, so be sure to use only trusted bridges)._

| **Input Name**     | **Description**                                 |
| ------------------ | ----------------------------------------------- |
| nftId              | NFT Id that will have funds deposited into      |
| bridgeAddresses    | Addresses of deployed bridge contracts          |
| bridgeEncodedCalls | Encoded calls to be passed on to delegate calls |

```javascript
function editPortfolio(
        uint256 nftId,
        address[] calldata bridgeAddresses,
        bytes[] calldata bridgeEncodedCalls
    ) external;
```

## WithdrawPortfolio

Withdraws funds from the portfolio after rearranging allocation (optional).&#x20;

| **Input Name**      | **Description**                                                             |
| ------------------- | --------------------------------------------------------------------------- |
| nftId               | NFT Id that will have funds deposited into                                  |
| outputs             | ERC20 token address and percentages that will exit the contract             |
| outputEthPercentage | Percentage of ETH in portfolio that will exit the contract  (100000 = 100%) |
| bridgeAddresses     | Addresses of deployed bridge contracts                                      |
| bridgeEncodedCalls  | Encoded calls to be passed on to delegate calls                             |

```javascript
function withdrawPortfolio(
        uint256 nftId,
        IPDataTypes.TokenData calldata outputs,
        uint256 outputEthPercentage,
        address[] calldata bridgeAddresses,
        bytes[] calldata bridgeEncodedCalls
    ) external;
```
