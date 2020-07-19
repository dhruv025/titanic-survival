# titanic-survival-prediction

In this project, our task is to create a machine learning model on the Titanic Dataset which predicts whether a passenger on the titanic would have been survived or not. Some of the classification algorithms have been used, out of which RandomForestClassifier gives the best result.

Major Steps followed during the project -
1. Data Gathering – Dataset has been downloaded from kaggle. The dataset consist of 891 rows and 12 columns.

2. Feature Engineering – In this, first of all I have checked for the missing values in the dataset if any. Since, Age feature has 177 missing values. So,
I have used fillna() method to fill the missing values.
Also, done exploratory data analysis to analyze the data with the help of seaborn library which is used for data visualization from which I came to know that the count of no. of males is more than no. of females who have not survived.
Now, handling some categorical values, there are two types of categorical values which are as follows:
a. Nominal data → data is not in any order.
b. Ordinal data → data is in order.

Since, we have two categorical features and both of them lie under the nominal data. So, I have used one hot encoding to convert them into numerical values.
Since, our machine learning model will only able to understand numbers and give better performance.

Now, our dataset is ready for applying to any machine learning algorithm.

3. Model Training – In this first of all, I have divide the dataset into train and test using the train_test_split method of sklearn.
For training the dataset, I have used various classification algorithms KneighborsClassifier, DecisionTree , SupportVector and RandomForest. Out of these four algorithms, Random Forest gives a result of accuracy 83.52 %.

Since, only accuracy doesn’t tells that how good our model is. So, we have to calculate other performance metrics such as precision, recall, support. These performance metrics can be calculated with the help of classification report.
A classification report is used to measure the quality of predictions from a classification algorithm.
