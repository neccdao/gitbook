---
description: Decentralised Interest Bearing Perpetual Swap Protocol
---

# Overview

## Introduction

Necc is a yield-bearing, fully collateralised stablecoin protocol. These properties are achieved by creating delta neutral positions on whitelisted collaterals. Deposited collateral is lent out to long and short traders to create up to 50x leveraged positions. Fees from trading and liquidations accrue to the stablecoin minters via a second token, NECC.&#x20;

NECC can also be vested by selling NAKA or NAKA/NECC LP tokens to the Treasury.

The stablecoin, NAKA, can be minted by depositing a whitelisted collateral. This stablecoin is minted 1-1 to the collateral's USD value, per its associated Chainlink price feed. NAKA can be burned for any whitelisted collateral type at a rate of `(collateral in pool) / (supply of NAKA).`

Traders looking to open leveraged positions can "borrow", or more accurately, trade against the collateral pool, with up to 50x leverage. A trader can deposit 1 ETH, then borrow 1 more ETH, for a total position size of 2 ETH.

NAKA retains its value against trading by seizing the long and short traders' collateral when price volatility occurs, and by natural price appreciation when prices rise.

### Walkthrough

**The price of ETH is $2000 USD**

* Alice, a risk-averse hodler, mints 2000 NAKA with 1 ETH. She also receives Necc tokens for staking NAKA. The 1 ETH is sent to the collateral pool.
* Bob, a risk-on trader, opens a 2X ETH long by depositing 1 ETH, and "borrowing" 1 ETH from the pool

**ETH price increases 10% to $2200**

* Bob closes his position. He is able to withdraw $2400 worth of ETH, or \~1.1 ETH
* The pool now has \~0.9 ETH, worth $2000
* Alice can redeem her 2000 NAKA for 0.9 ETH, and her NECC for staking NAKA

**ETH price decreases 10% to $1800**

* Bob closes his position. He is able to withdraw $1600 worth of ETH, or \~0.9 ETH
* The pool now has \~1.1 ETH, worth $2000
* Alice can redeem her 2000 NAKA for 1.1 ETH, and her NECC for staking NAKA

**ETH price decreases by 50% to $1000**

* Bob's position is liquidated
* The pool now has 2 ETH, worth $2000
* Alice can redeem her 2000 NAKA for 2 ETH, and her NECC for staking NAKA
