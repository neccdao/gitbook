---
description: Vault collateral pools weight ratios
---

# Rebalance mechanisms

Whilst isolated collateral pools have individual redemption ratios to ensure multiple pegs of the NAKA price, the protocol understands that each collateral has different properties.

Whitelisted collateral therefore have target weight ratios backing the NAKA \~$1 price.

Whitelisted collateral is assessed by multiple properties being:

* Market cap
* Annual projected volatility
* Staking ratios
* Systemic risk
* Smart contract risk
* Ecosystem utilisation
* Trading volume to market cap ratio
* Oracle data feed sources
* General price action

\---

By assigning each whitelisted collateral a target weighting within the system, we can ensure its distance away from that target weight is incentivised.

Below is the minting equation to incentivise target weighting:

```mathml
0.3% standard mint fee * 
( Current collateral pool NAKA supply / 
(Total NAKA supply * Target weight := 0 to 1) )

0.3% * (1000 collateral pool NAKA / (4000 total NAKA * 0.6))
=== 0.3% * 0.416 = 0.125% mint fee for that collateral
```

\---

Inverse perpetual trading fees help maintain Vault collateral pool ratios via weekly NAKA minting and NECC vesting.

Trading fees are swapped via AMM and NAKA is minted towards those collateral pool target ratios.

That NAKA is then vested for NECC tokens effectively redistributing trading fees as NECC yield tokens to sustain staking APY.
