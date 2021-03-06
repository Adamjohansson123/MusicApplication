# MusicApplication

Link to heroku MusicApplication: https://music-application.herokuapp.com/home

About the application
-

This is a project that me and a coworker made as an assignment at Experis Academy. 
The assignment was to create a Spring Boot Application using Java containing an REST API, multiple Thymeleaf views and SQLite database. 
The goal was to create different endpoints for the REST API to get different types of data from our SQLite database. 
The Thymeleaf views were supposed to display random data from the database and you were also supposed to be able to search for different types of data.

Endpoints requirements
-
Endpoints must be on a /api/ sub directory in your applications structure. Meaning, “/” and “/search?term=foo” are for the Thymeleaf pages and “/api/bar” 
is for the REST endpoints. The endpoints should be designed with best practices in mind. The endpoints should be named appropriately; remember, nouns not verbs. 
Provide a collection of API calls made in Postman to test the endpoints (done by creating a collection and exporting It as JSON).

REST API requirements
-
For customers in the database, the following functionality should be catered for:

1. Read all the customers in the database, this should display their: Id, first name, last name, country, postal code, phone number and email.

2. Read a specific customer from the database (by Id), should display everything listed in the above point.

3. Read a specific customer by name. HINT: LIKE keyword can help for partial matches.

4. Return a page of customers from the database. This should take in limit and offset as parameters and make use of the SQL keywords to get a subset of the customer data. The customer model from above should be reused.

5. Add a new customer to the database. You also need to add only the fields listed above (our customer object). 

6. Update an existing customer.

7. Return the number of customers in each country, ordered descending (high to low). i.e. USA: 13, ... 

8. Customers who are the highest spenders (total in invoice table is the largest), ordered descending. 

9. For a given customer, their most popular genre (in the case of a tie, display both). Most popular in this context means the genre that corresponds to the most tracks from invoices associated to that customer.

Data Access Requirements
-
You are encouraged to implement the repository pattern in this assignment. The version of the pattern to implement is up to you. 
This is not a requirement, but is little extra work that prepares you for structures we will see in the future.
