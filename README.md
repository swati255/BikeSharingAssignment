# bike_sharing_assignment_upgrad

Observations and explanations from our assignment:
<ol>
<li>There is an increase in the bike rental count in spring and summer season , and then decrease in the bike rental count in fall and winter season.

<li>The bike rental count distribution is higher in 2019 than in 2018.

<li>During no holidays, the bike rental counts is the highest, compared to during holidays for different seasons.

<li>There is no significant change in bike demand with working days and non working days.

<li>During clear, partly cloudy weather, the bike rental count is the highest, second-highest during misty cloudy weather, and followed by 3rd highest, during light snow and light rain weather.

<li>Outlier analysis:<br>
(i) No outliers are present in total_count variable.<br>
(ii) No outliers are present in normalized temp but few outliers are present in normalized windspeed and humidity variables.

<li>Normal probability plot is a graphical technique to identify substantive departures from normality and also it tells about goodness of fit. In our normal probability plot, some target variable data points are deviating from normality.

<li>Correlation matrix tells about linear relationship between attributes and helps us to build better models. From our correlation plot, we can observe that some features are positively correlated and some are negatively correlated to each other. The temp and atemp are highly positively correlated to each other, it means that both are carrying same information.The total_count,casual and registered are highly positively correlated to each other. So, we have ignored atemp,casual and registered variable for further analysis.

For modelling the datset, we split the dataset into train and test in the ratio of 70:30.

<li>Training dataset:<br>
(i) While fitting Linear regression to our trained dataset, Accuracy of the model: 82.4 %<br>
(ii) Cross validation prediction plot tells about finite variance between actual target value and predicted target value. In our Cross validation prediction plot for training dataset, some data points are have same finite variance between them and some are not having it.<br>
(iii) Model Evaluation metrics: R-Squared (R² or the coefficient of determination) is a statistical measure in a regression model that determines the proportion of variance in the dependent variable that can be explained by the independent variable.The R-squared or coefficient of determination for our model is 0.81 on average , it means that predictor is only able to predict 81% of the variance in the target variable which is contributed by independent variables.

<li>Testing dataset:<br>
(i) Model Evaluation metrics: Root Mean Square Error (RMSE) is the standard deviation of the residuals (prediction errors), and The mean absolute error of a model with respect to a test set is the mean of the absolute values of the individual prediction errors on over all instances in the test set.

For our model, 
Root mean square error : 802.4291866599553
Mean absolute error : 595.2441391283483
  
<li>Residual plot tells about finite variance between actual target value and predicted target values. In our Residual plot,very less data points are having the same finite variance between them.
</ol>


<hr>

License
=========================================
The dataset used in this assignment has been obtained from the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}

=========================================
Contact
=========================================
	
For further information about this dataset please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt)
