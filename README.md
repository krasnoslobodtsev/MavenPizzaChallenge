# MavenPizzaChallenge
The Dashboard can be accessed [here](https://app.powerbi.com/groups/me/reports/eb76e1b3-d6f3-4731-9b79-7b0ba61499e3/ed762c2b4b9a3593425b?experience=power-bi)
# Case description
Project Objective – Plato’s Pizza BI Challenge

In this project, I took on the role of a Business Intelligence Consultant for Plato’s Pizza, a Greek-inspired restaurant in New Jersey. The goal was to help the business become more data-driven by analyzing customer transactions and uncovering opportunities to increase sales and improve operational efficiency.
The analysis was designed to answer key business questions, including:
- Restaurant traffic patterns – What days and times are the busiest?
- Operational load – How many pizzas are prepared during peak periods?
- Menu performance – Which pizzas are the best and worst sellers?
- Financial insights – What is the average order value?
- Capacity utilization – How effectively is the restaurant using its seating capacity (15 tables, 60 seats total)?
# About the Data Set
A year's worth of sales from a fictitious pizza place, including the date and time of each order and the pizzas served, with additional details on the type, size, quantity, price, and ingredients.
| Table              | Field              | Description                                                                                                                                  |
| ------------------ | ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **orders**         | order\_id          | Unique identifier for each order placed by a table.                                                                                          |
|                    | date               | Date when the order was placed (entered into the system before cooking & serving).                                                           |
|                    | time               | Time when the order was placed (entered into the system before cooking & serving).                                                           |
| **order\_details** | order\_details\_id | Unique identifier for each pizza item within an order. (Pizzas of the same type and size are grouped in one row, with quantity incremented). |
|                    | order\_id          | Foreign key linking order details to the main order record.                                                                                  |
|                    | pizza\_id          | Foreign key linking to the specific pizza ordered (type and size).                                                                           |
|                    | quantity           | Number of pizzas of the same type and size ordered.                                                                                          |
| **pizzas**         | pizza\_id          | Unique identifier for each pizza (combination of type and size).                                                                             |
|                    | pizza\_type\_id    | Foreign key linking each pizza to its broader pizza type.                                                                                    |
|                    | size               | Pizza size (Small, Medium, Large, X Large, or XX Large).                                                                                     |
|                    | price              | Price of the pizza in USD.                                                                                                                   |
| **pizza\_types**   | pizza\_type\_id    | Unique identifier for each pizza type.                                                                                                       |
|                    | name               | Name of the pizza as displayed on the menu.                                                                                                  |
|                    | category           | Menu category the pizza belongs to (Classic, Chicken, Supreme, or Veggie).                                                                   |
|                    | ingredients        | Comma-separated list of ingredients used in the pizza (all include Mozzarella Cheese, even if not explicitly listed).                        |

