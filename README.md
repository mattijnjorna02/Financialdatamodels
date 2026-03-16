# Financialdatamodels

This notebook will:


*  Model asset dynamics with Geometric Brownian Motion
*  Verify the Martingale Property
*  Price options using Black–Scholes
*  Extend to Merton Jump Diffusion
*  Simulate paths with Monte Carlo
*  Model volatility with GARCH
*  Build a trading strategy
*  Backtest with realistic assumptions

usage:
!pip install yfinance arch statsmodels --quiet
!pip install quantstats

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import yfinance as yf
import quantstats as qs

from scipy.stats import norm
from arch import arch_model
from statsmodels.tsa.arima.model import ARIMA
