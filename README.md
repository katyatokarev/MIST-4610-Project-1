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
As with any business, there are orders and details about those to keep track of. And the supplies for the bakery are sourced from another company, simulating a real world 
example with small businesses and supply chain relations. Throughout this problem, we dive into modeling the various entities that make up the company, generating and inputting relevant data for the entities. We then  provide functioning queries for the generated data, resulting in insights about the bakery store's functions.

# Data Model Description
 Our model is based on a bakery store’s internal structure. The product entity represents the baked goods that our bakery is selling, which is connected to a supplier with a one to many relationship, since one supplier can supply multiple different products to the bakery. The ingredients are also connected to the supplier, with one supplier supplying multiple ingredients, which are later used in the recipe creating another one-to-many relationship between recipe to ingredients and a one-to-one relationship between recipe and products. 
 
Also, our model has an entity for employees, who have a schedule (with the one-to-one relationship) and also a customer that they are assigned to for the order. Our customer entity has many relationships with different entities in our data model. There is a one-to-one relationship between customers and employees, a one-to-many relationship between customers and orders (as customers can have many orders), a one-to-one relationship between customers and payments (a customer can make one payment and a payment can be made by one customer), and a one-to-many relationship between reviews. Reviews is a unique entity for our business situation. 

We chose these entities because they mirror the everyday operations of your typical bakery. 
<img width="625" alt="Screenshot 2025-03-17 at 1 55 29 PM" src="https://github.com/user-attachments/assets/c962c9ba-c7a9-40f6-ad04-afca9d0aadba" />


# Data Dictionary
  Here is the data dictionary for our model.

  
  <img width="630" alt="Screenshot 2025-03-17 at 2 13 04 PM" src="https://github.com/user-attachments/assets/2e4a854d-8fcd-4264-b1b0-627441709049" />

<img width="632" alt="Screenshot 2025-03-17 at 2 14 23 PM" src="https://github.com/user-attachments/assets/c722b103-7950-4cec-be16-f97921408544" />


<img width="658" alt="Screenshot 2025-03-17 at 2 14 39 PM" src="https://github.com/user-attachments/assets/863a0ec6-e0b9-41bb-ae73-f5b9a701bd87" />

<img width="674" alt="Screenshot 2025-03-17 at 2 14 55 PM" src="https://github.com/user-attachments/assets/801595fe-d387-409a-a203-9caa4c4ccb18" />

<img width="644" alt="Screenshot 2025-03-17 at 2 15 34 PM" src="https://github.com/user-attachments/assets/ef45046c-27c7-4766-aba4-468ebdda1634" />

<img width="675" alt="Screenshot 2025-03-17 at 2 15 40 PM" src="https://github.com/user-attachments/assets/70329a5c-8463-4dca-9dd2-b51faddd4f8d" />






