# Club-Mahindra-Machine-Learning-Hackathon
The task was to build to machine learning model to predict the average spend on Food & Beverages that a member would spend on a particular booking using historical bookings data like checkin date,checkout date,channel of booking,product purchased,resort type, resort location,room type,total persons travelling,roomnights booked,member demographics etc.
Datasets Provided :- train.csv and test.csv

#Modelling Approach
Generated more features out of the existing like:
1.Extracted features from date variables(checkin date,checkout date,booking date) - month of year, year,week of year,day of week, day of month , weekend flag(0/1)
2.Number of days between booking date and checkin date
3.Number of days of stays
4.days since last visit
5.days since first visit
6.number of visits before
7.roomnights per head
8.roomnights booked so far
9.Created various count variables based on categorical variables
10.Target encoding of categorical variables

Fitted a tuned xgboost model with 5 fold cross-validation.



