# 4.3 THe Risk-Free Rate

## Definition
- The interest rate on an investment with no default risk and no uncertainty about future payments
- The theoretical baseline for valuing all other assets - every risky asset's expected return is measured relative to the risk-free rate

## In Practice
There is no truly risk-free security, but some instruments are treated as practically risk-free due to their creditworthiness and liquidity.
|Currency|Common Proxy for Risk-Free Rate|Typical Instrument|
|:---|:---|:---|
|USD|Treasury securities|T-bills, Treasury notes/bonds|
|EUR|German government bonds|Bunds|
|GBP|UK Gilts|Treasury gilts|
|JPY|Japanese Government Bonds|JGBs|

## Key Properties of a Risk-Free Asset
- No default risk - issuer (e.g. government) is assumed to always repay
- Known cash flows - future payments and timing are fixed
- High liquidity - can easily be traded without price impact
- Denominated in the investor's domestic currency - eliminates FX risk

## Which Rate to Use
- For theoretical pricing (like in the Black-Scholes model), we use the continuously compounded risk-free rate
- In practice, the choice of instrument depends on the maturity of the derivative or bond being valued

|Use Case|Appripriate Risk-Free Rate|
|:---|:---|
|< 1 year|Treasury Bill yield|
|1-10 years|Treasury Note yield|
|> 10 years|Treasury Bond yield|
|Short-term interbank models|Overnight indexed swap (OIS) rate|

## LIBOR vs OIS
- Historically, LIBOR (London Interbank Offered Rate) was used as the benchmark "risk-free" rate
- But LIBOR included bank credit risk &rarr; not truly risk-free
- Now, OIS (Overnight Indexed Swap) rates are preferred because they reflect nearly risk-free overnight lending betwen baks, closely matching central bank policy rates

Example:
- LIBOR = 2.2% and the OIS = 2.0%
- 0.2% spread = interbank credit and liquidity risk

## Real vs Nominal Risk-Free Rate
|Type|Definition|Formula/Example|
|:---|:---|:---|
|Nominal rate|Rate including inflation expectations|e.g. Treasury bond yield = 4%|
|Real rate|Rate after removing inflation|$$r_{real} \approx r_{nominal} - \pi_{expected}$$|

## Why it matters
The risk-free rate is foundational for:
- Discounting cash flows in pricing models
- Computing forward/future prices
- Option pricing (Black-Scholes)
- Portfolio theory (e.g. CAPM)
- Performance measurement (Sharpe ratio)

