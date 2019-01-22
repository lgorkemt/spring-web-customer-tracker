. The application is a simple CRM web application for allowing user to make CRUD operations on a list of customers.
The code is written by using Chad Darby's Udemy course on Spring framework (https://www.udemy.com/spring-hibernate-tutorial/)

. A Mysql DB and workbench should be installed to the local machine which the application is going to run. (MySQL can be 
downlaoded from http://dev.mysql.com/downloads)

. Open MySql workbench and run three scripts respectively; 
    01-create-user.sql, 
    02-customer-tracker.sql, 
    03-setup-spring-security-bcrypt-demo-database 

These sripts would create a db user called springstudent, create the DB schema called web_customer_tracker, 
create a Customer table, populate the Customer table and create user and role tables that would be used in authentication a
nd authorization.

. Open the source code for the appropriate version

. Run the application: 
   a. Select the root project folder
   b. Right-Click, select Run As > Run On Server (A tomcat server should have been installed in your local machine)