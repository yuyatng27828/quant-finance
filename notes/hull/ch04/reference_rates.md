# 4.2 Reference Rates

## Definition
- Reference rates are benchmark interest rates used to determine payments of floating-rate financial instruments (e.g. swaps, loans, futures)

- They represent the cost of borrowing money in the interbank market (i.e. what a bank would charge another for short-term loans)

## Major reference rates
LIBOR (London Interbank Offered Rate)
- Historically the most used global benchmark
- Based on submissions from major banks on how much they would charge to lend unsecured funds to other banks
- Existed for several curencies (USD, GBP, EUR, JPY, CHF) and maturities (overnight to 12 months)
- Manipulation scandals + declining interbank lending volume &rarr; discontinued in 2023

SOFR (Secured Overnight Index Average)
- Replacement for USD LIBOR
- Based on actual transacctions in the US Treasury repo market (banks borrow cash overnight using US Treasuries as collateral)
- Hence, secured (lower credit risk than LIBOR)
- Published by the Federal Reserve Bank of New York
Considered robust and transaction-based

SONIA (Sterling Overnight Index Average)
- Replacement for GBP LIBOR
- Based on unsecured overnight lending between banks and other institutions
- Administered by the Bank of England

&euro;STR (Euro Short-Term Rate)
- Replacement for EUR LIBOR and EONIA
- Reflectd borrowing costs of euro-area banks in the unsecured overnight market
- Published by the European Central Bank (ECB)

TONIA (Tokyo Overnight Average Rate)
- Replacement for JPY LIBOR
- Based on uncollateralized overnight call rates in Japan
- Published by the Bank of Japan

## Key differences between old and new benchmarks
|Feature|LIBOR|SOFR/SONIA/&euro;STR/TONA|
|:---|:---|:---|
|Type|Estimated|Transaction-based|
|Secured|Unsecured|Mostly secured (e.g. SOFR)|
|Credit Risk|Includes bank credit risk|Minimal or none|
|Publication|Forward-looking (term structure)|Overnight, backward-looking|

## Implications for Derivatives Pricing
- Modern derivatives now reference risk-free rates (RFRs) like SOFR
- Discounting and forward-rate calculations now use compounded overnight RFRs
- Transition from LIBOR &rarr; RFR affects
  - Swap valuation
  - Hedge accounting
  - Risk management systems



