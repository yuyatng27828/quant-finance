# 3.5 Hedging an Equity Portfolio using Stock Index Futures
Institutional investors often hold equity portfolios and face systematic market risk (i.e. their portfolio moves with the market index).

They may want to:
- Hedge this market risk = reduce exposure
- Change the market exposure (adjust $$\beta$$)
via futures rather than selling/buying the underlying stocks dus to enhanced efficiency and liquidity.

## Key Variables
- $$V_A$$ = Current value of the portfolio being hedged.
- $$V_F$$ = Value (notional) of one index ftures contract = (futures price) $$\times$$ (contract size)
- $$\beta$$ = Beta of the portfolio relative to the index (sensitivity of portfolio returns to index returns)
  - $$\beta = 1$$: portfolio moves roughly like the index
  - $$\beta > 1$$: portfolio is more volatile than the index
  - $$\beta < 1$$: portfolio is less volatile than the index

## Number of Futures Contracts to Hedge
- $$N^* = \beta \times \frac{V_A}{V_F}$$  
- If you want to reduce your $$\beta$$ to zero (fully hedge market risk), you short $$N^* $$ contracts.
- If you want to increase you $$\beta$$, you go long contracts accordingly.

## Insights and Practical Notes
This hedge covers market/systematic risk, but not idiosyncratic risk (specific stock risk) - so the portfolio may still underperform or outperform due to stock-specific moves.

Compute the number of futures contracts to hedge when adjusting for a target $$\beta$$ ($$\beta^*$$):
- $$N = (\beta - \beta^* ) \times \frac{V_A}{V_F}$$
