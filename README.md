# Fair-Pricing-of-ABRC

Crude Monte Carlo method is used to price an Autocallable Barrier Reverse Convertible issued by Credit Suisse. 
Variance reduction techniques including control variate and antithetic variate are applied. 
Stress testing is applied to calculate the fair prices and expected values of the product under Worst Case Scenario under various stress levels of interest rate volatility and stock volatility. (See Project_Tim_stochastic)

Project_Tim: a fixed 23bps of risk-free rate is used to discount future cashflows

Project_Tim_Stochastic: a stochastic risk-free rate following CIR model is used instead. 

A vectorized stress testing function is currently under development in Project_Tim_Stochastic
