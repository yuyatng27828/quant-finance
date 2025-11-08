# 4.4 Measuring Interest Rates

## Basic Definitions
|Term|Definition|
|:---|:---|
|Principal (P)|The initial amount invested or borrowed|
|Rate (R)|The annualized rate of return|
|Time (T)|Time in years|
|Compounding frequency (m)|Number of times interest is compounded per year|

## Simple Interest
Interest is no reinvested - you earn interest only on the principal <br>
Total Value = $$P(1 + RT)$$

## Compound Interest
Interest is reinvested each period - you earn interest on interest <br>
$$A = P(1 + \frac{R}{m})^{mT}$$

## Continuous Compounding
Interest compounds infinitely often &rarr; smooth exponential growth <br>
$$A = Pe^{RT}$$ <br>
Continuous compounding simpliifies many pricing formulas in finance (e.g. derivatives, bond pricing)

## Comparing Compounding Conventions
To compare rates with different compounding frequencies, use the effective annual rate (EAR): <br>
$$R_{eff} = (1 + \frac{R_{nominal}}{m})^m - 1$$

## Discount Factors
Discount factors translate a future cash flow into present value: <br>
$$d(t) = e^{-R_ct}$$ <br>
If continuously compounded rate = 5%, 1-year discount factor = $$e^{-0.05}$$ = 0.9512 <br>
Interpretation: $1 received in one year is worth $0.9512 today

## Continuously Compounded vs Compounded Annually
|Rate Type|Formula|Compunding Style|
|:---|:---|:---|
|Annual compounding|$$(1+R)^t$$|Discrete|
|Continuous compounding|$$e^{R_ct}$$|Continuous|
|Conversion|$$R_c = ln(1 + R)$$ and $$R = e^{R_c} - 1$$|-|
