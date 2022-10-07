# Geospatial-Analysis

## Objective

The basic idea of analyzing the Zomato dataset is to get a fair idea about the factors affecting the establishment of different types of restaurants at different places in Bengaluru. This Zomato data aims at analyzing demography of the location. Most importantly it will help new restaurants in deciding their theme, menus, cuisine, cost, etc for a particular location. It also aims at finding similarity between neighborhoods of Bengaluru on the basis of food.

The main objective of this project is to find insights and get some idea about the restaurants in Bangalore using different techniques like EDA, Geospatial and Sentiment Analysis.

## Problem Statement

Observations on the following are made:
1. Top restaurant chains in Bangaluru
2. How does the price differ between restaurants that accept online orders and those that don't?
3. How many restaurants offer table reservations compared to those that do not?
4. Types of restaurants available
5. Top-rated restaurants
6.  Restaurants located at various locations around Bangalore
7. Approximate cost for 2 people
8. How does the vote on restaurants accepting online orders compare to those refusing to accept them?
9. In what restaurant does the most costly rate for two people exist? What is the dish involved? The most popular dish to eat there?
10. Top ten most expensive and cheapest restaurants, based on an estimate for two people
11. Restaurants under 500 (budget hotels)
12. Budget-friendly restaurants with rating >4
13. Overall number of restaurants that have ratings >4 and are under budget (less than 500)
14. Hotels at various locations with affordable rates
15. Foodie's hotspots
16. Heatmap of North Indian and South Indian restaurants
17. Chains with the most popularity for casual dining
18. Favorite dishes in various cuisines represented by a word cloud

## Dataset

The dataset contains 17 columns as shown below:
- **url** - url of the restaurant in the zomato website
- **address** - address of the restaurant in Bengaluru
- **name** - name of the restaurant
- **online_order** - whether online ordering is available in the restaurant or not
- **book_table** - table booking option available or not
- **rate** - overall rating of the restaurant out of 5
- **votes** - total number of rating for the restaurant as of the above mentioned date
- **phone** - phone number of the restaurant
- **location** - neighborhood in which the restaurant is located
- **rest_type** - restaurant type
- **dish_liked** - dishes people liked in the restaurant
- **cuisines** - food styles, separated by comma
- **approx_cost(for two people)** - approximate cost of meal for two people
- **reviews_list** - list of tuples containing reviews for the restaurant
- **menu_item** - list of menus available in the restaurant
- **listed_in(type)** - type of meal
- **listed_in(city)** - neighborhood in which the restaurant is listed

## Data Analysis Using Python

Work flow of process:
1. Data Collection
2. Data Cleaning
3. Performing EDA
4. Performing Geospatial Analysis
5. Performing Sentiment Analysis

<p align="center"><img width="436" alt="image" src="https://user-images.githubusercontent.com/71536311/194030212-c6501431-385d-401a-8b15-32c9eaf2864a.png"></p> 

### Data Collection
- The Dataset “ZOMATO BANGALORE RESTAURANTS” is publicly available on Kaggle website with 51,717 records and 17 attributes as shown under the dataset section.

### Data Cleaning
- This is an essential step to perform before creating a visualization. 
- Clean, consistent data will be much easier to visualize.
- As a result, missing values are filled, data are filtered accordingly, and inappropriate data are removed.   

### Exploratory Data Analysis
- There are different types of charts Bar, Pie, Line, Scatter Plot, Column chart etc. which can visually present the data in more understandable way.
- Below bar chart shows the most famous restaurant chains in Bangalore with number of outlets.

<p align="center"><img width="571" alt="image" src="https://user-images.githubusercontent.com/71536311/194037000-d06ac267-2a96-494e-867b-b85187c80e5a.png"></p>

- The following pie chart shows the percentage of online orders accepted by restaurants.

<p align="center"><img width="200" alt="image" src="https://user-images.githubusercontent.com/71536311/194037223-0b6008bd-fa97-40db-a14f-b7cd5294c31c.png"></p> 

- The below figure represents the bar chart for different types of restaurants.

<p align="center"><img width="657" alt="image" src="https://user-images.githubusercontent.com/71536311/194037589-e36863c3-5416-4e32-8417-2a4374569322.png"></p> 

- Bar graph of different varieties of cuisines in Bangalore.

<p align="center"><img width="436" alt="image" src="https://user-images.githubusercontent.com/71536311/194037795-00b5ec12-1978-4cbb-8bf9-c4bb6d376793.png"></p> 

- Below scatter plot with X axis denotes the ratings of the restaurants and Y axis denotes the approximate cost for 2 people. 

<p align="center"><img width="512" alt="image" src="https://user-images.githubusercontent.com/71536311/194037948-7d08a98d-3fd9-4797-b96e-bb8e702969ae.png"></p> 

- Box plot depicting the price difference between restaurants that accept online orders and those that do not

<p align="center"><img width="341" alt="image" src="https://user-images.githubusercontent.com/71536311/194038465-a933fa89-a360-474e-b8ef-bc8dec129d17.png"></p> 

### Geospatial Analysis
- Geospatial Analysis is useful for locating the geographical area in a particular region. 

##### Heatmap of Restaurants in Bengaluru city
- For locating the restaurants in geographical map, we need latitudes, longitudes and count of restaurants. 
- Extract the "Latitude" and "Longitude" w.r.t. different Locations using Python's Geopy Library.
- Generate a "BaseMap" of Bangalore using Python's Folium Library.

<p align="center">![geo analysis](https://user-images.githubusercontent.com/71536311/194481196-7dadb075-df9e-4cc7-a80a-d04d00e965ba.gif)</p> 

- Plot a HeatMap based on variety of use cases with the help of Python's Folium "HeatMap" Plugins.
- The heatmap below depicts the clutter of restaurants in Bengaluru.

<p align="center">![heatmap of blore](https://user-images.githubusercontent.com/71536311/194491554-33fb6835-b758-464d-a87e-cb629f09c917.gif)</p> 

##### Heatmap of North Indian restaurants

<p align="center">![hm of ni](https://user-images.githubusercontent.com/71536311/194495875-a61c539d-4ce2-4fd3-b880-abd85bd87d72.gif)</p> 

### Sentiment Analysis
- Here are the Wordclouds for 9 different types of restaurants where customers left feedback.   
- 
<p align="center"></p> 


## Tools Used
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)   ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)   ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)   ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)   ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23#ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=white)   ![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)

- Jupyter Notebook is used as IDE.
- Among the Python libraries, Pandas and NumPy are used for handling data, preprocessing, and mathematical operations, respectively.
- Plotly, Seaborn, and Matplotlib are used for visualizing plots.

For more details, please go through the Jupyter Notebook attached above.

## Conclusion

- 
