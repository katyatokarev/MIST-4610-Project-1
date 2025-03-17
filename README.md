### MIST-4610-Project-1

# Group Name 
21482 Group 2

# Group Members

1. Rachel Cox @rachellcox
2. Jack Delinsky @JackDelinsky
3. Summer Arrington @SummerA100
4. Nivedita Ganesan
5. Katya Tokarev @katyatokarev

# Project Description
  We were tasked with designing a data model, converting it to a relational database, inputting data, and writing
queries for the data for a bakery store. The bakery store has a structure within itself, including the customers and employees as well as necessary equipment to bake the goods.
As with any business, there are orders and details regarding transactions to keep track of. And the supplies for the bakery are sourced from another company, simulating a real world example with small businesses and supply chain relations. Throughout this problem, we dive into modeling the various entities that make up the company, generating and inputting relevant data for the entities. We then  provide functioning queries for the generated data, resulting in insights about the bakery store's functions.

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


Query 2: List all clients with their contact details, but only those who have placed an order
This query retrieves only customers who have made a purchase (ignores inactive clients) and ensures no duplicates appear in the results. This query can also help with customer retention efforts—targeting buyers for special discounts or loyalty programs, sending email promotions or follow-up messages to actual customers, and prevents marketing efforts from being wasted on clients who never made a purchase.


Query 3: Get all pending orders, sorted by most recent
This query retrieves all unfulfilled orders that are still marked as "Pending"and sorts them so that the newest orders appear first. It also ensures no orders are left waiting too long, improving customer satisfaction, helps prioritize recent and urgent orders for better workflow management, and is useful for tracking order delays and resolving bottlenecks in the baking process.
Query 4: Find all baked goods and their prices, showing only items above $4.00
This query retrieves only baked goods priced above $4.00 and sorts them from cheapest to most expensive. This query can help evaluate high-margin items to see which expensive products generate more profit, be used for pricing strategy—determining whether to increase prices, introduce discounts, or bundle items, and ensure premium-priced items are properly displayed and promoted.


Query 5: Find the total revenue generated from all transactions (complex)
The query calculates total revenue from completed sales and ensures only fully processed and completed transactions are counted.
Financial Planning: Helps bakery owners analyze weekly, monthly, or yearly income trends.
Profitability Analysis: Management can determine if they need to increase sales, adjust pricing, or introduce promotions.


Query 6: Get the number of orders placed by each client (complex)
The query identifies repeat customers and how often they place orders and helps understand customer loyalty and purchasing patterns. 
Customer Retention: The bakery can offer discounts or loyalty rewards to frequent buyers.
Personalized Marketing: If a customer consistently orders croissants, the bakery can suggest new pastry items they might like.


Query 7: Retrieve all orders along with the total quantity of items ordered (complex)
The query summarizes the total number of items in each order and highlights large orders, which may be for events or wholesale customers.
Inventory Management: Ensures the bakery has enough stock to meet demand.
Targeting Bulk Buyers: If businesses frequently place large orders, the bakery can offer corporate discounts or catering services.


Query 8: Find the most used ingredient across all baked goods (complex)
The query identifies which ingredient is used the most in recipes and helps plan purchases for high-demand ingredients.
Cost Optimization: Helps negotiate bulk discounts with suppliers for the most-used ingredients.
Menu Adjustments: If an ingredient is overused and expensive, the bakery might modify recipes or adjust pricing.


Query 9: List employees along with the total number of shifts they have worked (complex)
This query tracks how many shifts each employee has worked and ensures fair workload distribution among staff.
Payroll & Overtime Management: Helps track who has worked extra hours and if overtime pay is required. Allows management to see which employees have not worked as many shifts which may lead to cutting employees or hiring new ones.
Scheduling Efficiency: Prevents overworking employees while ensuring enough coverage for busy hours.

Query 10: Retrieve the best-rated baked good based on client reviews (complex)
The query determines which baked goods have the highest customer ratings and uses a correlated subquery to dynamically calculate ratings for each item.
Menu Optimization: The bakery can highlight or promote top-rated items.
Quality Control: If an item has consistently low ratings, the bakery can improve the recipe or discontinue it.

# Database Information 

<img width="639" alt="Screenshot 2025-03-17 at 2 32 53 PM" src="https://github.com/user-attachments/assets/b11f4a48-a40a-41dc-82b6-b1058ae6a4dc" />

<img width="629" alt="Screenshot 2025-03-17 at 2 33 06 PM" src="https://github.com/user-attachments/assets/8cef809c-a2f3-44e9-b9f6-90b918ad6ecc" />




