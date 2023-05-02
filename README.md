Download Link: https://assignmentchef.com/product/solved-cis560-homework-2
<br>
Submit a query for each of the following questions. All queries will be solutions against the <strong>WideWorldlmporters </strong>database. You are only to use constructs covered in class through the topic of JOINs. <em>Your solutions should not include subqueries.</em>

<strong>Question 1</strong>

Write a query that will return sales information for each customer category and year. The columns required in the result set are:

<ul>

 <li><strong>OrderYear – </strong>The year the orders were placed.</li>

 <li><strong>CustomerCategoryName – </strong>As it appears in the table <em>CustomerCategories.</em></li>

 <li><strong>CustomerCount – </strong>The number of unique customers placing orders for each <em>CustomerCategoryName </em>and</li>

 <li><strong>OrderCount – </strong>The number of orders placed for each <em>CustomerCategoryName </em>and</li>

 <li><strong>Sales – </strong>The subtotal from the orders placed, calculated from <em>Quantity </em>and <em>UnitPrice </em>of the table <em>OrderLines.</em></li>

 <li><strong>AverageSalesPerCustomer – </strong>The average sales per customer for each <em>CustomerCategoryName </em>and</li>

</ul>

The results should be sorted in ascending order, first by order year, then by customer category name.

<strong>Question 2</strong>

Write a query that will return sales for 2014 and 2015, with each year’s sales in a separate column. We should only have one row for each customer who placed an order in 2014 or 2015.

The columns required in the result set are:

<ul>

 <li><strong>CustomerlD – </strong>As it is in the table <em>Customers.</em></li>

 <li><strong>CustomerName – </strong>As it is in the table <em>Customers.</em></li>

 <li><strong>2014Sales – </strong>The total sales for the customer in 2014.</li>

 <li><strong>2015Sales – </strong>The total sales for the customer in 2015.</li>

 <li><strong>TotalSales – </strong>The total sales for the customer in both years.</li>

</ul>

The three sales columns are calculated from <em>Quantity </em>and <em>UnitPrice </em>of the table <em>Sales.OrderLines. </em>Also note that an identifier starting with a digit is irregular, which requires square brackets or double quotes as a delimiter.




11/12/2018                                                                                                                                                                                        Homework 2

The results should be sorted with the highest total sales at the top, and if two customers have the same total, use the <em>CustomerlD </em>in ascending order to make the results deterministic.

<strong>Question 3</strong>

Write a query to return 2015 sales information for each supplier. We would like to include <strong>all suppliers </strong>in the result set, regardless of whether their products were sold in 2015.

Sales are determined using <em>Sales.Orders </em>and <em>Sales.OrderLines </em>as in the previous two questions. However, since we are asking for this information from the perspective of the supplier, you also need to use the tables <em>Warehouse.Stockltems </em>and <em>Purchasing.Suppliers. </em>To better understand a table structure, see<strong><u> Browsing  Table Structures.</u></strong>

The columns required in the result set are:

<ul>

 <li><strong>SupplierlD – </strong>As it appears in the table <em>Suppliers.</em></li>

 <li><strong>SupplierName – </strong>As it appears in the table <em>Suppliers.</em></li>

 <li><strong>OrderCount </strong><strong>– </strong>The number of orders placed on products for each supplier.</li>

 <li><strong>Sales </strong><strong>– </strong>The subtotal from the orders placed, calculated from <em>Quantity </em>and <em>UnitPrice </em>of the table <em>OrderLines.</em></li>

</ul>

The results should be sorted such that the supplier with the highest sales is at the top. If two suppliers have the same sales, next use the order count with the highest count at the top. If two suppliers have the same sales and order count, use the supplier name in ascending order as the final tie breaker. This will ensure a deterministic result.

<strong>Submission</strong>

Please submit your solution to each question in a single SQL file. Include a comment line above each solution indicating which question it answers. Please do not submit your results, only the SQL solutions.