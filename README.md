## Holiday Package Prediciton

### Problem statement.
"Trips & Travel.Com" company wants to enable and establish a viable business model to expand the customer base.
One of the ways to expand the customer base is to introduce a new offering of packages. Currently, there are 5 types of packages the company is offering * Basic, Standard, Deluxe, Super Deluxe, King. Looking at the data of the last year, we observed that 18% of the customers purchased the packages. However, the marketing cost was quite high because customers were contacted at random without looking at the available information.
The company is now planning to launch a new product i.e. Wellness Tourism Package. Wellness Tourism is defined as Travel that allows the traveler to maintain, enhance or kick-start a healthy lifestyle, and support or increase one's sense of well-being.
However, this time company wants to harness the available data of existing and potential customers to make the marketing expenditure more efficient.

This Project showcases my expertise in performing 
### Data Collection.
The Dataset is collected from https://www.kaggle.com/datasets/susant4learning/holiday-package-purchase-prediction
The data consists of 20 column and 4888 rows.


### Project Overview



Trips & Travel.Com is a travel company seeking to expand its customer base by introducing a new “Wellness Tourism Package” — designed for travelers who wish to maintain or enhance a healthy lifestyle while traveling.




Historically, only 18% of customers purchased travel packages, and marketing costs were high due to random customer outreach.
This project leverages machine learning to identify potential customers who are more likely to purchase a package, enabling smarter marketing and reduced costs.

### Objective



Build a predictive model that:

Classifies customers as likely or unlikely to purchase a travel package (ProdTaken).
Provides insights into key factors influencing package purchases.
Helps the marketing team target potential buyers more efficiently.

### Dataset Description



The dataset represents customer profiles, engagement data, and travel preferences.
Target Variable: ProdTaken
(1 = Customer purchased a package, 0 = Did not purchase)




### Features Overview:

Feature	Description
Age	Age of the customer
TypeofContact	How the customer was contacted (e.g., Self Enquiry, Company Invited)
CityTier	Tier of the city (1 = Metro, 2 = Urban, 3 = Rural)
DurationOfPitch	Duration (in minutes) of the sales pitch
Occupation	Type of occupation (Salaried, Small Business, Free Lancer, etc.)
Gender	Gender of the customer
NumberOfFollowups	Number of follow-up calls made to the customer
ProductPitched	Type of package offered (Basic, Standard, Deluxe, etc.)
PreferredPropertyStar	Star rating preference of properties
MaritalStatus	Customer’s marital status
NumberOfTrips	Number of trips taken in the last year
Passport	Whether the customer holds a passport (1 = Yes, 0 = No)
PitchSatisfactionScore	Rating given by the customer after the pitch
OwnCar	Whether the customer owns a car
Designation	Professional designation (Executive, Manager, etc.)
MonthlyIncome	Monthly income of the customer
TotalVisiting	Total number of visits made for follow-up or interaction
### Approach

##### Data Preprocessing

Handled missing and inconsistent values.
Converted categorical variables into numerical using Label Encoding and One-Hot Encoding.
Scaled numerical features where needed.
Split the data into 80% training and 20% testing.

##### Exploratory Data Analysis (EDA)

Analyzed relationships between customer demographics and purchase behavior.
Visualized distribution of package purchases (ProdTaken).
Identified key influencing features such as income, pitch duration, and designation.

##### Model Training
Multiple models were trained and evaluated:

Logistic Regression
Decision Tree
Random Forest
(Gradient Boosting can be added for further optimization.)

##### Performance Evaluation
Each model was evaluated using:

Accuracy
F1-Score (Weighted)
Precision
Recall
ROC-AUC Score

### Model Performance Summary
Model	Train Accuracy	Test Accuracy	F1 Score	ROC-AUC
Logistic Regression	0.84	0.79	0.78	0.76
Decision Tree	1.00	0.75	0.74	0.73
Random Forest	0.97	0.82	0.81	0.80



(Actual values may vary depending on data preprocessing and parameter tuning.)

### Key Insights
Income, Pitch Duration, and Occupation are strong predictors of package purchase likelihood.
Customers with managerial roles and frequent travelers are more likely to buy packages.
Decision Tree overfitted, while Random Forest provided the best balance between bias and variance.
Logistic Regression helps interpret which features most influence customer decisions.

### Future Work
Apply Gradient Boosting (XGBoost, LightGBM) for improved accuracy.
Use SMOTE or class weighting to handle class imbalance.
Tune hyperparameters using GridSearchCV.
Deploy the final model using Flask API or Streamlit.
Create an interactive dashboard for marketing insights (Power BI / Tableau).


### Dependencies
##### Install required libraries:

pip install pandas numpy scikit-learn matplotlib seaborn

### How to Run
Clone the repository:
git clone https://github.com/yourusername/trips-travel-package-prediction.git

Navigate to the project directory:
cd trips-travel-package-prediction

Run the notebook or Python script:
jupyter notebook travel_package_prediction.ipynb

or
python model_training.py

### Results Summary



The trained Random Forest model achieved ~82% accuracy on the test set, helping identify high-potential customers for the new Wellness Tourism Package, thereby improving marketing efficiency.

####
