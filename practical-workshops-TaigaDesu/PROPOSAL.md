Sydney Housing Pricing Proposal
===

# Background

Sydney is the capital state of New South Wales and is the most populuar city in Australia and Oceania. The state has 658 suburbs, which consists 40 local government areas and 15 contiguous regions.Due to its popularity, housing prices in Australia nowadays are expensive and can roughly cost around $850,000, more or less, in specific locations. However, housing prices mostly depend on the size, room and spacing they have.

# Summary of Project

The Sydney Housing Pricing project uses data (gathered from sold property listings) to generate a prediction of housing prices based on general features of a house, such as bedrooms, bathrooms and car space. This project will group property listings by council to ensure accurate results.

# Goals
The aim of our project is to predict housing price of each local government council areas (LGCA) in Sydney. The average housing prices are categoriesed into groups by the amount of **bathrooms, rooms, car spaces and other features** they have.
   
The outcome of this project can help users to predict the housing price of their destined area, as well as how many rooms, bathrooms and other features they desire.

Our goal includes:
* Regression, RFE analysis and correlation matrices of the produced factors. Only the the best of these factors are considered and utilised for further analysis
* Exploration of the data by inputting various graphs such as histograms, clustered bar charts and scatter plots



# Datasets
A summary of the datasets that you will use in the analysis. Where were these obtained, what format are they in, what work (if any) will you need to do to make them usable
PDFs + domain

We are using Domains API website (link: https://developer.domain.com.au/docs/introduction) to get data on the Sydney Housing Market.
We will have to use the get command weekly for n weeks as the free version allows only < 300 results per request.
The data returned is in a JSON format which we will use an online converter to change to CSV.
The CSV files have the following column names 
`['unitNumber', 'streetNumber', 'streetName', 'streetType', 'suburb', 'postcode', 'state', 'geoLocation__latitude', 'geoLocation__longitude', 'propertyType', 'bedrooms', 'bathrooms', 'carspaces', 'price', 'result', 'agent', 'id', 'agencyId', 'agencyName', 'agencyProfilePageUrl', 'propertyDetailsUrl']`
The data should be for the most part usable. Some data preparation will have to be implemented to deal with null values, Especially for all the empty cells for `['unitNumber']` as it doesnt relate to houses.
We will need to make API calls weekly (preferably after the weekend) to ensure we have a large enough dataset to analyse.

# Techniques used
* Machine learning techniques that will classify a mean-regression model such as K-means clustering, linear and logistic Regression and REF.

# Project Plan
A project plan - set at least two milestones for yourselves over the time that you have to complete the project.  For each milestone, describe what you should have achieved at that time and how you will evaluate whether you succeeded. 

23/09/2019 - We should have compiled and clean data ready for analysis. After obtaining the desired data from DOMAIN, we will sift through it, ensuring we haven’t missed anything and clean it up. (Unsure of how to evaluate we have succeeded).

14/10/2019 - By about week 10, we should have a working solution that can generate a price prediction when given features (garage, bedrooms, bathrooms).
# Relevant Prior Work
Any relevant prior work? 

We have taken inspiration from a Kaggle project on the Melbourne Housing Market (link: https://www.kaggle.com/anthonypino/melbourne-housing-market?fbclid=IwAR10TIvlSaPyCW73dtIHkkXad6Tmjo4ezpUIPeWKFeMtl4o29SIN2QuKU1I)
We are going to adapt this for the Sydney housing market and will have to collect the data ourselves.

