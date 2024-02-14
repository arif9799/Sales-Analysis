

Situation:

- An online store data is information collected by online retailers about products, customers profiles , transactions/Sales, generalized information such as geographic locations, payment methods, etc
- It is crucial for analyzing customer behavior, buying patterns & trends among the population to improve customer experience & marketing strategies, make informed decisions and provide recommendations to customers in order to boost sales
- The data that we have available is in 12 different files pertaining to 12 months of a calendar year, that we combine and perform our Sales Analysis on

Task:

- To perform extensive Exploratory data analysis to understand consumer behavior and buying patterns, identify products to recommend and boost the profit margin

Approach:

- Starting off with data retrieval, fetch the 12 files of monthly sales data, clean, exclude na value and combine them into a Single Master File to easily work on

- Loading the combined data and performed feature engineering of imperative variables that will be crucial for extensive EDA, such as:
    - Separating the "Order_Date" into "Date" and "Time", and then Splitting the "Date" into "Month", "Day" and "Year" for time component analysis
    - Splitting the "Purchase_Address" Column into "City", "State" and "Zip"
    - Converting Order Date into Date time format (excluding exact time of the day) and creating individual hours and minutes column

- Performing Extensive EDA through following visualizations to understand sales patterns and consumer behavior:

    - Monthly sales (in terms of quantity of items and revenue generated): findings show that maximum number of items or maximum revenue generation was in the month of October and December, probably due to high demand in Thanksgiving and Christmas

    - City Wise Sales (in terms of quantity of items and revenue generated): findings revealed that maximum number of orders were placed from San Francisco, CA, hence resulting in high revenue generation through that city alone, followed by Los Angeles, CA, New York, NY, Boston, MA

    - State Wise Sales (in terms of quantity of items and revenue generated): Similarly findings revealed maximum demand was from CA, followed by NY, TX, MA

    - Best Selling Products (based on their sales): Plotted top 10 products that included AAA Batteries, AA Batteries, USB-C Cable, Lightning Cable, etc. The bar plot of best selling products was contrasted with its price, revealing an opposite trend, showcasing low-priced products with high sales & high priced products with low sales

    - Orders Placed on Specific hour of the day: An interesting finding was that most of the orders were placed at 13th & 20th hour of the day, where 13th hour is mot commonly lunch breaks and 20th hour is when most people get done with their day, finishing office work and their chores. It is at this time that people resort to online shopping to take their minds off the work and find recreation in shopping

- Finally, post EDA, we utilize certain python libraries and determine the most frequent item sets (pair of items that are often bought together), and found some very common pairings like [I-phone, Lightning Cable], [Google Phone, USB-C Cable], [I-phone, Wired Headphones], [Iphone, Apple Airpods]

- We also determined most frequent item sets in triplets such as  [I-phone, Lightning Cable, Apple Airpods], [I-phone, Lightning Cable, Wired Headphones ], [Google Phone, USB-C Cable], [Google Phone, USB-C Cable, Wired Headphones]

- Based on pairs and triplets of most frequent item sets, we curated a list of products to recommend item x to a buyer when they buy item y


Results:
- The list of recommendations, hypothetically surges the profits by 26% additional to the forecasted demand 
- If product x costing $10 is forecasted to have a demand of 20 items potential to gain foreseeable sales of $200, then product y costing $2.5 should be recommended alongside product x, which could potentially add $50 of additional sales value. Where product x and y are most frequently bought together, a new customer that tends to buy product x is highly likely to buy product as well!. 
