# Delaney-Solubility_
My first ML project! Used the Delaney Solubility dataset with Linear Regression and Random Forest models to make predictions. 
This project demonstrates a simple machine learning workflow to predict the solubility of molecules based on their molecular descriptors.

Dataset:

The dataset used in this project is the Delaney Solubility dataset, which contains experimental solubility data (logS) and calculated molecular descriptors (MolLogP, MolWt, NumRotatableBonds, AromaticProportion) for a variety of molecules.

The dataset is loaded from the following URL: https://raw.githubusercontent.com/dataprofessor/data/refs/heads/master/delaney_solubility_with_descriptors.csv

Data Preparation:

The data was split into features (X) and target (y), where y is the logS column and X includes the remaining molecular descriptors. The data was then split into training and testing sets using a 80/20 split with a random_state of 100.

Model Building:

Two regression models were built and evaluated:
Linear Regression: A simple linear regression model was trained on the training data.

Random Forest: A Random Forest Regressor model with a max_depth of 2 and random_state of 100 was trained on the training data.

The models were evaluated using Mean Squared Error (MSE) and R-squared (R2) metrics on both the training and testing sets.

Results:
The performance of the models is summarized in the following table:

<img width="543" height="95" alt="Screenshot 2025-08-08 at 2 52 32 PM" src="https://github.com/user-attachments/assets/5e739ee7-d22d-47cb-b8e3-f691b90cc751" />

Based on these results, the Linear Regression model performed slightly better on the testing set with a lower MSE and higher R2 score.

Data Visualization:

A scatter plot is generated to visualize the relationship between the experimental and predicted logS values for the Linear Regression model on the training data. A regression line is also plotted to show the trend.

<img width="464" height="449" alt="Screenshot 2025-08-08 at 2 52 21 PM" src="https://github.com/user-attachments/assets/694994ed-7cec-46cb-95fb-281d612607d7" />

