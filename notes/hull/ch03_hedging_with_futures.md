# 📖 Chapter 3: Hedging Strategies using Futures

## 3.1 Basic Principles
A hedger uses futures contracts to reduce risk from price movements of an underlying asset (commodity, currency, index, etc.)

- **Perfect hedge** = completely eliminates risk (rare in practice)

- **Common type of hedges**
  - Short hedge = Take a short futures position when you anticipate selling an asset in the future (to protect from price declines)
  - Long hedge = Take a long futures position when you anticipate buying an asset in the future (to protect from price increases)

- Hedgers need to consider
  - Which contract to use
  - The size of the futures position (hedge ratio)
  - Whether to adjust the hedge during its life (static vs dynamic strategies)

## 3.2 Arguments For and Against Hedging
- **For hedging**
  - By reducing risk, a firm can focus on its core business, avoid large undesirable fluctuations, improve planning and stability

- **Against hedging**
  - If already diversified, so the firm's hedge might reduce upside as well as downside
  - Hedger may be at a disadvantage compared to competitor if hedge does not work in favor

Hedging reduces uncertainty of outcomes (makes them more predictabl), but does not guarantee higher profits. Often trades off upside potential for downside protection.

## 3.3 Basis Risk
*Basis = Δ(Spot price - Futures price)*
Your hedge is imperfect because the futures price and actual underlying spot price don't move in perfect sync.

- **Spot** = Your real economic exposure 
- **Futures** = Your insurance contract to protect aginst spot price moves
*If you don't have a spot exposure, you're not hedging, you're speculating.

**Case 1: You own the asset (long spot)**
|Market move|Spot PnL|Futures PnL (short futures)|Net|
|:---|:---|:---|:---|
|Price rises| + | - |roughly 0|
|Price falls| - | + | roughly 0|

You short futures to protect against a price fall = short hedge

**Case 2: You need to buy the asset later (short spot)**
|Market move|Spot PnL|Futures PnL (long futures)|Net|
|:---|:---|:---|:---|
|Price rises| - | + |roughly 0|
|Price falls| + | - |roughly 0|

You go long futures to protect against a price increase = long hedge

## 3.4 Cross-Hedging
Hedging an exposure by using a futures contract on a different asset (becasue no exact match exists).
E.g. an airline heding jet fuel using heating oil futures.

**Optimal Hedge Ratio**  
- $$h^* = \frac{Cov(\Delta S, \Delta F)}{Var(\Delta F)}$$  
- $$h^* = \rho \frac{\sigma_S}{\sigma_F}$$

where:
|Symbol|Meaning|
|:---|:---|
|$$\Delta S$$|Change in spot price|
|$$\Delta F$$|Change in futures price|
|$$\sigma_S, \sigma_F$$|Standard deviations of $$\Delta S$$ and $$\Delta F$$|
|$$\rho$$|Correlation between $$\Delta S$$ and $$\Delta F$$|

$$h^*$$ indicates how many futures contracts' worth of exposure should be used to optimally hedge 1 unit of spot exposure.

**Optimal Number of Futures Contracts**  
- $$N^* = h^* \times \frac{V_A}{V_F}$$

where:
|Symbol|Meaning|
|:---|:---|
|$$N^*$$|Optimal number of futures contracts|
|$$V_A$$|Value of the asset being hedged|
|$$V_F$$|Value of one futures contract|

**Hedge Effectiveness**  
- $$\rho^2$$ = % of variance reduction  
- $$1 - \rho^2$$ = basis risk due to imperfect correlation 

## Hedging an Equity Portfolio using Stock Index Futures
Institutional investors often hold equity portfolios and face systematic market risk (i.e. their portfolio moves with the market index).

They may want to:
- Hedge this market risk = reduce exposure
- Change the market exposure (adjust $$\beta$$)
via futures rather than selling/buying the underlying stocks dus to enhanced efficiency and liquidity.

**Key Variables**
- $$V_A$$ = Current value of the portfolio being hedged.
- $$V_F$$ = Value (notional) of one index ftures contract = (futures price) $$\times$$ (contract size)
- $$\beta$$ = Beta of the portfolio relative to the index (sensitivity of portfolio returns to index returns)
  - $$\beta = 1$$: portfolio moves roughly like the index
  - $$\beta > 1$$: portfolio is more volatile than the index
  - $$\beta < 1$$: portfolio is less volatile than the index

**Number of Futures Contracts to Hedge**
- $$N^* = \beta \times \frac{V_A}{V_F}$$  
- If you want to reduce your $$\beta$$ to zero (fully hedge market risk), you short $$N^* $$ contracts.
- If you want to increase you $$\beta$$, you go long contracts accordingly.

**Insights and Practical Notes**
- This hedge covers market/systematic risk, but not idiosyncratic risk (specific stock risk) - so the portfolio may still underperform or outperform due to stock-specific moves.

- Compute the number of futures contracts to hedge when adjusting for a target $$\beta$$ ($$\beta^*$$):
  - $$N = (\beta - \beta^* ) \times \frac{V_A}{V_F}$$

