There are database with information about the characteristics of cars is given (data in the file cars.csv).

### Tasks:
1.  Determine what factors affect car pricing.
2.  Determine which variables are important for forecasting and how well the resulting model describes the data.
3.  Predict the cost of cars

### After some data transformations, the first model was built with only one predictor of price: (price) - horsepower

This model explains 65% of the price variability.

![](https://user-images.githubusercontent.com/104904113/202207153-6f2698b2-6e55-4bf7-a990-0b892e62219e.jpg)

### Then a model with all predictors was built

This model explains 95% of the price variability. However, only 3 car brands are significant in this model (p<0.05)

![](https://user-images.githubusercontent.com/104904113/202207454-54fc8b94-8d39-4d9e-bb79-40bfd493ec52.jpg)

### Then a model was built with all predictors except car brands

This model explains 90% of the price variability. Among the predictors, 10 out of 27 were not significant (p > 0.05)
![](https://user-images.githubusercontent.com/104904113/202206905-01bd1048-857e-45e6-a7f5-abc4ae7f731d.jpg)

### Conclusion: 
since Adj. R-squared in the last two models has not changed significantly, it is better to choose a model without car brands

### Interpretation (price prediction) assuming that the other variables remain unchanged:
1. the price INCREASES by 86.8164 for a single change in horsepower
2. the price INCREASES by 36.0515 for a single change in enginesize
3. the price INCREASES by 71.1868 for a single change in wheelbase
