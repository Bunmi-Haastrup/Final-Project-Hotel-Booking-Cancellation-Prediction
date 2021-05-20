## **Final-Project-Hotel-Booking-Cancellation-Prediction**

![alt text](https://github.com/Bunmi-Haastrup/Final-Project-Hotel-Booking-Cancellation-Prediction/blob/main/Visualizations/Portugal%20Map.png)

     
 ## **May 2021**
  
## **Content**

**[Background Information](#ibackground information)**

**[Problem of Solution](#problem of the solution)**

**[Executive Outline](#executive outline)**

**[Objective](#objective)**

**[Workflow](#workflow)**

**[Visualisation](#Visualisation)**

**[Observation and conclusion](#Observation and Conclusion)**

**[Data Dictionary](#data dictionary)**

## **Background Information**
The hotel industry is said to be one of the growing sector of the hospitality sector, most especially with the rise of giant OTA that make booking a hotel as       easy as is ever can been. However, the growth comes with its own challenge, one of the problem is the rising rate of cancellation in the hotel industry, the       cancellation rate grew from under 33% in 2014 to 40% in 2018[source](https://resources.emerchantpay.com/how-hotels-can-combat-rising-cancellation-rates).
The hospitality industry is a highly competitive industry which includes hotels, in order to stay competitive, hotels will have to be on top of their gain to       remain in business. Reflection on what it is they are doing wrong is as important as the business. One of the challenges faced with the hotel industry is Booking cancellations [source](https://www.rateboard.io/en/blog/hotel-cancellations-pose-a-great-challenge).  Booking cancellations are unquestionably one of the biggest headaches of any hotel manager nowadays, it poses a threat of attaining the forecasted revenue and ultimately affect production cost. The free 24-hour free cancellation policy, of course is a strategy to attract customers, however, can be a double-edged sword that equally has a negative effect on their revenue [source](https://www.researchgate.net/publication/310504011_Predicting_Hotel_Booking_Cancellation_to_Decrease_Uncertainty_and_Increase_Revenue).

## **Problem of the Statement**
With the increase in trend of booking cancellation from year to year, nearly 40 percent of hotel bookings is likely to be cancelled prior to arrival with only     few bookings leading to confirmation. The reports states that guests have become accustomed to free cancellation policies that have been made popular ([source].   (https://www.hotelmanagement.net/tech/study-cancelation-rate-at-40-as-otas-push-free-change-policy).This problem poses to have an adverse effect on the hotel's     business forecast, loss in opportunity cost which results to unsold room and automatically affects ROI. 

## **Executive Outline**
The objective of this project is to build a model that will predict a booking as cancelled or not cancelled using classification. To achieve this, we have used a real bookings dataset from City Hotel (Lisbon) and Resort Hotel in (Algarve region) Portugal, the dataset was gotten from[source](https://www.kaggle.com/jessemostipak/hotel-booking-demand). The bookings was scheduled between Ist July, 2015 until 31st August, 2017. The dataset consists of 119,390 observations with 32 variables. Full details in the data dictionary. Cleaning and Wrangling was performed on the dataset to remove all noise with appropriate feature engineering. The EDA process includes analysis of the traget variable which is (cancellation) in relation to the other features, various visualisation tools were deploy to identify trends and extract valuable insights from analysis. Pywedge was used to visualize correlation between variables, the data was afterwards balanced using SMOTE. Three models were used for prediction: logisticRegression, Decisiom Tree and Random Classifier. two accuracy checker was used to check best accuracy score: Confusion Matrix and AUC / ROC curve. The model with the highest test accuracy was selected to gain insights of the factors that most influence cancellations. The model were evaluated, conclusion and recommendations were derived for hotels to predict future inference, optimize production cost, improve forcast and ultimately increase revenue.

## **Objective**
 1.The goal is find out the Type of customer who cancelled and using EDA to understand the pattern of booking cancellation.
 2.To predict the variable that most affect cancellation.
 3.Identifing higher risk of booking cancellations, in order to accept the lower risk bookings.
 4.Building classification Machine learning ,model that best predict cancellations.
 5.Visualizing cancellation with dashboards to best explains the problem and proferring recommendations.
 6.Discover the model with highest accuracy score to predict cancellations.

## **Business Related Questions**
1. How lead time of bookings affects cancellations?
2. What time of the year has the highest bookings and cancellations?
3. Why Type of customer are more likely to cancel the most?
4. Does distance affects cancellations?
5. How much influence does other feautures have on cancellations


 ![alt text](https://github.com/Bunmi-Haastrup/Final-Project-Hotel-Booking-Cancellation-Prediction/blob/main/Visualizations/Workflow.png)

1. **Data Cleaning** :

   Dropping columns that has more than 30% missing values
   Dropping rows with abnormal values
   Total guests / adults in the booking
   Negative daily rate
   Dropping row with outliers that's super different compared to the other row in the columns
   Row with daily rate that's above 5000 euro

2. **Exploratory Data Analysis** :
 
   Feature Engineering
   Aggregating Columns
   Visualization
   Insight & Conclusion
  
3. **Feature Selection for machine learning process**

   Label encoding for certain columns that needs to be encoded
   Feature selection based on EDA
  
4. **Model Building**

  Train Test Split
  Using pipeline for model building
    scaling for numerical features
    label encoder for categorical features
    balancing imbalance data ( target variable) with SMOTE and TomekLinks
  Creating base model with few algorithm (Logistic Regression, Decision Tree Classifier, Random Forest classifier)
  Checking evaluation matrix (Confusion Matrix
  Checking evaluation matrix on the tuned model AUC ROC curve
  Plotting the Top 15 important faetures in the dataset

## **Visualisation**
Insightful dashboards was built with Tableau to effectively envision distinctive  plots such as the distribution plots of different variables (independent and dependent) and creation of a visually appealing dashboard to predict cancellations, understand customer behaviour and how to prevent future cancellations.

**Tableau visualization for this project can be found under this link**; 

[tableau link](https://public.tableau.com/profile/olubunmi.abimbola.haastrup#!/vizhome/InProgress_16213358728240/TotalofBookingsperspecialrequest?publish=yes)

![alt text](https://github.com/Bunmi-Haastrup/Hermione-granger/blob/main/visualization.png)

# **Observation Conclusion**
Logistic Regression, Decsion Tree and Radom Claasifier was the models adopted in solving the hotel booking classification. 735 accuracy score was identifed with Logistic regression, Decison tree identifed an accuracy score of 85% while Random Tree Classifier was 84%. As a result, I will therefore conclude that either Decision Tree and Random Forest Classifier can be considered for hotels to achieve a more accurate forecast of their booking confirmation which will better improve their return on investment(ROI). Although every model has its own shortcoming, can surfix in cutting down on cancellation rate. This will also help hotel managers to understand customer behaviour, which customer has better bookings confirmation and understand how fast a booking should be confirmed to avoid cancellations.


**Data Dictionary*+
