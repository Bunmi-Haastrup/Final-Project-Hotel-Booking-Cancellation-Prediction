# **Final-Project-Hotel-Booking-Cancellation-Prediction**

![alt text](https://github.com/Bunmi-Haastrup/Hermione-granger/blob/main/image.png)

     𝒫𝒾𝒸𝓉𝓊𝓇𝑒 𝓈𝑜𝓊𝓇𝒸𝑒:𝐿𝒶𝓃𝑔𝒶𝓃.𝒸𝑜𝓂, 𝑀𝒶𝓅 𝓈𝑜𝓊𝓇𝒸𝑒: 𝐻𝑒𝓇𝓂𝒾𝑜𝓃𝑒-𝑔𝓇𝒶𝓃𝑔𝑒𝓇
     
  ## **May 2021**
  
# **Content**
[Background Information](#ibackground information)

[Problem of Solution](#problem of the solution)

[Executive Outline](#executive outline)

[Variables-description](#variables-description)

[Data](#data)

[Database](#database)

[Visualisation](#visualisation)

[Statistical Analysis](#statistical-analysis)

[Conclusion](#conclusion)

## **Background Information**
The hotel industry is said to be one of the growing sector of the hospitality sector, most especially with the rise of giant OTA that make booking a hotel as       easy as is ever can been. However, the growth comes with its own challenge, one of the problem is the rising rate of cancellation in the hotel industry, the       cancellation rate grew from under 33% in 2014 to 40% in 2018[source](https://resources.emerchantpay.com/how-hotels-can-combat-rising-cancellation-rates).
The hospitality industry is a highly competitive industry which includes hotels, in order to stay competitive, hotels will have to be on top of their gain to       remain in business. Reflection on what it is they are doing wrong is as important as the business. One of the challenges faced with the hotel industry is Booking cancellations [source](https://www.rateboard.io/en/blog/hotel-cancellations-pose-a-great-challenge).  Booking cancellations are unquestionably one of the biggest headaches of any hotel manager nowadays, it poses a threat of attaining the forecasted revenue and ultimately affect production cost. The free 24-hour free cancellation policy, of course is a strategy to attract customers, however, can be a double-edged sword that equally has a negative effect on their revenue [source](https://www.researchgate.net/publication/310504011_Predicting_Hotel_Booking_Cancellation_to_Decrease_Uncertainty_and_Increase_Revenue).

#link to Map

## Problem of the Statement
With the increase in trend of booking cancellation from year to year, nearly 40 percent of hotel bookings is likely to be cancelled prior to arrival with only     few bookings leading to confirmation. The reports states that guests have become accustomed to free cancellation policies that have been made popular ([source].   (https://www.hotelmanagement.net/tech/study-cancelation-rate-at-40-as-otas-push-free-change-policy).This problem poses to have an adverse effect on the hotel's     business forecast, loss in opportunity cost which results to unsold room and automatically affects ROI. 

## Executive Outline
The objective of this project is to build a model that will predict a booking as cancelled or not cancelled using classification. To achieve this, we have used a real bookings dataset from City Hotel (Lisbon) and Resort Hotel in (Algarve region) Portugal, the dataset was gotten from[source](https://www.kaggle.com/jessemostipak/hotel-booking-demand). The bookings was scheduled between Ist July, 2015 until 31st August, 2017. The dataset consists of 119,390 observations with 32 variables. Full details in the data dictionary. Cleaning and Wrangling was performed on the dataset to remove all noise with appropriate feature engineering. The EDA process includes analysis of the traget variable which is (cancellation) in relation to the other features, various visualisation tools were deploy to identify trends and extract valuable insights from analysis. Pywedge was used to visualize correlation between variables, the data was afterwards balanced using SMOTE. Three models were used for prediction: logisticRegression, Decisiom Tree and Random Classifier. two accuracy checker was used to check best accuracy score: Confusion Matrix and AUC / ROC curve. The model with the highest test accuracy was selected to gain insights of the factors that most influence cancellations. The model were evaluated, conclusion and recommendations were derived for hotels to predict future inference, optimize production cost, improve forcast and ultimately increase revenue.

![alt text](https://github.com/Bunmi-Haastrup/Hermione-granger/blob/main/image-2.png)

# Objective
* The goal is find out the Type of customer who cancelled and using EDA to understand the pattern of booking cancellation.
* To predict the variable that most affect cancellation.
* Identifing higher risk of booking cancellations, in order to accept the lower risk bookings.
* Building classification Machine learning ,model that best predict cancellations.
* Visualizing cancellation with dashboards to best explains the problem and proferring recommendations.
* Discover the model with highest accuracy score to predict cancellations.

## Questions
* How lead time of bookings affects cancellations?
* What time of the year has the highest bookings and cancellations?
* Why Type of customer are more likely to cancel the most?
* Does distance affects cancellations?
* How much influence does other feautures have on cancellations

# picture workflow

1. Data Cleaning :

  * Dropping columns that has more than 30% missing values
  * Dropping rows with abnormal values
  * Total guests / adults in the booking
  * negative daily rate
  * Dropping row with outliers that's super different compared to the other row in the columns
  * Row with daily rate that's above 5000 euro

2. Exploratory Data Analysis :
 
  * Feature Engineering
  * Aggregating Columns
  * Visualization
  * Insight & Conclusion
  
3. Feature Selection for machine learning process

  * Label encoding for certain columns that needs to be encoded
  * Feature selection based on EDA
  
4. Model Building

  * Train Test Split
  * Using pipeline for model building
    * scaling for numerical features
    * label encoder for categorical features
    * balancing imbalance data ( target variable) with SMOTE and TomekLinks
  * Creating base model with few algorithm (Logistic Regression, Decision Tree Classifier, Random Forest classifier)
  * Checking evaluation matrix (Confusion Matrix
  * checking evaluation matrix on the tuned model AUC ROC curve
  * Plotting the Top 15 important faetures in the dataset


# Variables-description
Id: Unique identification number for the property.

date: the date the house was sold.

price: the price of the house.

waterfront: the house which has a view to a waterfront.

condition: How good the condition is (Overall). 1 indicates worn-out property and 5 excellent.

grade: Overall grade given to the housing unit, based on the King County grading system. 1 poor, 13 excellent.

Sqft_above: square footage of house apart from the basement.

Sqft_living15: Living room area in 2015(implies-- some renovations) This might or might not have affected the lotSize area.

Sqft_lot15: lotSize area in 2015(implies-- some renovations).

# Visualisation
Insightful dashboards was built with Tableau to effectively envision distinctive  plots such as the distribution plots of different variables (independent and dependent) and creation of a visually appealing dashboard to predict cancellations, understand customer behaviour and how to prevent future cancellations.

Tableau visualization for this project can be found under this link; 

https://public.tableau.com/profile/olubunmi.abimbola.haastrup#!/vizhome/MidProjectworkongoing/Dashboard4?publish=yes

![alt text](https://github.com/Bunmi-Haastrup/Hermione-granger/blob/main/visualization.png)

# Statistical Analysis
Under this stage we described the nature of the data to be analyzed, the given data were explored, the model to summarize understanding of how the data relates to the underlying dependent variable was created. This includes proving or disprove the validity of the model and lastly was to employ predictive analytics to anticipate future trends.

# Conclusion
Python was used to clean and sent out a few datasets. Utilizing the data at that point built a machine learning and use MySQL to meet our numerous objectives. As the data given was moderately straight forward, we had parcels of time to test with the visualisations in Scene through the use of Tableau , making a collection of outwardly engaging dashboards that offer curiously understanding.

here are techniques, like those outlined above, that you can use to control cancellation rates and recover from high cancellation rates.

the perfect time for the industry to start investing in this area and particularly in machine learning, since the advantages are huge in all fields of hospitality. Not only in predicting cancellations, but using regression analysis to forecast revenue and costs, cluster their clients on similar behaviors for marketing campaign or many other techniques.


Data Dictionary

Feature Name	Type	Description
ADR	Float	Average Daily Rate. Calculated by dividing the sum of all lodging transactions by the total number of staying nights.
Adults	Integer	Number of adults.
Agent	Categorical	ID of the travel agency that made the booking.
ArrivalDateDayOfMonth	Integer	Day of the month of the arrival date.
ArrivalDateMonth	Categorical	Month of arrival date with 12 categories: “January” to “December”.
ArrivalDateWeekNumber	Integer	Week number of the arrival date.
ArrivalDateYear	Integer	Year of arrival date.
AssignedRoomType	Categorical	Code for the type of room assigned to the booking. Sometimes the assigned room type differs from the reserved room type due to hotel operation reasons (e.g. overbooking) or by customer request. Code is presented instead of designation for anonymity reasons.
Babies	Integer	Number of babies.
BookingChanges	Integer	Number of changes/amendments made to the booking from the moment the booking was entered on the Property Management System until the moment of check-in or cancellation. Calculated by adding the number of unique iterations that change some of the booking attributes, namely: persons, arrival date, nights, reserved room type or meal.
Children	Integer	Number of children. Sum of both payable and non-payable children.
Company	Categorical	ID of the company/entity that made the booking or responsible for paying the booking. ID is presented instead of designation for anonymity reasons.
Country	Categorical	Country of origin. Categories are represented in the International Standards Organization (ISO) 3155–3:2013 format.
CustomerType	Categorical	Type of booking, assuming one of four categories: Contract (when the booking has an allotment or other type of contract associated to it), Group (when the booking is associated to a group), Transient (when the booking is not part of a group or contract, and is not associated to other transient booking), and Transient-party (when the booking is transient, but is associated to at least other transient booking).
DaysInWaitingList	Integer	Number of days the booking was in the waiting list before it was confirmed to the customer. Calculated by subtracting the date the booking was confirmed to the customer from the date the booking entered on the Property Management System.
DepositType	Categorical	Indication on if the customer made a deposit to guarantee the booking. This variable can assume three categories: No Deposit (no deposit was made), Non Refund (a deposit was made in the value of the total stay cost), and Refundable (a deposit was made with a value under the total cost of stay). Value calculated based on the payments identified for the booking in the transaction (TR) table before the booking׳s arrival or cancellation date. In case no payments were found the value is “No Deposit”. If the payment was equal or exceeded the total cost of stay, the value is set as “Non Refund”. Otherwise the value is set as “Refundable”.
DistributionChannel	Categorical	Booking distribution channel. The term “TA” means “Travel Agents” and “TO” means “Tour Operators”.
IsCanceled	Integer	Value indicating if the booking was canceled (1) or not (0).
IsRepeatedGuest	Integer	Value indicating if the booking name was from a repeated guest (1) or not (0). Variable created by verifying if a profile was associated with the booking customer. If so, and if the customer profile creation date was prior to the creation date for the booking on the Property Management System database it was assumed the booking was from a repeated guest.
LeadTime	Integer	Number of days that elapsed between the entering date of the booking into the Property Management System and the arrival date. Calculated by subtracting the entering date from the arrival date.
MarketSegment	Categotical	Market segment designation. In categories, the term “TA” means “Travel Agents” and “TO” means “Tour Operators”.
Meals	Categorical	Type of meal booked. Categories are presented in standard hospitality meal packages: Undefined/SC (no meal package), BB (Bed & Breakfast), HB (Half board: breakfast and one other meal – usually dinner), and FB (Full board: breakfast, lunch and dinner).
PreviousBookingsNotCanceled	Integer	Number of previous bookings not canceled by the customer prior to the current booking. In case there was no customer profile associated with the booking, the value is set to 0. Otherwise, the value is the number of bookings with the same customer profile created before the current booking and not canceled.
PreviousCancellations	Integer	Number of previous bookings that were canceled by the customer prior to the current booking. In case there was no customer profile associated with the booking, the value is set to 0. Otherwise, the value is the number of bookings with the same customer profile created before the current booking and canceled.
RequiredCarParkingSpaces	Integer	Number of car parking spaces required by the customer.
ReservationStatus	Categorical	Reservation last status, assuming one of three categories: Canceled (booking was canceled by the customer), Check-Out (customer has checked in but already departed), No-Show (customer did not check-in and did inform the hotel of the reason why).
ReservationStatusDate	Date	Date at which the last status was set. This variable can be used in conjunction with the ReservationStatus to understand when was the booking canceled or when did the customer checked-out of the hotel.
ReservedRoomType	Categorical	Code of room type reserved. Code is presented instead of designation for anonymity reasons.
StaysInWeekendNights	Integer	Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel. Calculated by counting the number of weekend nights from the total number of nights.
StaysInWeekNights	Integer	Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel. Calculated by counting the number of week nights from the total number of nights.
TotalOfSpecialRequests	Integer	Number of special requests made by the customer (e.g. twin bed or high floor).
