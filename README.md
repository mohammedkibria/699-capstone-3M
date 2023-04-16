# What Makes A Valuable Airbnb?
699-capstone-3M
Capstone Project for SIADS 699 - Mark, Mohammed, Matthew

# About The Project
The goal of this data science project is to discover and describe common characteristics of desirable Airbnb investment properties. 

# Data Flow
There are four primary tasks for this project. 
* Amenities Generalization
* Nearby Attractions and Entertainment
* Price Prediction Modeling and Analysis
* Topic Modeling

Please refer to the data flow illustration below to understand how all assets interact with each other.
![alt text](https://github.com/mohammedkibria/699-capstone-3M/blob/main/images/Data%20Flow%20Illustration%20Final.png?raw=False)

# Data Access Statement
There are two primary datasets for this application. 
## AirBnB
The full and detailed listings, calendar, and reviews comma-separated values (CSV) files from AirBnB can be found [here](http://insideairbnb.com/get-the-data). The selected destination for this project is Nashville, Tennessee (TN).

## Yelp Fusion API
The nearby attractions and entertainment task requires an account with Yelp and register an application in order to get an authentication token. The authentication token will allow someone to call the Yelp Fusion API. The following documentation is provided by Yelp. 
### Documentation
* The [Fusion Authentication](https://docs.developer.yelp.com/docs/fusion-authentication) document explains how register an application to get an authentication token. 
* The [Getting Started with Yelp Fusion API](https://docs.developer.yelp.com/docs/fusion-intro) document explains the Yelp Fusion API. The Yelp Fusion API has many flavors known as *endpoints*. Each *endpoint* returns different information. The *endpoint* for this project is **Business Search**.
* The [Search businesses](https://docs.developer.yelp.com/reference/v3_business_search) document is a data dictionary to explain what is returned from calling the **Business Search** endpoint. 
* The [Categories](https://docs.developer.yelp.com/docs/resources-categories) document is a list that shows all categories currently recognized for search filtering.

### Inserting Yelp Fusion API Authentication Token
This application is setup to accept any Yelp Fusion API authentication token. There is the *Yelp API Key.txt* file located at the root of this repository. This file is referenced in the application whenever calling the Yelp Fusion API. Update this file with the latest authentication token to run this feature of the application. The syntax is as follows. 
```sh
API Key : <Insert Yelp Fusion API Key Here>
```

### API Terms of Use
* As mentioned directly from the written report, the Terms of Use for the Yelp Fusion API requires information to be at an aggregate form. Final submission for SIADS Capstone requires the GitHub project repository to be made publicly available for others to view. Making the GitHub project repository publicly available and pushing the business information from Yelp may have unintended consequences. One cannot assume the intentions of the viewers of the repository. As a result, a CSV file which has fake business information has been made available to illustrate the schema and information returned by calling the Yelp Fusion API.
* The API Terms of Use by Yelp can be found [here](https://www.yelp.com/developers/api_terms). 

