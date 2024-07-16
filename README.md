# A VAR Model Analysis of Consumer Price Index Volatility in the UK (2001-2022): Impact of Macroeconomic Variables

## Introduction
Consumer Price Index (CPI) is a crucial indicator that reflects mean changes in consumer expenses for specified goods and services over time. It serves as a benchmark for understanding inflation trends and aids professionals in policymaking, economic analysis, and risk management. Understanding the relationship between CPI and other macroeconomic variables enhances decision-making by revealing how different parameters react in the economy.

Vector Autoregression (VAR) modeling is employed in this study to analyze the yearly data from 2001 to 2022, aiming to understand the relationship between macroeconomic variables and CPI volatility. This approach helps in assessing the extent of each variable's contribution to changes in consumer price levels over time.

## Methodology

### Models Used
- **VAR Model:** Utilizes a similar approach as the paper "The Relationship Between Selected Financial and Macroeconomic Variables with Consumer Confidence Index" by Cagatay Basarir et al. The procedure involves unit root tests, Granger causality tests, and VAR model estimation with optimal lag length determination.
- **GARCH Model:** Referencing "Analysing Volatility of Colombo Consumer Price Index using GARCH Models" by Alibuhtto (2014). The study employs GARCH models, including GARCH (1, 1), TGARCH (1, 1), and EGARCH (1, 1), to analyze CPI volatility.

### Data Variables
- **Control Variable:**
  - Year: 2001-2022
- **Dependent Variable:**
  - LOG CPI: Consumer Price Index (base year 2015)
- **Independent Variables:**
  - LOG RETURNS: Stock market returns
  - LOG GDP GROWTH: GDP growth rate
  - LOG BANK RATE: Base rate set by the Bank of England
  - LOG VIX: Volatility Index
  - LOG TOTAL TRADE INFLOWS: Total trade inflows to the UK
  - LOG INFLOWS: Foreign direct investment inflows
  - LOG EXCHANGE RATE: Exchange rate (Pounds to Dollars)
  - LOG UNEMPLOYMENT: Unemployment rate
  - LOG GROWTH RATE: Population growth rate

### Data Analysis
- **Stationarity Test:** Conducted using the Augmented Dickey-Fuller (ADF) test. LOG CPI is found to be stationary with a p-value of 0.9986.
- **VAR Model:** Estimated with LOG CPI as the dependent variable. Significant variables include Bank Rate, Volatility Index, Trade Inflows, and Foreign Direct Investments at various critical levels.

### Diagnostic Tests
1. **Lag Selection:** Akaike Information Criterion (AIC), Bayesian Information Criterion (BIC), Final Prediction Error (FPE), and Hannan-Quinn Information Criterion (HQC) indicate lag 1 as appropriate.
2. **Granger Causality Test:** p-value of 0 indicates causality in the time series.
3. **Lagrange Multiplier Test:** Indicates autocorrelation among variables.
4. **Eigenvalue Stability Condition:** Model found unstable at lag 1.
5. **Wald Lag Exclusion Test:** Indicates significance at lag 1.

## Conclusion
The study provides preliminary insights into the extent CPI is affected by macroeconomic variables. Future research should include more data and advanced tests to stabilize the model and enhance its accuracy. Additional variables could be incorporated to better understand the nuanced relationship between CPI and the economy.
