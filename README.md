# Furniture Store: 35 SQL Requests
35 explained SQL queries from Furniture Store database that sells primarily desks and tables in the United States. 

- 01-customer-insights
- 02-order-analysis
- 03-product-performance
- 04-sales-value-metrics
- 05-subqueries-and-exists
- 06-conditional-analysis

This project showcases 35 SQL queries written against a sample database of 4 tables. Each query solves a practical business question, using joins, aggregation, filtering, and advanced SQL features.

## ERD (Entity Relationship Diagram) 
![ERD](https://github.com/JzesatiD/DeskStoreSQL_35_Queries/blob/main/assets/furniturestoreERD.png?raw=true)

### Why SQL Was Used for This Analysis
This analysis leveraged SQL as the primary tool to explore a relational database representing a furniture store’s operations. SQL's power to perform complex joins, filtering, group-based aggregation, and subqueries made it ideal for answering layered business questions drawn from customer, order, product, and sales data.

SQL enabled structured interrogation of the data to reveal insights across multiple levels of the business — from regional customer activity and order composition, to product demand patterns and revenue concentration. The language’s flexibility in combining data across multiple related tables (Customer, Order, OrderLine, Product) allowed for targeted business questions to be answered with clarity and precision.

### Business Insights Discovered
Through the use of SQL, several strategic findings were uncovered:

Customer Insights: Patterns emerged around where customers were concentrated, how engaged they were (based on order frequency), and which states showed untapped or declining activity. This surfaced opportunities for location-based re-engagement and more personalized outreach.

Order Composition and Value: Orders were not only analyzed by volume and contents, but also by spend thresholds — identifying high-value orders, frequently bundled products, and customers contributing the most revenue. This has direct implications for loyalty programs and sales forecasting.

Product Performance: SQL was instrumental in highlighting which product finishes were consistently lower or higher priced, and which products were most commonly ordered. These insights support pricing strategy, inventory planning, and marketing focus on best-sellers.

Revenue and Sales Metrics: Customer-level spend aggregation and per-order cost analysis made it possible to pinpoint top customers and high-performing SKUs. These findings guide customer prioritization and can help align marketing with profitability.

Advanced Filtering and Segmentation: Using subqueries and conditional logic, the analysis could surface nuanced customer groups — such as those who ordered premium products but reside outside major states, or those who have lapsed in engagement. These refined cohorts are critical for targeted campaign development.

### Summary
By leveraging SQL to model real business questions, this analysis demonstrated how raw transactional data can be transformed into decision-ready insights. Each query went beyond syntax — it addressed a tangible operational, sales, or marketing need. The process reflects what data analysts do in real-world roles: not just retrieve data, but uncover what matters and why it matters to the business.

### 📁 01-customer-insights.md

1. List all States with more than 2 customers per state

2. Retrieve names and state of customers not in Florida, California, and Texas

3. Find how many customers are there in each state

4. List Customer ID and names for customers that did not place any order

5. For each Florida customer with less than three orders, display their names and how Many times each customer placed orders

6. For each customer with less than 2 orders and outside California and Florida, display their names and how many times each customer placed orders

7. List customer names and states that either ordered products with less than average price or they are located in any state except NY, NJ, TX (EXISTS Operator)

8. Retrieve names and states of customers that have placed orders and are not located in California or Texas

### 📁 02-order-analysis.md

1. Display Order ID and the total amount of each order (each order may include multiple products)

2. List Orders with more than one Product and show number of products in each of these orders

3. List total dollar amount for each order that includes ProductID = 2

4. List total dollar amount for each order that includes Coffee Table

5. For orders more than $2000, create an invoice and show the total dollar amount of each order. Sort the result by orderID

6. For the most expensive products, display the order ID and customer name

### 📁 03-product-performance.md

1. Display average standard price for every product finish

2. For all ordered products, list product IDs, their description and the number of times each product has been ordered.

3. List product ID, description and price of products with less than average standard price of all products.

4. List product ID, description and price for products with less than average standard price that have been ordered more than once. Sort the result based on the product price. (Use subqueries)

6. What quantity of each product finish has been ordered by customers whose postal code starts with 9 or ends with 4? Show each Product finish along with its total quantity ordered.

7. List in alphabetic order the product finish and the average price for each product finish with the average price of less than 750.

### 📁 04-sales-value-metrics.md

1. Retrieve the Product IDs and the total cost of each product in Order 1001

2. List Customer names and total amount spent per customer

3. For all customers that have placed orders, display customer IDs, names and their order numbers. Sort the result based on customer names

4. Show customers with two or more orders. Include customer ID, name and number of orders.

5. Retrieve customer ID and name that purchased products below average price

### 📁 05-subqueries-and-exists.md

1. List customer names and states that ordered products with “Natural Ash” finish and are located outside California.

2. What are the customer states and their order IDs that include product(s) with more than the average standard price? (EXISTS)
Customers who ordered “Natural Ash” and live outside CA (EXISTS)

3. Retrieve name and IDs of customers that have not placed any orders or they are located in Texas. Sort the result based on the customer ID

4. Show description and total quantity of products that have been ordered a total of more than 3 quantity and are more expensive than the average price of product lines 1 and 2

### 📁 06-conditional-analysis.md

1. Display the names and addresses of Florida customers with total orders of more than $2000 value

2. Names of Florida customers with more than one order

3. For Customers with one or more orders, display their names and number of times they placed orders Customers from FL or who ordered Cherry finish: retrieve order IDs, names, states, and order total

4. For orders placed by customers from Florida or include products with “Cherry” finish, retrieve order IDs, Customer names, their state, and the total amount of orders

5. For each customer with less than 2 orders and outside of California and Florida, display their names and how many times each customer placed orders.

✅ Summary
Category	     &emsp;&emsp;&emsp;&emsp; Count

1. customer-insights.md	   &emsp;&emsp;&emsp; 8
2. order-analysis.md	    &emsp;&emsp;&emsp;&emsp;&emsp;6 
3. product-performance.md&emsp;&emsp;7
4. sales-value-metrics.md&emsp;&emsp;&emsp;5
5. subqueries-and-exists.md&emsp;&emsp;4
6. conditional-analysis.md&emsp;&emsp;&emsp;5

Total &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;   35 
