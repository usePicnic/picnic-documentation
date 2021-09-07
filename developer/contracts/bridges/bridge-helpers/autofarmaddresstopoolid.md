# AutofarmAddressToPoolId

## GetPoolId

Returns an Autofarm `poolId` based on an input ERC20 token address.

| Input Name | Description |
| :--- | :--- |
| asset | Address of the asset to check for pool Id in Autofarm |

```javascript
    function getPoolId(address asset) external returns (uint256);
```

