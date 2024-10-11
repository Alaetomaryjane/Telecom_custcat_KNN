# Telecom Customer Communication


### Machine learning and Python 

### TITLE: Telecom Service Prediction

### AIM: The aim of this project is to use demographic data like age, region and marital status to predict which service group a new or unknown customer belongs to .

#### DATA DESCRIPTION: This dataset from IBM's Cloud Object Storage service contains customer records from a telecommunication company, with demographic and service related attributes.\
- Data source: https://s3-api.us-geo.objectstorage.softlayer.net/cf-courses-data/CognitiveClass/ML0101ENv3/labs/teleCust1000t.csv
- Total Samples: 1000 customer records
- Number of features: There are 12 features (including the target variables ‘custcat’)

#### FEATURE:
- region: The geographical region the customer is from, encoded as integers.
- tenure: The number of years the customer has been using the service.
- age: The age of the customer.
- marital: Marital status of the customer, represented as categorical values.
- address: Number of years the customer has lived at their current address.
- income: The customer’s annual income.
- ed: The education level of the customer, encoded as integers.
- employ: Number of years the customer has been employed.
- retire: Binary variable indicating whether the customer is retired (1) or not (0).
- gender: Gender of the customer, encoded as integers (e.g., 0 for male, 1 for female).
- reside: Number of years the customer has lived in their current residence.
- custcat (Target Variable): The customer category, with values ranging from 1 to 4, representing different customer segments (Basic, E-Service, Plus, Total Service).

#### Development Process: 
- Data loading and preparation: Libraries such as Pandas, NumPy (for data manipulation), matplotlib.pyplot (for visualization), sklearn.preprocessing (for machine learning preprocessing), and %matplotlib inline (for notebook display) are imported.
- Data Visualization and Analysis: To streamline the analysis, an irrelevant column was removed from the dataset. The income distribution was then examined, revealing that the majority of customers fall into lower income brackets, indicating a skewed distribution across the customer base.
- Data Preprocessing: The predictor and target variables were defined, followed by feature scaling using StandardScaler to normalize the data and ensure all features are on a consistent scale.
- Model Development: Using the train_test_split function from sklearn.model_selection, the features were split into training and testing sets. The K-Nearest Neighbors (KNN) classifier was then applied for model development.
- Model Accuracy: The model's accuracy was assessed using the accuracy_score function from the metrics module in sklearn.
#### Evaluation Result:
##### Model Accuracy Scores:
- Train Set Accuracy: 50.25%
- Test Set Accuracy (yhat, yhat1, yhat2): 32%, 31%, and 34%, respectively.

#### Conclusion:
In this project, we used the K-Nearest Neighbors (KNN) algorithm to classify customer categories. The evaluation showed that while the training accuracy was 50.25%, the model’s test accuracy ranged from 31% to 34%. This indicates potential overfitting, meaning the model may perform well on the training data but struggles to generalize to new, unseen data.

![image](https://github.com/user-attachments/assets/3a0e44ce-e8b0-4a93-819d-dfd9e29ab8e3)
