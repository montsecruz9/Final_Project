# Machine Learning model

## Preliminary data processing
The following columns were deleted as there were of no use for our model: ['Year', 'DayofMonth', 'CRSDepTime', 'DepTime', 'DepDelayMinutes', 'CRSArrTime', 'ArrTime', 'CRSElapsedTime', 'ActualElapsedTime', 'CarrierDelay', 'WeatherDelay', 'NASDelay', 'SecurityDelay', 'LateAircraftDelay', 'Origin', 'OriginCityName', 'DestCityName', 'Unnamed: 0', 'Cancelled', 'FirstDepTime', and 'CancellationCode'

We created the column 'Is_Delayed' as this is our target for the model, to predict whether a flight might be delayed or not independently of the origin or destination city. 

The columns for the types of delays contained a lot of NaNs. We stil decided to keep those columns and drop the NaNs.  

## Preliminary feature engineering and preliminary feature selection
Our target is the 'Is_Delayed' column, and so our features are all the rest of the columns. 

As mentioned before, we decided to ignore the origin and destination cities, and just take into account the airline, the elapsed times between destinations (flight duration), and the type of delay. 

To convert our categorical data into indicators we used the pandas get_dummies() method. In our case, we just converted the 'Airline' column. 

## Splitting data into training and testing sets
Data was split in the ratio 70:30

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.30, random_state=42)

## Model choice
After trial and error with several models, we decided on using the Logistic Regression model, as it was the only one that worked for us. 
