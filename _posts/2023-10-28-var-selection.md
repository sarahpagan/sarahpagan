# Variable Selection

## What variable selection techniques do you prefer?

The variable selection techniques I’ve employed the most have been backward elimination and forward selection. I’ve been taught these procedures in several statistics courses prior to ST 558 and these methods always made practical, intuitive sense to me. However, learning about the lack of theory behind them has inspired me to take stock in the many other possible variable selection techniques available to me. Furthermore, I’ve learned from the *“Variable selection – A review and recommendations for the practicing statistician”* paper that backward elimination and forward selection are only reliable if a small number of pre-specified models are compared. Otherwise, multiple testing becomes an issue. And these procedures fail to test if a variable is relevant in absolute, but rather test if it is relevant given other predictors in the model.  All said, I would like to keep these procedures as part of my toolkit and acknowledge their issues, while expanding my practice to include other variable selection techniques.

The following are some techniques I’d prefer to keep in mind moving forward in my career: 

1. Use background knowledge to identify an initial set of working variables. Understand the relationship of the variables to the response without yet consulting the data. Remove redundant variables or variables without interest from consideration.
    - This technique seems simple, but it’s always helpful to remind myself to reconsider objectives and relevancy often while analyzing data!
2. Calculate the EPV (events per variable) ratio. Consider the greater than 15 rule of thumb — limit variables so that there are at least 15 observations per variable included in the model.
    - I would not employ this technique as hard and fast rule, but I think it's a helpful reminder of the risk of overfitting.
3. Calculate all possible subsets. Compare models in terms of **several** optimization criteria. Investigate AIC, adjusted R squared, Mallows Cp, etc.
    - Criterion-based methods have been suggested over stepwise regression by some of our readings. Coupled with the reality that computing power is less of a concern now, I think employing best subset techniques would be a good approach.
4. Apply shrinkage methods like LASSO. Remember to standardize predictors.
      - This technique is helpful for estimating regression coefficients when many predictors have a small influence on the response. It also has a "built-in" variable selection feature in a way, with the possibility of shrinking a coefficient to zero.
5. Use k-fold cross validation when model building. Minimize prediction error rate on a test data set when prediction is the goal.
      - The idea of splitting data into a training and test data set is new to me and very compelling. I would hesitate to use this technique on small data sets, but otherwise I see it as very practical tool for verifying my work.
