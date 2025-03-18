### MIST-4610-Project-1

# Group Name 
21482 Group 2

# Group Members

1. Rachel Cox [@rachellcox](https://github.com/rachellcox)
2. Jack Delinsky [@JackDelinsky](https://github.com/JackDelinsky)
3. Summer Arrington [@SummerA100](https://github.com/SummerA100)
4. Nivedita Ganesan [@niviganesan](https://github.com/niviganesan)
5. Katya Tokarev [@katyatokarev](https://github.com/katyatokarev)

# Project Description
  We were tasked with designing a data model, converting it to a relational database, inputting data, and writing
queries for the data for a bakery store. The bakery store has a structure within itself, including the customers and employees as well as necessary equipment to bake the goods.
As with any business, there are orders and details regarding transactions to keep track of. And the supplies for the bakery are sourced from different suppliers, simulating a real world example with small businesses and supply chain relations. Throughout this problem, we dive into modeling the various entities that make up the company, generating and inputting relevant data for the entities. We then  provide functioning queries for the generated data, resulting in insights about the bakery store's functions.

# Data Model Description
 Our model is based on a bakery store’s internal structure. The product entity represents the baked goods that our bakery is selling, which is connected to a supplier with a one to many relationship, since one supplier can supply multiple different products to the bakery. The ingredients are also connected to the supplier, with one supplier supplying multiple ingredients, which are later used in the recipe creating another one-to-many relationship between recipe to ingredients and a one-to-one relationship between recipe and products. 
 
Also, our model has an entity for employees, who have a schedule (with the one-to-one relationship) and also a customer that they are assigned to for the order. Our customer entity has many relationships with different entities in our data model. There is a one-to-one relationship between customers and employees, a one-to-many relationship between customers and orders (as customers can have many orders), a one-to-one relationship between customers and payments (a customer can make one payment and a payment can be made by one customer), and a one-to-many relationship between reviews. Reviews is a unique entity for our business situation. 

We chose these entities because they mirror the everyday operations of your typical bakery. 
<img width="625" alt="Screenshot 2025-03-17 at 1 55 29 PM" src="https://github.com/user-attachments/assets/c962c9ba-c7a9-40f6-ad04-afca9d0aadba" />


# Data Dictionary
  Here is the data dictionary for our model.

  
  <img width="630" alt="Screenshot 2025-03-17 at 2 13 04 PM" src="https://github.com/user-attachments/assets/2e4a854d-8fcd-4264-b1b0-627441709049" />

<img width="673" alt="Screenshot 2025-03-17 at 2 38 08 PM" src="https://github.com/user-attachments/assets/ded0b33c-e806-48c6-bd9f-e31ebd0f5edc" />

<img width="639" alt="Screenshot 2025-03-17 at 2 38 13 PM" src="https://github.com/user-attachments/assets/181c769e-2b4f-4212-bfe0-dc39d547c3ef" />

<img width="658" alt="Screenshot 2025-03-17 at 2 14 39 PM" src="https://github.com/user-attachments/assets/863a0ec6-e0b9-41bb-ae73-f5b9a701bd87" />

<img width="674" alt="Screenshot 2025-03-17 at 2 14 55 PM" src="https://github.com/user-attachments/assets/801595fe-d387-409a-a203-9caa4c4ccb18" />

<img width="644" alt="Screenshot 2025-03-17 at 2 15 34 PM" src="https://github.com/user-attachments/assets/ef45046c-27c7-4766-aba4-468ebdda1634" />

<img width="675" alt="Screenshot 2025-03-17 at 2 15 40 PM" src="https://github.com/user-attachments/assets/70329a5c-8463-4dca-9dd2-b51faddd4f8d" />

# 10 Queries

Query 1: Retrieve all employees and their roles, sorted by salary
This query retrieves a list of employees with their roles and salaries and sorts them from highest to lowest salary. This query also helps the bakery review payroll expenses and ensure fair wages.This can be useful when deciding salary adjustments or promotions and helps in budgeting for new hires (e.g., knowing how much they pay top bakers vs. cashiers).

![image](https://github.com/user-attachments/assets/36fbbd4b-8ccc-4d1a-a9b0-932939fb74c8)
![image](https://github.com/user-attachments/assets/14617cf5-97b7-40a6-bc39-7cba5fa177e2)


Query 2: List all clients with their contact details, but only those who have placed an order
This query retrieves only customers who have made a purchase (ignores inactive clients) and ensures no duplicates appear in the results. This query can also help with customer retention efforts—targeting buyers for special discounts or loyalty programs, sending email promotions or follow-up messages to actual customers, and prevents marketing efforts from being wasted on clients who never made a purchase.

![image](https://github.com/user-attachments/assets/bcefdc92-985f-42c5-ad5a-e7b71435c45b)
![image](https://github.com/user-attachments/assets/4a9a01c7-c112-4a27-879a-c69df359d5ca)

Query 3: Get all pending and processing orders, sorted by most recent
This query retrieves all unfulfilled orders that are still marked as "Pending" or "Processing" and sorts them so that the newest orders appear first. It also ensures no orders are left waiting too long, improving customer satisfaction, helps prioritize recent and urgent orders for better workflow management, and is useful for tracking order delays and resolving bottlenecks in the baking process.

<img width="471" alt="Screenshot 2025-03-17 at 8 56 44 PM" src="https://github.com/user-attachments/assets/3e3f8086-5c5f-4a05-8f23-f44be071a863" />
<img width="334" alt="Screenshot 2025-03-17 at 8 57 05 PM" src="https://github.com/user-attachments/assets/eb37f8ad-b34e-4607-9e56-af8ff2abd493" />

Query 4: Find all baked goods and their prices, showing only items above $4.00
This query retrieves only baked goods priced above $4.00 and sorts them from cheapest to most expensive. This query can help evaluate high-margin items to see which expensive products generate more profit, be used for pricing strategy—determining whether to increase prices, introduce discounts, or bundle items, and ensure premium-priced items are properly displayed and promoted.

![image](https://github.com/user-attachments/assets/b73672ba-fabb-45bf-9148-dff0620d4475)
![image](https://github.com/user-attachments/assets/71a8c1c0-01b2-4f6a-99c2-8d581102ed02)

Query 5: Find the total revenue generated from all transactions (complex)
The query calculates total revenue from completed sales and ensures only fully processed and completed transactions are counted.
Financial Planning: Helps bakery owners analyze weekly, monthly, or yearly income trends.
Profitability Analysis: Management can determine if they need to increase sales, adjust pricing, or introduce promotions.

![image](https://github.com/user-attachments/assets/9ed31747-4d45-489d-8d92-32a76bef715c)
![image](https://github.com/user-attachments/assets/8516ebf4-7b46-4e98-b52b-7ca60c6dc288)

Query 6: Get the number of orders placed by each client (complex)
The query identifies repeat customers and how often they place orders and helps understand customer loyalty and purchasing patterns. 
Customer Retention: The bakery can offer discounts or loyalty rewards to frequent buyers.
Personalized Marketing: If a customer consistently orders croissants, the bakery can suggest new pastry items they might like.

<img width="490" alt="Screenshot 2025-03-17 at 9 18 37 PM" src="https://github.com/user-attachments/assets/3d37c478-ea7d-4ab4-b229-13e602b22776" />


<img width="241" alt="Screenshot 2025-03-17 at 9 19 01 PM" src="https://github.com/user-attachments/assets/19c01db3-0279-4aec-964e-a7cc88110f2e" />


Query 7: Retrieve all orders along with the total quantity of items ordered (complex)
The query summarizes the total number of items in each order and highlights large orders, which may be for events or wholesale customers.
Inventory Management: Ensures the bakery has enough stock to meet demand.
Targeting Bulk Buyers: If businesses frequently place large orders, the bakery can offer corporate discounts or catering services.

![image](https://github.com/user-attachments/assets/14338cbc-217a-4c61-bf6b-0c78168d9687)
![image](https://github.com/user-attachments/assets/9aac6d16-5316-4de6-bd46-fe1e810e9ff1)

Query 8: Find the most used ingredient across all baked goods (complex)
The query identifies which ingredient is used the most in recipes and helps plan purchases for high-demand ingredients.
Cost Optimization: Helps negotiate bulk discounts with suppliers for the most-used ingredients.
Menu Adjustments: If an ingredient is overused and expensive, the bakery might modify recipes or adjust pricing.

![Image 3-17-25 at 9 01 PM](https://github.com/user-attachments/assets/8fd11f8b-87dc-4811-9585-2ef0082a930d)


<img width="198" alt="Screenshot 2025-03-17 at 9 24 23 PM" src="https://github.com/user-attachments/assets/e2b0c77f-4fb5-4912-aba1-a901e0f2ea5d" />


Query 9: This query finds most profitable baked goods
The subquery calculates total revenue for each baked good by: Multiplying quantityOrdered by goodPrice. Filtering only "Completed" orders. Orders the results from highest to lowest revenue. This helps the business identify which baked goods generate the most revenue, so they know which products to promote. This also supports a pricing strategy based on demand from customers.

<img width="630" alt="Screenshot 2025-03-17 at 9 15 42 PM" src="https://github.com/user-attachments/assets/2d2ed62d-6be1-42fa-aa48-d742957e3015" />
<img width="653" alt="Screenshot 2025-03-17 at 9 16 07 PM" src="https://github.com/user-attachments/assets/f30ccf15-97f9-4f65-9282-2acdcd1fe9db" />

Query 10: Retrieve the best-rated baked good based on client reviews (complex)
The query determines which baked goods have the highest customer ratings and uses a correlated subquery to dynamically calculate ratings for each item.
Menu Optimization: The bakery can highlight or promote top-rated items.
Quality Control: If an item has consistently low ratings, the bakery can improve the recipe or discontinue it.

![image](https://github.com/user-attachments/assets/0b6db900-0a86-47a8-b908-50d3ba8becc9)
![image](https://github.com/user-attachments/assets/c4e6c1a8-650d-4afb-81ea-3763d04618aa)

# Database Information 

<img width="653" alt="Screenshot 2025-03-17 at 9 28 36 PM" src="https://github.com/user-attachments/assets/f362b239-ee05-45da-a6cd-641597206b9f" />





