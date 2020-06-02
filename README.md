![Airbnb logo](https://miro.medium.com/max/2000/1*BsKbDTA9ZUVroeJ7asId4Q.png)

# Smart(er) Pricing Predictor
Dinis Oliveira Costa
Data Part-time Dec 2019

## Content
- [Project Description](#project)
- [Data](#data)
- [Hypothesis](#hypothesis)
- [Problem](#problem)
- [Project goal](#projectgoal)
- [Workflow](#workflow)
- [Results](#results)
- [Deliverables](#deliverables)


### Project Description

- In a nutshell, Smart Pricing is Airbnb’s way of ensuring hosts make the most of possible bookings depending on the situation of the market. Once you enable the tool, you can then set the minimum price that you’d accept, and the maximum price which you’d be willing to charge. In addition, you can also input when you want to make your property available.

- Some hosts simply state that Airbnb smart pricing not working, but the main issue seems to be related with the algorithm setting their prices too low. Since Airbnb wants you to make a booking, and that will most likely happen with lower prices, the theory is that the algorithm tends to suggest lower-than-market-value prices. 

- The goal of this project was to build an alternative price predictor based on a dataset of Barcelona's listings.

- The workflow consisted of an extensive exploratory data analysis of listings in Barcelona and the construction of a machine learning model capable of predicting the most recommendable price.

- The commands assume an intermediate understanding of the Pandas, Matplotlib and scikit-learn libraries.

### Data
- For the purpose of this analysis, the [dataset](https://wiki.montera34.com/airbnb/datos/barcelona) used contains about 20K  Airbnb listings in the city of Barcelona and 96 variables regarding its specific charactheristics and amenities.

Columns: 
- `id` - listing identification number
- `name` - title of the airbnb listings
- `host_id` - host identification number 
- `host_name` - name of the owner of the listings
- `neighbourhood_group` - name of the regional neighbourhood where the listing is located
- `neighbourhood` - name of the neighbourhood where the listing is located
- `latitude` - geo coordinates
- `longitude` - geo coordinates
- `room_type` - type of listings (entire apt/private bedroom/shared bedroom/hotel room)
- `price` - cost per night 
- `minimum_nights` - minimum stay requested by the owner
- `number_of_reviews` - number of reviews in each listing
- `last_review` - date of the last time a review was posted
- `reviews_per_month` - average monthly number of reviews in each listing
- `calculated_host_listings_count` - number of listings per host
- `availability_365` - number of available days per year to rent

### Hypothesis
- [Recent posts](https://www.passiveairbnb.com/why-smart-airbnb-hosts-do-not-use-smart-pricing/), [articles](https://www.mashvisor.com/blog/airbnb-smart-pricing/) and [opinions](http://bernews.com/2020/01/column-never-use-airbnbs-smart-pricing/) suggest that hosts are increasingly starting to question the benefit of using airbnb's Smart Pricing tool when it comes to define their listing price.

- Given the surge of opinions against its use, I've decided to try to compile an algorithm to suggest an alternative price based on available data from listings in Barcelona.

### Problem:
- The prices suggested by the current airbnb Smart Pricing tool are too low when compared to market rates

### Project goal: 
- Produce a descriptive analysis of the factors that most influence an Airbnb listing's success in Barcelona 
- Develop a machine learning capable of suggesting the most adequate price for a listing
- Compare its performance based on occupancy rate and revenue generated on the long term, against the same listings that used Smart Pricing


### Workflow
- Step 1: Data Analysis - Exploratory analysis and preliminary data wrangling of the airbnb market in Barcelona 
- Step 2: Data Preprocessing - Feature transformation, encoding and scaling so it can be interpreted by the algorithm
- Step 3: Machine Learning - Training, scoring and hyperparameter tuning  of different models to improve performance 

### Results
* data.csv - with all the data collected 
* main.ipynb - containing all the code that built the project
* figures - containing the product of all the visualization that supported the project
* predicted.csv - containing the result of the predicted prices

### Deliverables
* Clean data set containing all the Airbnb listings in Barcelona 
* ML model
* Result of the predicted prices
