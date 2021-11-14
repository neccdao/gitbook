---
description: Compound those profits on the way up mate
---

# Inverse Longs and Shorts

Necc protocol inverse perpetuals give a profit payout in the speculated volatile token.\
WETH, WBTC, WNEAR etc.

NDOL Stablecoins can still be used as collateral to open positions but the payout will be in the non-stablecoin volatile token.

Funding rates are dynamic percentages that open positions will have to pay every 8 hours based on the borrowed collateral utilisation rates with the aim to rebalance usage following volatile periods.

\---

Below is an illustration of how the Necc protocol can be used for inverse leverage longs with amounts of payments:

1. The Price of ETH is 1000 USD
2. Alice mints 1000 NDOL by supplying 1 ETH to the system
3. The system now has 1 ETH that is borrowable for an inverse long position
4. Bob deposits 1 ETH and opens a 2X ETH long position
5. The system now has 2 ETH
6. The price of ETH goes up 100 USD, one ETH is now worth 1100 USD each
7. The system now has 2200 USD worth of ETH
8. Bob can be paid 1200 USD worth of ETH
9. Alice can burn 1000 NDOL worth of ETH

In addition to funding rates, Necc yield tokens are** **distributed to Alice for staking her NDOL.

\---

Below is an illustration of how the Necc protocol can be used for inverse leverage shorts with amounts of payments:

1. The Price of ETH is 1000 USD
2. Alice mints 1000 NDOL by supplying 1 ETH to the system
3. Bob mints 2000** **NDOL by supplying 2 ETH** **to the system
4. The system now has 3 ETH
5. Chris supplies 1 ETH and opens a 2x short by borrowing 1 ETH
6. The price of ETH goes down 100 USD, one ETH is now worth 900 USD each
7. The system now has 2700 USD worth of ETH&#x20;
8. Chris can be paid 1.2 ETH
