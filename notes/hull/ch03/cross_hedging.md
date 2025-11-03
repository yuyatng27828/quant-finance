# 3.4 Cross-Hedging
Hedging an exposure by using a futures contract on a different asset (becasue no exact match exists).
E.g. an airline heding jet fuel using heating oil futures.

## Optimal Hedge Ratio
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

## Optimal Number of Futures Contracts
- $$N^* = h^* \times \frac{V_A}{V_F}$$ <br>

where:
|Symbol|Meaning|
|:---|:---|
|$$N^*$$|Optimal number of futures contracts|
|$$V_A$$|Value of the asset being hedged|
|$$V_F$$|Value of one futures contract|

## Hedge Effectiveness
- $$\rho^2$$ = % of variance reduction  
- $$1 - \rho^2$$ = basis risk due to imperfect correlation 

