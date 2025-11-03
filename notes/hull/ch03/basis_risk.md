# 3.3 Basis Risk

## What is basis risk
*Basis = Δ(Spot price - Futures price)*
Your hedge is imperfect because the futures price and actual underlying spot price don't move in perfect sync.

- **Spot** = Your real economic exposure 
- **Futures** = Your insurance contract to protect aginst spot price moves

*If you don't have a spot exposure, you're not hedging, you're speculating.

## Case 1: You own the asset (long spot)
|Market move|Spot PnL|Futures PnL (short futures)|Net|
|:---|:---|:---|:---|
|Price rises| + | - |roughly 0|
|Price falls| - | + | roughly 0|

You short futures to protect against a price fall = short hedge

## Case 2: You need to buy the asset later (short spot)
|Market move|Spot PnL|Futures PnL (long futures)|Net|
|:---|:---|:---|:---|
|Price rises| - | + |roughly 0|
|Price falls| + | - |roughly 0|

You go long futures to protect against a price increase = long hedge
