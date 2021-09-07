# AutofarmAddressToPoolId

The purpose of this contract is to enable `AutofarmDepositBridge` to comply with the `IStake` interface. This happens because the Autofarm contract requires a poolId, that is not easily mapped to an ERC20 address, so we had to create the mapping ourselves.

## GetPoolId

Returns an Autofarm `poolId` based on an input ERC20 token address.

| Input Name | Description |
| :--- | :--- |
| asset | Address of the asset to check for pool Id in Autofarm |

```javascript
    function getPoolId(address asset) external returns (uint256);
```

