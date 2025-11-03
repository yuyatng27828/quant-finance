# 3.6 Stack and Roll

## Purpose
Used when the hedging horizon is longer than the maturity of available futures contracts. <br>
>> Maintain a hedge over time by rolling short-term futures positions forward.

## Concept
- Stack = Open a "stack" of short-term futures to hedge long-term exposure.
- Roll = When contracts near expirty, close them and open new ones with later maturities.
- Repeat until the hedge horizon ends.

## Risks
- Basis risk = Each roll, the spot futures relationship may change >> small gains/losses.
- Roll yield (roll cost)
  - Contango (future price > spot) = Rolling costs money
  - Backwardation (future price < spot) = Rolling gains money
  - Transaction/liquidity risk = Each roll incurs bid-ask spreads, commisions, slippage

## Usage
- Commodity producers/consumers
- Portfolio managers hedging index exposure
- Corporates with long-term FX or rate risk

## Formula
$$Position_i = h \times \frac{V}{F_i}$$ <br>
where
- $$h$$ = hedge ratio
- $$V$$ = value of exposure
- $$F_i$$ = current futures price at roll $$i$$
