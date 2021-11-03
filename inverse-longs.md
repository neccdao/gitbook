---
description: Compound those profits on the way up mate
---

# Inverse Longs

Necc inverse longs give a profit payout in a non-stablecoin volatile token.\
ETH, WBTC etc.

Stablecoins can still be used as collateral to open inverse longs but the payout will be in the non-stablecoin volatile token.

Funding rates are dynamic percentages that open positions will have to pay or get paid every 8 hours based on collateral utilisation rates with the aim to rebalance price following volatile periods towards the index price.

\---

Below is an illustration of how the Necc protocol can be used for inverse leverage longs and rough amounts of payments:

1. The Price of ETH is 1000 USD
2. Alice mints 1000 Necc by supplying 1 ETH to the system
3. The system now has 1 ETH that is borrowable for an inverse long position
4. Bob deposits 1 ETH and opens a 2X ETH long position
5. The system now has 2 ETH
6. The price of ETH goes up 100 USD, it is now 1100 USD each
7. The system now has 2200 USD worth of ETH
8. Bob can be paid 1200 USD worth of ETH
9. Alice can be 1000 USD worth of ETH

In addition to funding rates, Necc yield tokens are** **distributed to Bob for his 2X ETH long position.
