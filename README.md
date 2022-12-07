# Final_Project

## Selected Topic:
	
Flight Status Prediction

## Reason why they selected their topic:
	
We chose this topic because we want to know what attributes are the ones that are the most important to generate a delay in a certain flight. In that way, we will create a web page for users that will fill attributes and give them a forecast with machine learning if the flight will be “On Time” or “Delayed”


## Questions to answer:
	
  Will a flight be “On Time” or “Delayed”?
  
  Which attributes are the ones that mostly affect a flight's status?
  
  What is the probability that your flight will be delayed? 
  
  How do airlines compare between each other? 


## Members

Montserrat Cruz

Paolo Zambrano

Luis Canas

Alejandro Rabelo

## Technology

- Database storage: AWS’s S3
- ETL Process: Python with Jupyter Notebook
- Deep Learning model: Scikit learn & Python in Google Collab
- DashBoard: Tableau
- Heroku 


## Database:

Data was extracted from Kaggle but the information it contains comes from the Marketing Carrier On-Time Performance. Data contains more than 100 variables with information about flights like: Day of the Week, Day of the Month, Airline Carrier Code, Operating Airline, Origin Airport, Destination Airport, Departure Time, ArrDelay. Data will be stored in AWS's S3. 

Link to data on Kaggle:

https://www.kaggle.com/datasets/robikscube/flight-delay-dataset-20182022

## ETL:

After choosing our topic and finding a database we wanted to work on, it was time to begin the cleaning process in order to use it. Since our data was divided into different csv files we where required to join them together to have all the data on one same file. To do this we first uploaded all data into an S3 Bucket on AWS. By doing so all team members had access to the data and we where able to merge the databases together using Jupyter Notebook. Once merged, we where able to select only the variables that where usefull for our analysis, create a machine learning model and create visualizations on Tableau public.

![65658928-9987-450d-b9ec-3ce94ba675ea](https://user-images.githubusercontent.com/108498940/203883553-f1b7ff22-5d54-4aa3-ba7f-8e771a50e90c.jpg)

Result of importing data into Jupyter Notebook to start merging all databases using concatenate:

<img width="863" alt="Screen Shot 2022-12-06 at 21 35 43" src="https://user-images.githubusercontent.com/108498940/206082001-acd52c02-b2fa-4c7d-9dbc-9001d9836be6.png">


## Machine Learning Model:

### Description of preliminary data preprocessing

### Description of preliminary feature engineering and preliminary feature selection, including their decision-making process 

### Description of how data was split into training and testing sets 

### Explanation of model choice, including limitations and benefits


## Dashboard:

After going over our data, we decided that the best way to display our visualizations is using Tableau Public Storys. This is an interactive and easy way to visualize our data and interact with it. 

Link to Dashboard on Tableau Public:

https://public.tableau.com/shared/YKTTJT8R8?:display_count=n&:origin=viz_share_link


### Interactive elements:

Months with the most minutes delay:

![ac1be28d-b802-4cab-9367-49dfb2b24944](https://user-images.githubusercontent.com/108498940/206078738-3b2bbc8e-f6bd-4332-a7ab-70d2c8f64722.jpg)

Airlines with the most delays:

![f5fc7426-d69e-4250-ab86-caf587fa72ec](https://user-images.githubusercontent.com/108498940/206078789-7a685622-f82d-4f2e-b734-86c8d22bc2ec.jpg)

Day of the week with most delay:

![ea950d06-67fa-4a73-8e9c-720f81e36f58](https://user-images.githubusercontent.com/108498940/206078878-879f2335-73e7-4e57-9a11-00595eb70b56.jpg)

Orignins with most delays:

![0140753a-0446-4acf-8223-31e37c26e799](https://user-images.githubusercontent.com/108498940/206078974-583b4fdc-e4d3-4be9-8c8b-0b2374f9a06b.jpg)

Destinations with most delay map:

![b6ba2277-a137-4a96-a7c9-cb1d7e181406](https://user-images.githubusercontent.com/108498940/206079135-c46ca67a-c42a-4d74-ab85-741011b4c5e6.jpg)


## Results/Conclusions

Results from ML and conclusions!

## Final presentation:

https://docs.google.com/presentation/d/16Z3Wulr2pZyQmhmy__KBiV7Zt9pVuMMYErxm2aR9sDc/edit#slide=id.g1a2b0531266_0_39
