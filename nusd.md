---
description: Interest bearing stablecoin
---

# Minting Stablecoin

It is also an index weighting for the underlying basket of collateral.

NDOL keeps track of supplied liquidity for counter party inverse longs and shorts.

NDOL is minted at a rate of 1:1 when whitelisted collateral is supplied to the protocol for borrowing. The supplied collateral price is sourced from its Flux price feed.

Each collateral type also has its isolated own redemption rate:

&#x20;`Collateral in pool / NDOL minted from that collateral`

Meaning the amount of NDOL minted affects the amount of collateral type that can be returned upon burning it.

The amount of collateral returned cannot be greater than the amount of NDOL redeemed in USD dollar amounts.

For this purpose, this cap is to reduce the amount of debt in the system against the collateral supplied over time.

Overall the price for 1 NDOL is:

`Total collateral supplied in USD value / Total NDOL minted`

NDOL can be staked for a portion of the protocol fees distributed in the form of staked NECC tokens as 1% of bond purchases are allocated for NDOL stakers.
