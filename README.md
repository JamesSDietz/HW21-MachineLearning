# HW21-MachineLearning

Machine Learning using Kepler dataset of exoplanets

James S. Dietz


Findings:

(1) Exoplanetary data originating from NASA were imported and preprocessed which involved creating a matrix of X values 
and a y value which were then split into training and testing sets.

(2) Data were then scaled using the MinMax scaler which projected them into a zero to 1 space.

(3) Scaled data were then used to train and test four machine learning models--(a) Logistic Regression, (b) Support Vector 
Machine classifier, (c) K Nearest Neighbors, and (d) a Neural Network Deep Learning Model.

(4) The Logistic Regression Model demonstrated a Training Data Score of 0.756 compared with a Testing Data Score
of 0.773.  The SVM/SVC Model initially yielded an accuracy score of 0.758 with the Training Data compared to a 
0.780 with Testing Data.  The hyperparameters of the model were then fine-tuned with a GridSearch method which yielded a set of parameters (C=10, gamma=0.001) and a revised accuracy score.  A KNN model was tested which yielded an accuracy score of 0.737 with 10 neighbors used for classification.  Finally, a Neural Network Deep Learning Model was run with two hidden layers of 100 nodes each.  This model was, by far, the best model in terms of prediction using the testing data. It yielded an accuracy of 0.837 suggesting it was over 83 percent accurate in its prediction of whether the object was a false positive or an exoplanet candidate.


Notes:

koi_pdisposition was renamed disposition and recoded, where candidate (which appears to mean confirmed) = (1) and the false positives (disconfirmed) = (0). 

All error columns were deleted as were any non numeric data.

Analysis = kepler.ipynb
Data = kepler.csv