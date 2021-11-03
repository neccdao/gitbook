---
description: Yield and governance token
---

# Necc

By supplying collateral to the protocol to be borrowed for leveraged positions, Necc is distributed in return according to the collateral demand and liquidity weights.

Necc can be redeemed for a portion of the basket of collaterals that are accumulated as fees for using the Necc protocol as described in [Fees](fees.md).

Necc could also be swapped on a secondary market like an AMM that should target the total underlying collateral basket price.

**Distributing Necc:**&#x20;

Total supplied collateral in USD = $10M&#x20;

\- ETH - 10% ($1M)

\- MKR - 20% ($2M)&#x20;

\- LINK - 70% ($7M)

**TBD weighted distribution**

`(Percentage of user nUSD minted for supplied collateral type * Weighted percentage of supplied collateral of total) * Percentage of Necc block emissions/rewards`

User puts in $10k USD worth of LINK, gets 10k Necc

User puts in $10k USD worth of ETH, gets 30k Necc

**Redeeming Necc:**&#x20;

Total rewards pool:&#x20;

\- $1M ETH&#x20;

\- $1M LINK&#x20;

\- $1M MKR&#x20;

User redeems 10k Necc (10% of total), receives $300k total (10% of USD value).

**Decisions to make**&#x20;

\- What are the collateral weights? FTX?&#x20;

\- How much more should you get for choosing the small collateral vs. the large&#x20;

\- How many tokens do you get per USD of collateral?&#x20;

%age share of total collateral supplied in USD?

* Funding rates affecting the Necc distribution?

\- How do we incentivise longs/shorts?&#x20;

* Should governance be another token given in return for staking Necc?
* Do we want another token index weighted farming Necc or a zap vault?&#x20;
