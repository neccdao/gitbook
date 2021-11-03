---
description: Interest bearing stablecoin
---

# nUSD

It is also an index weighting for the underlying basket of collateral.

The point of nUSD is to keep track of supplied liquidity for counter party inverse longs.

nUSD is minted at a rate of 1:1 when white listed collateral is supplied to the Necc protocol for borrowing. The supplied collateral price is sourced from its Chainlink price feed.

Each collateral type also has its isolated own redemption rate.

Meaning the amount of nUSD minted affects the amount of collateral type that can be returned upon redeeming the nUSD.

The isolated collateral type redemption rate is based on:

`Governed redemption ratio := 0.9 * Collateral type amount in the system * (Amount of nUSD to redeem / Total nUSD minted)  `\
`= Amount of collateral returned`

The amount of collateral returned cannot be greater than the amount of nUSD redeemed in USD dollar amounts.

For this purpose, this cap to reduce the amount of debt in the system against the collateral supplied overtime.

Overall the price for 1 nUSD is:

`Total collateral supplied in USD value / Total nUSD minted`

nUSD can be staked for a portion of the protocol fees distributed in the form of [Necc](necc.md) tokens.
