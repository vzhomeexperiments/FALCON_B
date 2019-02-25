# FALCON_B

Designed to work best with Decision Support System developed inside Lazy Trading Project

https://vladdsm.github.io/myblog_attempt/topics/lazy%20trading/

# Introduction

FALCON_B is the modified version of The-Falcon:

* Let robot to log results of the trades to the file
* Let robot be disabled unless it's flagged to be enabled by external software

# Reference

Functionality of this robot is explained in the Udemy course [Lazy Trading Part 2: Set up your Trading Strategy Robot
](https://www.udemy.com/your-trading-robot/?couponCode=LAZYTRADE-GIT)

# Optimization Method

1. set up date to be | Start: Today - 3month; End: Today - 1 month
2. open prices | M15 chart
3. optimize 4 strategy parameters + stop levels volatility parameters 
4. during optimization set max 10 trades, lots = 0.01
5. check in the folder TEST file 're-train' which systems need optimization
6. once optimization parameters are found set date to be | Start: Today - 1month; End: Today
7. test obtained parameters on independent data, prefer those that have rising tendency...
8. once parameters are found, store them into the folder 'PARAMETERS' | name file EURAUD_M15.set
9. deploy parameters in Terminal 1, keep max 10 trades, fixed lot size 0.01
10. deploy parameters in Terminal 3/4 max 1 trade, lot sizing ON with 1% risk

# Disclaimer

Use on your own risk: past performance is no guarantee of the future results!
