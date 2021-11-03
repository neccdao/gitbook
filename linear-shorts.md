---
description: We prefer if you take profits near the top
---

# Linear shorts

Necc protocol linear shorts give a profit payout in a stablecoin volatile token.\
USDC, USDT etc.

Non-stablecoins can still be used as collateral to open linear shorts but the user chooses what stablecoin collateral type they will get paid out in. (nUSD payouts are not possible)

Funding rates are dynamic percentages that open positions will have to pay or get paid every 8 hours based on collateral utilisation rates with the aim to rebalance price following volatile periods towards the collateral index price.

\---

Below is an illustration of how the Necc protocol can be used for linear leverage shorts and rough amounts of payments:

1. The Price of ETH is 1000 USD
2. Alice mints 1000 nUSD by supplying 1 ETH to the system
3. The system now has 1 ETH that is borrowable for a linear short position
4. Bob mints 2000** **nUSD by supplying 2000 USDC** **to the system
5. The system now has 1 ETH and 2000 USDC
6. Chris supplies 1 ETH and opens a 2x short by borrowing 1000 USDC
7. The price of ETH goes down 100 USD, it is now 900 USD each
8. The system now has 1800 USD worth of ETH and 1000 USDC&#x20;
9. Alice and Bob can be paid 1800 USD worth of ETH and 800 USDC
10. Chris can be paid 1200 USDC

In addition to funding rates, Necc yield tokens are** **distributed to Bob for his 2X ETH short position.
