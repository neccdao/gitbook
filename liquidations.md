---
description: Information on when you need to deposit another 1000 USD
---

# Liquidations

The max leverage is essentially the margin collateral ratio which in other terms means the minimum amount of collateral (percentage) the user has to supply to the protocol to borrow another collateral type up to a certain maximum.

```
If the margin collateral ratio is 5%,
1/0.05 = 20x maximum leverage where 0.05 === 5%.

Or 100/5 = 20x.
```

\---

Partial liquidations are implemented as a primary priority to maintain protocol trader lifetime by reducing position size to its half life at the index price whilst maintaining an open position.

Below is the pseudo code to demonstrate this:

```
        if (!hasProfit) {
            remainingCollateral = position.collateral.sub(delta);
        }

        if (remainingCollateral.mul(MAX_LEVERAGE) <
        position.size.mul(BASIS_POINTS_DIVISOR)) {
            position.size.mul(5).div(10); // divide by 2
        }
```

\---

Below is an illustration of how the Necc protocol can be used to allow a free market for inverse leverage longs _full_ liquidation:

1. The price of ETH is 1000 USD
2. The governed maximum leverage in the system is 2x which means the minimum collateral ratio is 50%
3. Alice mints 1000 nUSD by supplying 1 ETH to the system
4. The system now has 1 ETH that is borrowable for an inverse long position
5. Bob deposits 1 ETH and opens a 2X ETH long position
6. The system now has 2 ETH
7. The price of ETH goes down 500 USD, it is now 500 USD each
8. The system now has 1000 USD worth of ETH
9. Bob can get liquidated as his initial supplied collateral is now worth 50% of what he has borrowed
10. Chris liquidates Bob's position, gains a liquidation fee paid in ETH and the system fee reserves increase plus retains the remaining collateral.

\---

Necc protocol prevents cascades of liquidations/flash crashes systematically via the following with each synchronous liquidation call:&#x20;

- Funding rates are paid out for that volatile token and updated
- Reserved and guaranteed collateral amounts are updated for future NDOL redemptions
- The mark price of the liquidated collateral is either the min price for longs or the max price for shorts from the Flux price feed&#x20;
- Validations are made to revert transactions if losses, margin or liquidation fees exceed position collateral and max leverage is surpassed
