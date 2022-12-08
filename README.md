
## Machine Learning Model:

### Data preprocessing
The following columns were deleted as there were of no use for our model: 'Year', 'DayofMonth', 'CRSDepTime', 'DepTime', 'DepDelayMinutes', 'CRSArrTime', 'ArrTime', 'CRSElapsedTime', 'ActualElapsedTime', 'CarrierDelay', 'WeatherDelay', 'NASDelay', 'SecurityDelay', 'LateAircraftDelay', 'Origin', 'OriginCityName', 'DestCityName', 'Unnamed: 0', 'Cancelled', 'FirstDepTime', and 'CancellationCode'

We created the column 'Is_Delayed' as this is our target for the model, to predict whether a flight might be delayed or not, taking only into account the airline, destination, month and day of the week. 

The columns for the types of delays contained a lot of NaNs. We stil decided to keep those columns and drop the NaNs.
### Feature engineering and feature selection
Our target is the 'Is_Delayed' column, and so our features are all the rest of the columns.

As mentioned before, we decided to ignore the origin and destination cities, and just take into account the airline, the elapsed times between destinations (flight duration), and the type of delay.

To convert our categorical data into indicators we used the pandas get_dummies() method. In our case, we just converted the 'Airline' and the 'Dest' columns.

### Description of how data was split into training and testing sets 
Data was split in the ratio 70:30 using the scikit-learn library.
After splitting the training and testing sets, we used the RandomOversampler on our data as we noticed a huge imbalance in the classification sets. Afterwards, we scaled the data using the StandardScaler on our training data. 

### Explanation of model choice, including limitations and benefits
We chose to do a Logistic Regression Model, as it was the one that worked better with our dataset. We tried several different models: RandomForest Classifications, SMOTEEN, Easy Ensemble Classification, and others. The benefit from the Logistic Regression Model is that it is way easier to set up and train than other models. The major limitation from logistic regression is the assumption of linearity between the independent and the dependent variables. 
