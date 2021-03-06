# Restaurant_Rating_Prediction

![eazytrendz_2723_trend20200219060910](https://user-images.githubusercontent.com/82859280/149061502-e3bf6807-84c8-4c5b-b8df-89e301bca4cf.jpg)


About Using zomato bangalore data to predict restaurant rating in machine learning, and deploy
Predicting Restaurant Ratings using Machine Learning Algorithms

Nowadays, starting a restaurant project in a given location requires a large investment by investors and effort. To start a new restaurant, you need funding from investors, who look at a lot of things before deciding to fund your restaurant. A few of those criteria are location, menu, rating of similar restaurants, etc. To help restaurant startups in Bangalore, we decided to experiment with the Zomato Bangalore Restaurants database, to see if we could draw conclusions about how location, food type, etc could affect the ratings of a restaurant.

Description of the dataset : The dataset consists of 51717 rows and 17 columns. Column Description : url : Contains the url of the restaurant in the Zomato website. address : Contains the address of the restaurant in Bangalore. name : Contains the name of the restaurant. online_order : Whether online ordering is available in the restaurant or not. book_table : Table book option available or not. rate : Contains the overall rating of the restaurant out of 5. votes : Contains the total number of rating for the restaurant as of the mentioned date. phone : Contains the phone number of the restaurant. location : Contains the neighbourhood in which the restaurant is located. rest_type : Restaurant type. dish_liked : Dishes people liked in the restaurant. cuisines : Food styles, seperated by comma. approx_cost(for two people) : Contains the approximate cost for a meal for two people. reviews_list : List of tuples containing reviews for the restaurant, each tuple consists of two values, rating and review by the customer. menu_item : contains list of menus available in the restaurant. listed_in(type) : type of meal. listed_in(city) : Contains the neighbourhood in which the restaurant is listed.

Data Preprocessing : Our data consisted of quite a few null values. To solve the problem of missing values, we followed the following steps : (i) First we removed all rows containing null values in the ???cuisines??? column. (ii) For the second step, since the ???address???, ???phone???, ???url???, ???listed_in(city)??? columns had a lot of null values, we dropped these 4 columns. (iii) The third step was renaming the ???approx_cost(for two people)??? and ???listed_in(type)??? columns as ???average_cost??? and ???listed_type???

After performing a few visualizations to understand our data better, we split the data into 80% training data and 20% test data. Next, we used Machine Learning models to fit the data.
