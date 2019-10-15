Sydney Housing Pricing Proposal
===

# Background
Sydney is the capital state of New South Wales and is the most popular city in Australia and Oceania. The state has 658 suburbs, which consists of 40 local government areas and 15 contiguous regions. Due to its popularity, housing prices in Australia nowadays are expensive and can roughly cost around $850,000, more or less, in specific locations. However, housing prices mostly depend on the size, room and spacing they have.

# Summary of Project
The Sydney Housing Pricing project uses data (gathered from sold property listings) to generate a prediction of housing prices based on general features of a house, such as __bedrooms, bathrooms and car space__. This project will group property listings by council to ensure accurate results.

# Goals
The aim of our project is to predict the housing price of each local government council areas (LGCA) in Sydney. The average housing prices are categorised into groups by the number of __bathrooms, rooms, car spaces and other features__ they have.
   
The outcome of this project can help users to predict the housing price of their destined area, as well as how many rooms, bathrooms and other features they desire.

Our goal includes:
* Regression, RFE analysis and correlation matrices of the produced factors. Only the best of these factors are considered and utilised for further analysis
* Exploration of the data by inputting various graphs such as histograms, clustered bar charts and scatter plots

# Datasets
We are using **Domain's** API website (link: https://developer.domain.com.au/docs/introduction) to get data on the Sydney Housing Market.
We will use the get command weekly for n weeks as the free version allows only < 300 results per request.
The data returned is in a JSON format which we will use an online converter to change to CSV.
The CSV files have the following column names 
`['unitNumber', 'streetNumber', 'streetName', 'streetType', 'suburb', 'postcode', 'state', 'geoLocation__latitude', 'geoLocation__longitude', 'propertyType', 'bedrooms', 'bathrooms', 'carspaces', 'price', 'result', 'agent', 'id', 'agencyId', 'agencyName', 'agencyProfilePageUrl', 'propertyDetailsUrl']`
The data should be usable for most of them. Some data preparation will have to be implemented to deal with null values, especially for empty cells, such as `['unitNumber']` as it is not necessary.
We will need to make API calls weekly (preferably after the weekend) to ensure that we have a large enough dataset to analyse.

# Techniques used
* Machine learning techniques that will classify **a mean-regression model** such as __K-means clustering, linear and logistic Regression and REF__.


# Project Plan
**Our project plan** - assign at least two milestones for each member over the period of time and have them complete the given tasks. For each milestone, it describes and evaluates the result of what it has achieved in that period. 

**23/09/2019** - Have our data compiled and clean ready for analysis. After obtaining the desired data from **'DOMAIN'**, we will sift through it and ensure that we haven’t missed anything, as well as tidying it up. (Unsure of how to evaluate we have succeeded).

**14/10/2019** - By week 10 or week 11, Our project should have a working solution that can generate a price prediction model from inputted features (e.g. 1 garage, 2 bedrooms, 1 bathroom).

# Relevant Prior Work
We have taken inspiration from a Kaggle project on the Melbourne Housing Market (link: https://www.kaggle.com/anthonypino/melbourne-housing-market?fbclid=IwAR10TIvlSaPyCW73dtIHkkXad6Tmjo4ezpUIPeWKFeMtl4o29SIN2QuKU1I)
We are going to adapt to this idea, **'Sydney housing Pricing'** and collect the necessary data that is required.

