# About
This is a mini project for SC1015 (Introduction to Data Science and Artificial Intelligence) which uses weather conditions taken from [Wunderground](https://www.wunderground.com/weather/WSSS "Wunderground"). We focused on the Changi Airport Station dataset, as it contained the most datapoints for us to work with.

# Contributors
Kenny - Data Extraction, Slides, Video  
Wei Xian - EDA, Slides, Video  
[Ming En](https://github.com/MingEn82 "Github") - Model Architecture, Data Visualization, Data Analysis 

# Problem Definition
We would like to determine whether one should bring an umbrella outside by predicting the weather condition given past data.

# Models used in order of performance
1. Gradient Boosting Trees
2. LSTM
3. Support Vector Machines with the Radial Basis Function (RBF) kernel
4. Logistic Regression

# Models we experimented with
1. Support Vector Machines with the linear kernel
2. Multi-layer Perceptron Classifier
3. Balanced Bagging Classifier

# Conclusion
* Resampling imbalanced data improved model performance especially on the minority class
* Logistic Regression did not perform well with non-linearly correlated variables
* Neural Networks along with SMOTE resampling method consistently did well in predicting whether an umbrella is needed (86% recall for Yes, 96% recall for No)
* Traditional Machine Learning methods performed at the same level as deep learning models with sufficient tuning of hyperparameters

# Lessons Learnt
* Handling imbalanced datasets using resampling methods and imblearn package
* Handliing Time-Series Datasets with concepts such as 
* Keras and Tensorflow
* Logistic Regression, SVM, Gradient Boosting Trees, MLP and Balanced Bagging from sklearn
* Tuning Hyperparameters
* Concepts about Precision, Recall, and F1 Score

# Resources Used
* https://machinelearningmastery.com/time-series-forecasting/
* https://towardsdatascience.com/stationarity-in-time-series-analysis-90c94f27322
* https://scikit-learn.org/stable/
* https://www.tensorflow.org/api_docs/python/tf/keras/
