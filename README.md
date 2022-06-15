# Goals of Linear Regression Model:-

	To model the demand for shared bikes with the available independent variables. It will be used by the management to understand
	how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand
	levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics
	of a new market.


Steps:-

	Step 1 - Reading Data.
	Step 2 - Understanding the Data by visualizing continuous & categorical variables.
	Step 3 - Data preparation:
				- Removing column which are not needed.
				- Removing extreme data from continuous & categorical variables.
				- Create dummy variables for categorical data, having more than two unique values.
	Step 4 - Model Building:
				- Split train & test data.
				- Data Training:
					- Rescale the continuous variables.
					- Use RFE to extract relevant features.
					- Build a model using these relevant features.
						- Check p-values & VIF for these variables.
						- Keep on deleting features one by one having high p-value & high VIF.
	Step 5 - Residual Analysis for train data:
				- Check residual is normally distributed with mean being zero.
				- Check there is no pattern in residual.
	Step 6 - Model Evaluation:
				- Scale the continuous variables using trained scalar.
				- Predict the output for test dataset.
				- Calculate the R-square value for test dataset.

Conclusion:-
	1. "temp" & "atemp" are highly corelated (0.991696).
	2. "registered" & "cnt" are highly corelated (0.945411).
	3. model parameters:
		season_3        0.31
		yr              0.28
		season_2        0.24
		season_4        0.23
		const           0.20
		mnth_10         0.14
		mnth_6          0.12
		mnth_5          0.11
		mnth_9          0.10
		mnth_8          0.06
		mnth_3          0.06
		windspeed      -0.07
		weathersit_2   -0.08
		weathersit_3   -0.29
	
Contributors:-

	1. Siddhant Srivastava

Developed as part of the Liner Regression Module required for Executive PG programme in Machine Learning And AI.
