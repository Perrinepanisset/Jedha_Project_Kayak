# KAYAK PROJECT

## CONTEXT
Kayak marketing team needs help on a new project. After doing some user research, the team discovered that 70% of their users who are planning a trip would like to have more information about the destination they are going to.

In addition, user research shows that people tend to be defiant about the information they are reading if they don't know the brand which produced the content.

Therefore, Kayak Marketing Team would like to create an application that will recommend where people should plan their next holidays. The application should be based on real data about: Weather and Hotels in the area

The application should then be able to recommend the best destinations and hotels based on the above variables at any given time.

## GOAL

As the project has just started, the team doesn't have any data that can be used to create this application. Therefore, the job will be to:
- Scrape data from destinations (35 cities listed)
- Get weather data from each destination 
- Get hotels' info about each destination 
- Store all the information above in a data lake Extract, transform and load cleaned data from the datalake to a data warehouse

## USAGE

**1_KAYAK-API_Requests.ipynb

Extraction of GPS information for the 35 cities from the API https://nominatim.openstreetmap.org
Extraction of weather information for the next 7 days from the API https://api.openweathermap.org
  - OUTPUT FILE : '35 cities - 7 days weatherforecast.csv'

Input file : features_info.csv
Output file : dataset_with_labels.csv (not hosted on this repository, you have to create it yourself)
Explore_dataset.ipynb
Automates some computations of basic statistics and plots for each feature in the dataset

Input file : dataset_with_labels.csv
Train_models.ipynb
Trains some multiclass classifiers from different packages (scikit-learn, keras, XGBoost) and compare their performances

Input file : dataset_with_labels.csv
