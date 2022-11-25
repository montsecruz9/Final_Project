# Final_Project

## Selected Topic
	
  Flight Status Prediction

## Reason why they selected their topic
	
  We chose this topic because we want to know what attributes are the ones that are the most important to generate a delay in a certain flight. In that way, we will create a web page for users that will fill attributes and give them a forecast with machine learning if the flight will be “On Time” or “Delayed”

## Description of their source of data
	
  Data was extracted from the Marketing Carrier On-Time Performance. Data contains information about flights like: Day of the Week, Day of the Month, Airline Carrier Code, Operating Airline, Origin Airport, Destination Airport, Departure Time, ArrDelay. Data will be stored in AWS's S3. 

## Questions they hope to answer with the data
	
  Will a flight be “On Time” or “Delayed”?
  Which attributes are the ones that mostly affect a flight's status?

## Roles

X: Montserrat Cruz

Square: Paolo Zambrano

Circle: Luis Canas

Triangle: Alejandro Rabelo

## Technology

- Data Storage: AWS's S3
- ETL Process: Python with Google Collab
- Deep Learning model: Scikit learn & Python in Google Collab
- DashBoard: FlaskApp

## Communication protocols:

Our team will be communicating through Slack and working on the same repository on Github. Every team member will have their own branch in order to make changes without affecting the main branch. We will join at leats one zoom meeting every week to work on the project, in addition to the two classes per week. In case someone needs help they should let the team know through Slack and everyone should help regardless of their roll. It is responsability of each individual to let the team know if they need help, won't attend class or is having an issue of any type.

## Outline of the project:

### Database:

#### After finding the database we wanted to work on, we where required to clean its columns and values in order to be able to use it for our analysis. Since our data was divided in different documents, we first uploaded everything into an S3 bucket on AWS. This way all team members will have access to them and it will make it posible to load our data into a Jupyter Notebook to clean the data:

![65658928-9987-450d-b9ec-3ce94ba675ea](https://user-images.githubusercontent.com/108498940/203883553-f1b7ff22-5d54-4aa3-ba7f-8e771a50e90c.jpg)

#### Once this was done, we where able to import our data into a Jupyter Notebook to start joining all databases using append:

![b0a900dc-c66d-4291-bc40-c6db2722f856](https://user-images.githubusercontent.com/108498940/203883877-f573924d-fc59-4ea4-a89a-d7db55d61c27.jpg)

![08ebba1f-646f-499d-a08c-74b5a4b320c2](https://user-images.githubusercontent.com/108498940/203883926-2084fbf1-55ab-48ad-88c8-09b4f665f4ba.jpg)


#### Once all our databases where joined together we cleaned the data on SQL:




## Machine Learning Model:

### Description of preliminary data preprocessing

### Description of preliminary feature engineering and preliminary feature selection, including their decision-making process 

### Description of how data was split into training and testing sets 

### Explanation of model choice, including limitations and benefits


## Dashboard:


### Storyboard on Google Slides:



### Tools:

After going over our data, we decided that the best way to display our visualizations is using Tableau. Some ideas of possible visualizations we have right now are: 

1.	Map with the locations of the airports with the most delays.
2.	Heatmap of the days with the most delays.
3.	Bar graph / heatmap with the day of the week with the most delays.
4.	Bar graph with the hours of the day with the most delays.
5.	Shape with the airlines with the most delays similar to the following:

<img width="215" alt="image" src="https://user-images.githubusercontent.com/108498940/203885440-b462da1e-4ec0-48d9-b080-7c8b0da2b5a5.png">

### Interactive elements:





