---
description: "\U0001F44B Welcome to Pods' docs. This documentation aims to provide a high-level overview of the protocol and its existing components."
---

# Wallet

## UseBridges

This function runs the bridges to interact with other DeFi protocols. These function is extremely sensitive from attacks from malicious bridges, as bridges can access all wallet funds.

| Input Name | Description |
| :--- | :--- |
| bridgeAddresses | Addresses of deployed bridge contractsbridge |
| EncodedCalls | Encoded calls to be passed on to delegate calls |

```javascript
 function useBridges(
        address[] calldata _bridgeAddresses,
        bytes[] calldata _bridgeEncodedCalls
    ) external;
```

## Withdraw

This functions withdraws money from the Wallet to the NFT owner.

| Input Name | Description |
| :--- | :--- |
| outputs | ERC20 token address and percentages that will exit the contract |
| outputEthPercentage | Percentage of ETH in portfolio that will exit the contract |
| nftOwner | NFT owner address |

```javascript
function withdraw(
        IPDataTypes.TokenData calldata outputs,
        uint256 outputEthPercentage,
        address nftOwner
    ) external returns (uint256[] memory, uint256);
```



