# Natural-Gas-Futures-Price-Forecasting-using-Facebook-Prophet
Time series forecasting of Natural Gas futures prices using univariate and multivariate Prophet models with Fourier seasonality.

# Natural Gas Futures Price Forecasting using Facebook Prophet

## Project Overview
This project applies the Facebook Prophet framework to forecast daily
Natural Gas futures prices from January 2002 to December 2023.

Both univariate (price-only) and multivariate (price + exogenous variables)
models are developed, with seasonality captured using Fourier series.

---

## Dataset Description
- Daily Natural Gas futures prices
- Time period: 2002–2023
- Additional exogenous variables included
- Long, volatile time series with structural shifts

---

## Methodology
- Facebook Prophet forecasting framework
- Additive trend and seasonality components
- Fourier order:
  - Base model: 6
  - Sensitivity analysis: 8
- Model evaluation using forecast accuracy metrics

---

## (a) Prediction Accuracy (Fourier Order = 6)

### Univariate Model
- Captures long-term trend and seasonality
- Performs adequately during stable market regimes
- Struggles during sudden price shocks and volatility spikes

### Multivariate Model
- Incorporates external drivers of price movements
- Demonstrates lower forecast error
- Better responsiveness to macro and supply–demand conditions

**Conclusion:**  
The multivariate Prophet model outperforms the univariate model in terms of
forecast accuracy and robustness.

---

## (b) Impact of Increasing Fourier Order to 8

- Higher flexibility in seasonal pattern capture
- Slight improvement in in-sample fit
- No consistent improvement in out-of-sample accuracy
- Increased risk of overfitting

**Conclusion:**  
Fourier order 6 provides a better balance between accuracy and stability,
while Fourier order 8 offers limited incremental benefit.

---

## (c) Limitations of the Framework
1. Limited ability to handle abrupt structural breaks
2. Additive structure may not capture nonlinear price dynamics

---

## Tools & Skills Demonstrated
- Time series forecasting
- Facebook Prophet
- Univariate & multivariate modeling
- Seasonality modeling using Fourier series
- Commodity price analysis

---

## Business Relevance
Applicable to:
- Energy price forecasting
- Risk management and hedging
- Trading strategy support
- Macroeconomic analysis
