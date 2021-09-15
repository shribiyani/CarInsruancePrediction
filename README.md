# Car Insruance Prediction


As world is moving towards fast and luxuries life. Every individual want to have a car for their short trip with family. Unfortunately, if your car got crashed or meet with an accident, it may bring financial stress on individual and incurred loss in hand of a person, who crashed upon other car. 

In this kind of situation  **Third Party Insurance** is required to minimize loss of accident. Even if vehicle is **Lossed due to Robery** or even if any **Loss due to Natural Calamities**, to cover all these losses an individual requires **`An Insurance`** to protect financial losses from uncertain events. So every individual have an **Car Insurance**.

**Car insurance** offers protection against accidents, theft, natural calamities & other unforeseen circumstances that could harm your car. Having a good car insurance policy ensures that you and your car are protected from the financial losses of these unfortunate events.


## Purpose 

As you are a **Data Scientist** at a bank and your Bank started car insurance service besides usual banking services. The bank has potential customers data and bank employees call them for advertising and give brife information regarding available car insurance policy. So existing customer might get insterested to purchase car insurance.

Currently Bank is running an **Insurance Sell Campaign** with reference to customers details information.

We have data about 3100 customers who **contacted during the last campaign** and for whom the results of the campaign (if the customer bought insurance or not) are known.


So our purpose of this study is - **too Predict a Car Insurance Sell** on the basis of contacted customers.


###  About the Data

There are 19 variables (including the target variable) in the train dataset. Below are some of the listed variables and their description:


- **age** : age of the customer

- **job_type** : what job does customer do

- **marital_status** : if the customer is married or not

- **education_level** : education level of the customer

- **default_or_not** : if the customer was able to repay in time or not

- **balance_amt** : balance amount of the customer in the bank

- **hoursehold_insurance** : if the customer has bought household insurance or not

- **car_loan** : if the customer has car loan

- **communication** : mode of communication

- **last_contact_day** : when the customer was last contacted (day)

- **last_contact_month** : when the customer was last contacted (month)

- **no_of_contacts** : How many times was the customer contacted in the current campaign

- **days_passed** : days passed since the last contact (-1 means the data is missing)

- **prev_attempts** : how many times was the customer previously contacted (i.e. in the campaigns befor this) 

- **outcome** : what was the outcome of the last contact

- **call_start** : call start time

- **call_end** : call end time

- **car_insurance** : if the customer bought car insurance (the **target variable**, 1 - **Boutght**, 0 - **Not-Bought**)


#### **Brief About Data** 

1. Target variable is **Binary Classification**.
2. Data is devided into **Train** and **Test** with rows of 3102 and 935 and 18 independent features.
3. Brief Analysis from Data Visualization -
   - Target variable distribution looks **around 60:40 ratio**
   - Customers who are married are having higher chances getting **Car Insurance**.
   - If Car insurance are sold, around 98% customers will pay premium on time and they have high chances to have car insurance.
   - Those who has car insurance they will buy car insurance but even those don't have car insurance, if they have car, they will also buy insurance.



Here I have tried Logistic Regression, SVC, Random Forest Classifier, Ada Boost Classifier, Gradient Boosting Classifier, Decision Tree Classifier, XGB Classifier, CatBoost Classifier. Out off these models **AdaBoost Classifier** with **Random Forest Classifier** as base estimator gives **approx. 70% Accuracy Score**.
