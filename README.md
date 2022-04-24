# About
This is a mini project for SC1015 (Introduction to Data Science and Artificial Intelligence) which uses weather conditions taken from [Wunderground](https://www.wunderground.com/weather/WSSS "Wunderground"). We focused on the Changi Airport Station dataset, as it contained the most datapoints for us to work with.

You can follow our project using the slides provided [here](https://docs.google.com/presentation/d/1KrQD1V2QRjoReH4YOghomfbqK7u-ulyihedcrom0Euk/edit?usp=sharing "Presentation")

# Problem Definition
With the easing of Covid restrictions, more tourists will be visiting Singapore. However, bad weather can disrupt our outdoor plans, and this is more so for tourists who might not be familiar with the tropical climate of Singapore. Hence, we would like to determine whether one should bring an umbrella outside by predicting the weather condition given past meteorological data, which can be displayed in information kiosk systems around the airport, and maybe even hotels.

# Data Cleaning
* Missing numerical data was filled with the mean, while categorical data was filled with the previous data point
* Analyzed whether data was stationary using ADF Test
* Dropped irrelevant features
* Converted dataset to time-series

# Handling Imbalanced Data
* Grouping similar classes together
* Experimented with sample weights, SMOTE and resampling

# Models used in order of performance
1. Gradient Boosting Trees
2. LSTM
3. Support Vector Machines with the Radial Basis Function (RBF) kernel

# Other models we experimented with
* Support Vector Machines with the linear kernel
* Multi-layer Perceptron Classifier
* Balanced Bagging Classifier
* Logistic Regression

# Conclusion
* Resampling imbalanced data improved model performance especially on the minority class
* Logistic Regression did not perform well with non-linearly correlated variables
* Gradient Boosting Trees performed the best in classifying the weather conditions, as they are able to learn complex problems much better than classification techniques utilising linear or radial kernal functions
* Traditional Machine Learning methods can perform with similiar performance to simple deep learning models with sufficient tuning of hyperparameters and data augmentation

# Lessons Learnt
* Handling imbalanced datasets using resampling methods and imblearn package
* Handliing Time-Series Datasets with concepts such as 
* Keras and Tensorflow
* Logistic Regression, SVM, Gradient Boosting Trees, MLP and Balanced Bagging from sklearn
* Tuning Hyperparameters
* Concepts about Precision, Recall, and F1 Score

# Future Works
* Classify whether conditions on degree of urgency (e.g. “Highly Recommended”, "Slightly Recommended", “Not Recommended” etc.)
* Include macroweather features (long term flucuations of temperature, rainfall etc.) to train better models
* Utilise PyTorch module to build LSTM model for more control over hyperparameters and model architecture.

# Contributors
Kenny - Data Extraction, Slides, Video  
Wei Xian - EDA, Slides, Video  
[Ming En](https://github.com/MingEn82 "Github") - EDA, Model Architecture, Data Visualization, Data Analysis 

# Resources Used
* https://machinelearningmastery.com/time-series-forecasting/
* https://towardsdatascience.com/stationarity-in-time-series-analysis-90c94f27322
* https://scikit-learn.org/stable/
* https://www.tensorflow.org/api_docs/python/tf/keras/
* https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2015GL065665
