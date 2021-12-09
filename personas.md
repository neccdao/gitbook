---
description: Different actors and their roles within the Necc protocol
---

# Personas

Necc protocol was created to appeal to multiple actors getting them to collaborate irrespective of their self motives. Understanding that there will be winners and losers as liquidity and market conditions change, the long term goal of the protocol is to keep increasing TVL and sustain capital efficiency.

Below are illustrations of how the different personas can be winners and losers whilst interacting with Necc protocol:

#### Minters

- Risk off stablecoin minters can get a good mint rate by looking at the current weightings backing the NDOL stablecoin, they can attain <= 0.3% mint fee based on the collateral they mint with. In return for the lower mint rate, they help rebalance the multiple collateral redemption ratios to aid stablecoin pricing.
- Compared to other protocols, NDOL is an interest bearing stablecoin with deep redemption liquidity. Liquidity becomes sticky via weighted mint fees and staking the stablecoin for NECC yield tokens as 1% of vested NECC is available to claim by NDOL stakers.
- NDOL and NDOL/nNECC LP can be used as principal for vested NECC which in turn can be staked for a higher NECC APY. Instead of potentially causing an imbalance in the collateral pools that back NDOL by burning it, NDOL can be sold to the Treasury to lock liquidity in for borrowers.
- Stablecoin minters can redeem/burn NDOL at a fixed rate of 0.3% burn fees with zero price slippage. This shifts debt between the collateral pools.
- Traders reserve a portion of the inverse pool for the duration of their open position so NDOL burners may not redeem as much collateral as they would like based on liquidity pool depth.
- NDOL burners face price risk as collateral may go up in price so they can redeem less.
- Traders can close high utilisation inverse perpetual short positions locking in a chunk of the collateral pool as profit although it is expected more liquidity is returned to the pools as long positions get liquidated if collateral price goes does.
- NDOL minters take on cash and carry trades in its nature with fee income derived from funding, swap and vesting rates.

#### Traders

- Decentralised inverse perpetuals are available based on counterparty liquidity contributed by NDOL stablecoin minters. This means that the open interest is capped by how much liquidity is available per collateral pool.
- Debt swaps can be made before opening an inverse perpetual position, this means WBTC collateral can be used to open an ETH long or short for example.
- Funding rates are essentially borrow rates based on collateral pool utilisation rates rather than longs or shorts paying each other. This is due to pure inverse perpetuals regardless of direction bias and zero slippage or synthetic mark price.&#x20;
- Flux oracles have limited price feeds per blockchain limiting the amount of potential whitelisted collaterals.
- Linear perpetual contracts require spot holdings to be sold off to top up USD based collateral margin, you are effectively having a 1x short open with negative funding rate whilst having a linear long position open. Rollover for margin top up exponentially increases in costs with spot swap fees as collateral spot price goes up.
- Inverse perpetuals allow positive convexity regardless of direction bias; bullish shorting.
- Payouts in the speculated index token as realised profit gives fundamental trade expression as a benefit of DeFi. Bullish on ETH, you use spot collateral to long ETH and gain even more ETH.
- Inverse perpetuals are existential in terms of underlying collateral fixed supply caps, there is only so much Bitcoin that can go around for your PnL.
- Inverse perpetuals increasing in open interest are expressive but can correlate with sudden liquidation cascades.

#### Degenerates

- Early principal vesters and NECC stakers lock in crucial liquidity for the Necc protocol to grow therefore their APY is higher in return.
- Degenerates can attain the lowest NECC vesting cost by minting NDOL from the lowest current weighted collateral to get lower minting fees.
- Degenerates can arbitrage vesting discounts against AMM secondary markets.
- Degenerates can sell NDOL/nNECC LP token for further vested NECC yield tokens in return for increasing protocol owned liquidity.
- Necc protocol yield accrues via trading fees and swap fees within the collateral pools, degenerates get the highest APY as they speculate on future protocol income.
- Degenerates have governable say in protocol income streams, partnerships, products and newer markets.
- Degenerates bet on (3,3) and long term price stabilisation.
- Market wide price drops can affect degenerates the most if they are not faithful and necc. Mainly due to volatile assets within collateral pools with imbalance and utilisation by borrowers and burners.&#x20;
- Degenerates are bound by Treasury risk free value.&#x20;

\---

> _Now I lay me down to sleep,_
>
> _I pray the Lord my Sats to keep,_
>
> _If I should die before I ‘wake,_
>
> _I pray the Lord my Key to take._
>
> \~ Arthur Hayes

Recommended reading to understand the foundational ideas of Necc protocol from the bull God Arthur Hayes:

- [https://cryptohayes.medium.com/all-aboard-4d50435190d6](https://cryptohayes.medium.com/all-aboard-4d50435190d6)
- [https://blog.bitmex.com/stablecoins-sophistry-at-its-best/](https://blog.bitmex.com/stablecoins-sophistry-at-its-best/)
- [https://blog.bitmex.com/convexity-rektum-damn-near-killed-em/](https://blog.bitmex.com/convexity-rektum-damn-near-killed-em/)
- [https://blog.bitmex.com/cash-and-carry-arbitrage-with-bitmex-futures/](https://blog.bitmex.com/cash-and-carry-arbitrage-with-bitmex-futures/)
- [https://cryptohayes.medium.com/yes-i-read-the-whitepaper-59cfa2ea9c2c](https://cryptohayes.medium.com/yes-i-read-the-whitepaper-59cfa2ea9c2c)
- **[_https://blog.bitmex.com/all-ye-faithful/_](https://blog.bitmex.com/all-ye-faithful/)**
