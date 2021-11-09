---
description: To sustain the ponzi
---

# Fees

These values were calculated to be competitive against cexes and to sustain the NAKA peg and Necc protocol through a bear market.&#x20;

| Event                                                   | Amount                                                                                                 |
| ------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| <p></p><p>Minting NAKA with a volatile token</p><p></p> | 0.3%                                                                                                   |
| Burning NAKA                                            | 0.3%                                                                                                   |
| Swapping Collateral                                     | 0.3%                                                                                                   |
| Opening long/short position                             | 0.1%                                                                                                   |
| Closing long/short position                             | 0.1%                                                                                                   |
| Funding rates on Open position                          | <p>0.06% * (collateral utilisation ratio) every 8 hours</p><p>Theoretical maximum of ~65% annually</p> |
| Liquidation                                             | 5 USD in collateral token to liquidator                                                                |
| Vesting                                                 | <p>20% to DAO</p><p>1% to NAKA stakers</p>                                                             |



These fees are redistributed in the form of NECC tokens to:

* NAKA stakers
* Over collateralise NAKA
* Treasury
* DAO

\---

Trading fees are redistributed weekly by calculating collateral mint amounts and swapping via external AMMs to help rebalance Vault pool ratios.

Basket of trading fees -> AMM swap -> Mint NAKA -> Bond NAKA principal for NECC

\-> Vested NECC redistributed to NAKA and NECC stakers.

