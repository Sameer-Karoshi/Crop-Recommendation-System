# Crop-Recommendation-System

Crop Selection has become very important. It is crucial to identify crops that go well with the weather and atmosphere of the land. It is also important to take into consideration the nutrients and chemicals present in the soil before planting the crops. This method takes into consideration all these parameters and suggests the optimal crop . The system takes input of Nitrogen, Phosphorus, Potassium and pH level of the soil along with Temperature, Humidity and Rainfall in the region.

Dataset: The dataset is in the form of a csv file. The dataset consists of 7 parameters namely - Nitrogen level, Phosphorus level, Potassium level, Temperature ,Rainfall in the region ,pH level of soil and humidity. Total 22 crops are included in the database along with the levels of the above-mentioned parameters for each of these crops. In totality 100 data points of each of these crops are included in the dataset. Therefore, there are 2200 different data points in the dataset. The null values in the dataset are removed. For each of the 100 data-points of each crop the average of each parameter is calculated. So for each crop an optimal level of each parameter is obtained which is most suitable for the respective crop. Supervised Learning algorithms are used for suggestion of the crop. The data is split into 80:20 test train ratio. The model is trained using four supervised learning algorithms such as Logistic Regression, K-Nearest Neighbor, Decision Tree , Random Forest.

## Flowchart of Crop Recommendation System
![alt text](https://github.com/Sameer-Karoshi/Crop-Recommendation-System/blob/main/Crop%20Recommendation%20System.png)

It is observed that Random Forest algorithm was the most efficient. The flow of Random Forest algorithm is shown below figure. It is a classifier consisting of many decision trees on different subsets of a dataset and takes a voting (average) to improve the accuracy. Higher accuracy is achieved by a greater number of decision trees and addresses the problem of overfitting.

![alt text](https://github.com/Sameer-Karoshi/eFarma/blob/master/Crop%20Recommendation%20using%20RF.PNG)

## A. Data Visualization

1. Imported required libraries like pandas, numpy and matplotlib.NumPy is a Python library used for working with arrays and pandas is used for data science/data analysis and machine learning tasks.Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python.
2. Firstly the dataset is loaded from Gdrive in csv format. 
3. Then check if there are null values present or not. (Since we already removed null values there are no null values present :)).
4. Using describe() function we can get the details about the data like mean count of rows and all.

![alt text](https://github.com/Sameer-Karoshi/Crop-Recommendation-System/blob/main/Statistics.PNG)

5. Then average values(Nitrogen, Phosphorus…) of different crops calculated and plotted a bar plot.

![alt text](https://github.com/Sameer-Karoshi/Crop-Recommendation-System/blob/main/Average%20Values%20of%20Diffrent%20Crops.PNG)

6. Here, we plotted a scatterplot for different crops(temperature / Rainfall). 

![alt text](https://github.com/Sameer-Karoshi/Crop-Recommendation-System/blob/main/ScatterPlot%20of%20Different%20Crops(Temp%20Vs%20Rainfall).PNG)

1. Imported all required libraries. The sklearn library contains a lot of efficient tools for machine learning and statistical modeling including classification, regression, clustering and dimensionality reduction.
2. Then we find correlation between parameters using corr() function.Correlation explains how one or more variables are related to each other.

![alt text](https://github.com/Sameer-Karoshi/Crop-Recommendation-System/blob/main/Correlation.PNG)
3. There are basically 7 input parameters that are features and one output parameter that is label. (This is supervised machine learning so a pair of input & output is always required :) ).

![alt text](https://github.com/Sameer-Karoshi/Crop-Recommendation-System/blob/main/Features%20and%20Label.PNG)

4. After this we divided the data into train and test data(80% and 20%).

![alt text](https://github.com/Sameer-Karoshi/Crop-Recommendation-System/blob/main/Train%20%26%20Test.PNG)

5. Then tried different supervised  algorithms like KNN, Logistic Regression, Decision Tree and Random forest.

![alt text](https://github.com/Sameer-Karoshi/Crop-Recommendation-System/blob/main/Algorithms.PNG)

Here we can see that amongst these four algorithms random forest works pretty well and gives highest accuracy also that is 99%.
6. Last step is cross validation and then saving the model.  

![alt text](https://github.com/Sameer-Karoshi/Crop-Recommendation-System/blob/main/Cross%20Validation%20%26%20saving%20the%20model.PNG)

## Results:

![alt text](https://github.com/Sameer-Karoshi/Crop-Recommendation-System/blob/main/Results.PNG)
 
