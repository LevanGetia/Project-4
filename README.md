#Project Title: Retail Size Prediction Model
##Overview

This project encompasses the development of a predictive model aimed at enabling
retail sellers to efficiently stock up on clothing items by predicting the required
sizes for different categories of clothing across various seasons. The primary
objective is to minimize overstocking or understocking, thereby optimizing
inventory management and meeting consumer demands effectively.

##Data Collection

The dataset utilized in this project comprises historical sales data, customer
reviews, and product details from a retail clothing seller. The data encompasses
multiple attributes such as product ratings, review counts, available sizes, and
categorical data pertaining to clothing types and seasons.

##Data Cleaning and Preprocessing

The initial phase of the project involved extensive data cleaning and preprocessing
to ensure the quality and usability of the data for predictive modeling. The steps
included:

###Handling Missing Values: 
Missing data points were identified and imputed or removed, based on the nature and
significance of the missing information.

###Data Transformation: 
Non-numeric data fields, such as categorical variables representing clothing
categories and seasons, were transformed using one-hot encoding to facilitate their
use in the machine learning model.
###Feature Selection: 
Irrelevant features were dropped, and relevant features were selected based on
their potential impact on the target variables, i.e., the sizes.

##Model Development
The core of the project was developing a machine learning model capable of
predicting the demand for each clothing size. The steps involved were:

###Feature Engineering: 
Created combined features for each category and season, allowing the model to
understand the nuances of seasonal size demand.

###Target Variable Identification: 
Defined the target variable as a set of size-related columns, representing the
sizes in demand.
###Data Splitting: 
Split the data into training and testing sets to ensure the model could be trained
and evaluated effectively.
###Model Selection: 
Chose RandomForest as the primary algorithm for its robustness and suitability for
the dataset's characteristics.
###Multi-Output Classification: 
Adapted the RandomForest to predict multiple targets simultaneously using the
MultiOutputClassifier wrapper.
###Model Training and Evaluation: 
Trained the model on the training set and evaluated it on the test set, achieving
an accuracy of 83%.

##Model Evaluation

The RandomForest model's performance was meticulously evaluated using standard
classification metrics:

###Accuracy: Measures the proportion of correctly predicted instances. The model
achieved an 83% accuracy rate.

###Precision and Recall: 
Precision provides the proportion of positive identifications
that were actually correct, while recall provides the proportion of actual
positives that were identified correctly. These metrics provided insights into the
model's performance across different sizes.

###F1 Score:
 The harmonic mean of precision and recall, providing a single metric for
evaluating the model's accuracy regarding false positives and false negatives.

##Visualization and Insights

The predicted data was visualized to offer intuitive insights into the predicted
size distributions across different categories and seasons. This visualization aids
retail sellers in understanding which sizes are more likely to be in demand, thus
informing their inventory decisions.

##Conclusion and Future Work

The developed RandomForest model serves as a reliable predictor for size demand in
retail clothing. With an accuracy of 83%, it provides actionable insights that can
be leveraged to optimize inventory management. For future work, the model could be
refined with additional data, and other algorithms could be explored to further
improve the predictive performance.

#Instructions to run the supply chain optimization model
## Download csv dataset file from following link:
https://www.kaggle.com/datasets/a23bisola/fashion-dataset-uk-us
## Run firstly CleaningData.iypnb
## Run Random Forest.iypnb
