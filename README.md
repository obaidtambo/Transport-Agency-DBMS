# Transport Agency DBMS
 SQL for Transport Agency Database.
PostgreSQL code written in Notebook format.


You need to have a  Postgres installed on your system to run your code

 The following is the ER diagram of the Database showing all the relationships between the different  Tables.

![DBMS](https://user-images.githubusercontent.com/80193224/206838148-0949b400-af17-487b-a60b-50826799936d.png)

 
## Introduction
A transport company mainly deals with shipment of goods from source location to destination location
through various available logistics. Finding out optimal route and logistics combinations is one of the key
challenges of this system. Apart from this, it also handles tasks such as taking order from customers,
creating automated billing system for their service, tracking or updating shipment status of customers’
good etc. 

ER diagram and the transport company database follow the following design specifications.


Design of the database:
In this project, several databases are required to hold following information :
*  Information of all available logistics which includes their type such as truck,rail etc and
capacity their unique id, their present location and status.
*  Information of all registered customers ;their credentials and each customer is assigned a
unique id.
*  Information about cargo/goods like Its id, the customer-id of the customer who placed the
order. its destination, logistic id of the logistics carrying the cargo/goods and status of
customer's’ order etc.
*  Billing information of every order: the order-id for which the billing is done, the customer-id,
cost and the status of payment.
*  Schedule for the different logistics on different working days; it will include the logistic -id,
departure day, source location, destination , route id .
*  Route information of the different routes from one city to another. This includes identifying
intermediate stations of a route. Finding the total cost of that route in terms of distance.
* Administrator and employee information for accessing the database and updating order
status.
*  On-route information which will give us information of all on-route logistics; it will contain
the logistic-id, time of departure, source , destination, its present location and status.
