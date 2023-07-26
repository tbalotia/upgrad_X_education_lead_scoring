# X Education Lead Scoring Assignment
## Background
X Education is an online education company that offers various courses and training programs to potential customers through its website. The sales team at X Education faces challenges in converting website visitors into leads, and ultimately, into paying customers. To address this, the company is interested in implementing a lead scoring model that can prioritize potential leads and help the sales team focus their efforts on the most promising prospects.

## Problem Statement
The goal of this assignment is to build a logistic regression model for lead scoring that can predict the likelihood of a website visitor getting converted into a paying customer. The model will be trained on historical data of leads and their conversion status, and it will be used to predict the probability of conversion for new website visitors.

## Data Description
The dataset provided for this assignment contains information about various leads and their interactions with the X Education website. It includes both numerical and categorical features such as 'TotalVisits', 'Total Time Spent on Website', 'Page Views Per Visit', 'Lead Origin', 'Lead Source', 'Specialization', 'Last Activity', and more.

## Steps in the Analysis

1. Data Preprocessing:

	*	Handling missing values: We will explore the dataset to identify columns with missing values and decide on the appropriate strategy for imputation or removal of those rows/columns.
	*	Dropping irrelevant columns: Some columns, such as 'Prospect ID' and 'Lead Number', have no impact on lead conversion and can be dropped from the analysis.
	*	Encoding categorical variables: We will convert categorical variables into dummy/indicator variables so that they can be used in the logistic regression model.
2. Data Analysis:

	*	Exploratory Data Analysis: We will analyze the distribution and summary statistics of numeric variables, as well as the value counts of categorical variables, to gain insights into the data.
	*	Feature Selection: We will use Recursive Feature Elimination (RFE) to select the most relevant features for the logistic regression model.
3. Model Building:

	*	Train-Test Split: We will split the dataset into training and testing sets to train the logistic regression model and evaluate its performance on unseen data.
	*	Feature Scaling: If required, we will apply feature scaling to numeric columns to ensure that they are on a similar scale.
4. Logistic Regression:

	*	We will build a logistic regression model using the selected features from RFE and fit it on the training data.
	*	Model Evaluation: We will evaluate the performance of the model using metrics such as confusion matrix, classification report, ROC-AUC score, accuracy, sensitivity, and specificity.
5. Optimal Threshold:

	*	We will plot the ROC curve and decide on the optimal probability threshold for classifying a lead as converted or not.
	*	Using the optimal threshold, we will calculate the accuracy and sensitivity metrics for the model.

## Conclusion
The logistic regression model developed in this assignment will help X Education in predicting the probability of lead conversion for new website visitors. By focusing on leads with higher conversion probabilities, the sales team can optimize their efforts and improve lead conversion rates.

Note: The code and analysis provided in this repository are for educational purposes only and may not represent a complete or production-ready solution.
