# Credit Card Fraud Detection - Data Science Project

The main reason for analyzing this dataset is to get a trained model that can detect whether a transaction is a fraud or not.

The first thing that I had to take in consideration was the Exploratory Data Analysis, as this is not an explicit dataset. Then, once I examined the data, I saw
the behavior of the values of the transaction columns and I figured it out that the transaction movements classified as "healthy" (in blue) are almost opposite to those
classified as "fraud" (in red). In the following graph we can notice what has being said previously:

![_figure 1: Behavior_](https://github.com/Camiloalejan/CreditCardFraudDetection_DataScienceProject/blob/main/images/values.png)

After, I took the Amounts of each row, and I decided to compare them through the time. We can clearly see, that the healthy movements, used to be greater than those fraudulents
as it is shown below:

![_figure 2: Amounts_](https://github.com/Camiloalejan/CreditCardFraudDetection_DataScienceProject/blob/main/images/amounts.png)

Here we have a qualitative data set, due to the "Class" column that indicates whether a completed transaction is a fraud or not. Therefore, the best models to complete 
the main task are the algorithms that are used to classify. So I chose the K-Nearest-Neighbors (K-Neighbors-Classifier) and Random Forest Machine Learning models 
for this case.

Once I trained the models, we could clearly see that the Random Forest had a better performance. As it is shown in the confusion Matrix below:

![_figure 3: Confusion Matrix_](https://github.com/Camiloalejan/CreditCardFraudDetection_DataScienceProject/blob/main/images/confusion%20matrix.png)

Finally, I decided to train the model once again, but this time manipulating the parameters and I got this ROC curve with a high value of AUC, as we can note in the
next figure:

![_figure 4: ROC_](https://github.com/Camiloalejan/CreditCardFraudDetection_DataScienceProject/blob/main/images/ROC.png)
