# Overview

This repository implements a finite-horizon dynamic programming model inspired by Herkenhoff (2019).

* Housholds choose whether to work, apply for credit, borrow, default, and consume under uncertainty about job opportunities, productivity, and expense shocks.
  Households are also differed by immigrants vs. natives, where immigrants face an extra hiring cost during their job-search process.
* Firms in this economy choose the wage they are going to offer based on state conditions
* Lenders will decide whether they will offer credit access to households, and how much they will give out.

The policy functions are solved using vectorized value function iteration (VFI) and simulated using NumPy-based backward iteration.

The model will be calibrated to SIPP data, where immigrants differ in hiring cost, planning horizon, cost to obtain credit,  and bond price premium.  

# Model Features
* 120-period finite-horizon VFI
* Joint labor, credit, and consumption choices
* Stochastic productivity, job offers, and shocks
* Borrowing limits and credit-approval frictions
* Immigrant vs. native parameterization
* Fully vectorized terminal-period and intermediate-period updates
* Calibration using SIPP
