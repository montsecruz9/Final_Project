# Machine Learning model

## Preliminary data processing
The following columns were deleted as there were of no use for our model because of NaNs and the amount of categorical data: 'Origin', 'Dest', 'Unnamed: 0', 'OriginCityName', 'DestCityName', 'Cancelled', 'CarrierDelay', 'WeatherDelay', "NASDelay", 'SecurityDelay', 'LateAircraftDelay', 'FirstDepTime', and 'CancellationCode'.

We created the column 'Is_Delayed' as this is our target for the model, to predict whether a flight might be delayed independently on the type of delay, origin city, destination city, and the rest of the columns deleted. 

## Preliminary feature engineering and preliminary feature selection
As mentioned before, we decided to ignore the features deleted as we don't want to focus on the type of delay flights may have. We will ignore the origin and destination cities as well, and just take into account the airline and the elapsed times between destinations (flight duration). 

To convert our categorical data into indicators we used the pandas get_dummies() method. 

Our target is the 'Is_Delayed' column, and so our features are all the rest of the columns. 

## Splitting data into training and testing sets

## Model choice

