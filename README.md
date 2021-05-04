# Fair-Pricing-of-ABRC

Crude Monte Carlo method is used to price an Autocallable Barrier Reverse Convertible issued by Credit Suisse. 

Variance reduction techniques including control variate and antithetic variate are applied. 

Fixed risk-free interest and stochastic interest rate (CIR) are incorporated separately.

Stress testing is applied to calculate the fair prices and expected values of the product under Worst Case Scenario under various stress levels of interest rate volatility and stock volatility.

A vectorized stress testing function is currently under development, which aims to calculate the fair price, probability of each redemption scenario and expected value given Worst Case Scenario under flexible inputs including parameters of CIR, redemption and coupon payment dates, stress levels of intereste rate volatility (sigma in CIR) and stress levels of underlying stocks volatility, and number of simulations. 

Volatility surfaces of fair prices and expected value given Worst Case Scenario are visualized in the end of Project_Tim file.

# Assumption

Throughout the project, it is assumed that the daily lowest prices of underlying stocks follow a correlated Geometric Brownian Motions with parameters estimated by 3-year historical data. Coupon payments are quarterly compounded and priced are discounted continuously by risk-free rate under time convention actual/360. Parameters of CIR model are estimated by OLS using 3-year historical data of U.S. 1Y TSY. 

# Product Description

https://derivative.credit-suisse.com/ch/ch/en/detail/autocallable-brc-caterpillar-deere-co-8-25-p-a/CH0575750291/57575029
