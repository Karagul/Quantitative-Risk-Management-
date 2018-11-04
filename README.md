# Quantitative-Risk-Management
Quantitative Risk Management School Homework and project

Calibration
Let E be Exxon Mobile stock (ticker XOM), and I be Intel stock (ticker INTC). Their historical
values are in the spreadsheets XOM-bloomberg.csv and INTC-bloomberg.csv, respectively, which were downloaded using the Bloomberg Excel API.
Let μ(S, t, l) and σ(S, t, l) be the estimated drift rate (mean) and relative volatility parameters for a GBM process S computed on date t using the last l years worth of observations (i.e. assume dS = Sdt + σSdW and that μandσ are constant over that set of observations).

## 1) Moving Average



Tabulate and graph μ(S, t, l) andσ(S, t, l) for S = E and S = I for t ranging over the last 20 years, and l being 2, 5, and 10 years, using unweighted fitting. Use adjusted closing prices.
Why are the computed parameters over time comparable even though the value invested varies?
How stable do the results look?

## 2) Exponential Weighting


Some references say to use exponential weighting with λ=0.94 or λ = 0.97, to calibrate to the
last few weeks or about a month of data. These λs correspond roughly these periods because the weight becomes 1/2 after approximately 14 days and 22 days, respectively.
To see the impact of exponential weighting with these weights, repeat the previous problem using exponential weighting, with λ = 0.94 and λ = 0.97.

## 3) Equivalence

Equivalence What λs should be used for exponential weighting to get results most similar to using windows of 2, 5, and 10 years, respectively?

## 4) Historical estimates with equivalent λ

Repeat exponential weighting parameter estimation using the above computed λ equivalent to 2 year, 5 year and 10 year windows. Compare the windowed versions to the corresponding equivalent exponentially weighted versions.

## 5) Formula VaR and ES from historical estimates

Using the estimates for the drift and volatility from last week using 2year, 5year and 10year windows, and using the corresponding equivalent exponential weights from above, tabulate and graph the VaR(S, T, p) and the ES(S, T, p) for S being E and L, using p = 0.99, p = 0.975, and T = 5days (i.e. one week), for each day over the last 20 years, or as far back as the above estimates were done. Tabulate and graph. Computing them assuming a $10,000 position each day.


