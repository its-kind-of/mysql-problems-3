# mysql-problems-3
1. Write a stored procedure that accepts the month and year as inputs and prints the
ordernumber, orderdate and status of the orders placed in that month.
Example: call order_status(2005, 11);
2. Write a stored procedure to insert a record into the cancellations table for all cancelled
orders.<br>
>STEPS:<br>
a. Create a table called cancellations with the following fields
id (primary key),
customernumber (foreign key - Table customers),
ordernumber (foreign key - Table Orders),
comments<br>
All values except id should be taken from the order table.<br>
b. Read through the orders table . If an order is cancelled, then put an entry in the
cancellations table.<br>
3. Solve following problems <br>
> a. Write function that takes the customernumber as input and returns the
purchase_status based on the following criteria . [table:Payments]
if the total purchase amount for the customer is < 25000 status = Silver, 
amount between 25000 and 50000, status = Gold
if amount > 50000 Platinum <br>
b. Write a query that displays customerNumber, customername and purchase_status from
customers table.

4. Replicate the functionality of 'on delete cascade' and 'on update cascade' using triggers
on movies and rentals tables. Note: Both tables - movies and rentals - don't have primary or
foreign keys. Use only triggers to implement the above.
5. Select the first name of the employee who gets the third highest salary. [table: employee]
6. Assign a rank to each employee based on their salary. The person having the highest
salary has rank 1. [table: employee]
