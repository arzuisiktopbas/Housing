# Housing

## RESULTS:

* Area,bedrooms,bathrooms,stores and Boolean-values are affecting house prices. They are responsible for 67% of the variation in house prices. (Adj. R-squared=67%)

*  Areas, bathrooms and stores are of critical importance. They are responsible for 52% of the variation in house prices.

   - A 1,000-unit increase in area increases house prices by about $244,000.
   
   - The addition of 1 more bathroom increases house prices by $987,700.
   
   - The addition of 1 more store increases house prices by $450,800.
   
* I checked the OLS assumptions. And found no evidence of voiloation.

 **Explanation of other variables**

* Being close to a mainroad increases house prices by $421,300.

* Having a guestroom, basement, hotwaterheating, airconditioning, and preferarea increases house prices by 300,500 , 350,100 ,  855,400 , 865,000, and $651,500, respectively.

* A house with a furniture is more valuable than an unfurnished house by $411,200. There is no statistical difference in house prices of semi-furnished and unfurnished premises.

**Linear Regression Assumptions**

* No Endogeneity: I did the Durbin-Wu Hausman tests for area. All p-values are greater than 0.10. So, we do not have endogeneity problem at 10% significance level.

* Normality of Errors: I drew the histogram of the residuals from the OLS regression, and the distribution is very close Normal centered at 0. Also, Shapiro–Wilk test did not reject that residuals are normally distributed.

* Homoskedasticity: I plotted the residuals versus fitted (predicted) values. On the left end of the graph , the residuals seem to fluctuate more, i.e. higher variance, which is an indication of heteroscedasticity. But homoskedasticity does not seem to be a major problem. I also ran the robust regression (RLM) by allowing heteroskedastic error term but the standard errors didn’t change much.

* No Multicollinearity: I checked VIFs. Mainroad(5.51) has the highest VIF value.
