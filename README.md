# Final_Project

## Selected Topic:
	
Flight Status Prediction

## Reason why they selected their topic
	
 We chose this topic because we want to know what attributes are the ones that are the most important to generate a delay in a certain flight. In that way, we will create a web page for users that will fill attributes and give them a forecast with machine learning if the flight will be “On Time” or “Delayed”


## Questions they hope to answer with the data
	
  Will a flight be “On Time” or “Delayed”?
  
  Which attributes are the ones that mostly affect a flight's status?
  
  What is the probability that your flight will be delayed? 
  
  How do airlines compare between each other? 


## Roles

X: Montserrat Cruz

Square: Paolo Zambrano

Circle: Luis Canas

Triangle: Alejandro Rabelo

## Technology

- AWS’s S3
- ETL Process: Python with Jupyter Notebook
- Deep Learning model: Scikit learn & Python in Google Collab
- DashBoard: Tableau
- Heroku 


## Database:

Data was extracted from Kaggle but the information it contains comes from the Marketing Carrier On-Time Performance. Data contains more than 100 variables with information about flights like: Day of the Week, Day of the Month, Airline Carrier Code, Operating Airline, Origin Airport, Destination Airport, Departure Time, ArrDelay. Data will be stored in AWS's S3. 

Link to data on Kaggle:

https://www.kaggle.com/datasets/robikscube/flight-delay-dataset-20182022

## ETL:

After choosing our topic and finding a database we wanted to work on, it was time to begin the cleaning process in order to use it. Since our data was divided into different documents we where required to join them together to have all the data on one same document. To do this we first uploaded all data into an S3 Bucket on AWS. By doing so all team members had access to the data and we where able to merge the databases together using Jupyter Notebook. Once merged, we where able to select only the variables that where usefull for our analysis, create a machine learning model and create visualizations on Tableau public.

![65658928-9987-450d-b9ec-3ce94ba675ea](https://user-images.githubusercontent.com/108498940/203883553-f1b7ff22-5d54-4aa3-ba7f-8e771a50e90c.jpg)

#### Importing data into Jupyter Notebook to start merging all databases using concatenate:

![a15b8f2e-467d-40c7-88b2-37f1f34e242c](https://user-images.githubusercontent.com/108498940/203888358-4f0d954f-5134-4fb6-b134-e7d4bfc2ed58.jpg)


## Machine Learning Model:

### Description of preliminary data preprocessing

### Description of preliminary feature engineering and preliminary feature selection, including their decision-making process 

### Description of how data was split into training and testing sets 

### Explanation of model choice, including limitations and benefits


## Dashboard:

After going over our data, we decided that the best way to display our visualizations is using Tableau Public Storys. This is an interactive and easy way to visualize our data and interact with it. 

Link to Dashboard on Tableau Public:

https://public.tableau.com/shared/B3ZTZZN7S?:display_count=n&:origin=viz_share_link


### Interactive elements:

After going over our data, we decided that the best way to display our visualizations is using Tableau. Some ideas of possible visualizations we have right now are: 

1.	Map with the locations of the airports with the most delays.
2.	Heatmap of the days with the most delays.
3.	Bar graph / heatmap with the day of the week with the most delays.
4.	Bar graph with the hours of the day with the most delays.
5.	Shape with the airlines with the most delays similar to the following:

<img width="215" alt="image" src="https://user-images.githubusercontent.com/108498940/203885440-b462da1e-4ec0-48d9-b080-7c8b0da2b5a5.png">

These visualizations are interactive because if you click on any part of the visualization, it will show you specific infromation like in the following example: 

![Dashboard](https://user-images.githubusercontent.com/108498940/203888488-1c434bd2-c7e1-49c3-8f11-ebc7b0d8cdeb.gif)
Source: https://analyticsindiamag.com/how-to-create-interactive-public-dashboards-and-storylines-in-tableau/


## Final presentation:

https://docs.google.com/presentation/d/16Z3Wulr2pZyQmhmy__KBiV7Zt9pVuMMYErxm2aR9sDc/edit#slide=id.g1a2b0531266_0_39
