Problem 1. Linear Regression

Use the data in the baseseg.csvPreview the document file on kidney disease to construct a good fitting model for GFR as a function of the following potential predictors measured at baseline

1) Serum Creatinine (bascre); 2) Systolic blood pressure (sbase); 3) Diastolic blood pressure (dbase); 4)Urine protein (baseu); 5) Age; 6) Gender (Sex = 1 if male; = 0 if female); 7) African-American (black)

When building your model, consider potential transformations of the outcome and variables as well as interaction terms.

Examine the fit of your model by regression diagnostics by checking model assumptions such as constancy of variance, linearity, normality and characteristics such as outliers, influence, etc).

Describe your findings in clearly written text, tables and figures. Discuss which factors are predictive and how. Show some predictive plots showing outcomes as a function of the predictors.

 

Problem 2. Logistic Regression

Wells in Bangladesh used for drinking are often contaminated by natural arsenic which can cause diseases as exposure accumulates in someone’s body. If someone’s well is contaminated, a neighbor’s well may be safe and so if they agree, one can switch to sharing their well. After a research team measured arsenic levels in all the wells in a certain area, residents were urged to switch wells if theirs was labelled unsafe (more than 0.5 hundred micrograms per liter, i.e. 50 micrograms). A few years later the researchers returned to see who had switched wells. The data are in the file wells.txtPreview the document, found in the data sets folder. They include 5 variables for 3020 wells

switch is a binary indicator for whether the household switched wells
arsenic is the level of arsenic in the well in hundreds of micrograms per liter
dist is the distance to the nearest safe well in meters
assoc is whether household members are active in community organizations
educ is the number of years of education of the head of household.
First construct a training data set of the first 2520 wells and a test data set of the last 500.

Construct a good logistic regression model predicting the decision to switch wells as a function of the 4 predictors (arsenic, distance, association and education) on the training data. Consider potential transformations of continuous variables and possible interactions.
Compute and graph the predicted probabilities stratifying by the predictors. You could do this using graphs such as in the papers we discussed in class or by using contour plots which would allow you to graph two continuous predictors on the same plot. You can array different lines and plots to try to put this all on one sheet or you can spread across different plots. See what works best.
Compute the confusion matrix on the test data using p = 0.5 as a cutoff and discuss what this tells you about the predictive model you have constructed (e.g. sensitivity, specificity, error rate, etc.)
Construct an ROC plot and compute the area under the ROC curve.
What does this curve tell you about choice of threshold that balances sensitivity with specificity (i.e., how would you balance risk of switching and not switching?)
