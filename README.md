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


Use packages:
import pandas as pd 
import numpy as np
import matplotlib.pyplot as plt 
import seaborn;seaborn.set() 
from scipy.stats import norm 
from math import log

