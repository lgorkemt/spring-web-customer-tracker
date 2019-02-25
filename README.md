. The application is a simple CRM web application for allowing user to make CRUD operations on a list of customers. It
runs on Amazon Elastic Beanstalk web service and running on the url; 

http://web-customer-tracker-06.us-east-2.elasticbeanstalk.com/

. A Mysql DB for the appication is running on the RDS Amazon web service.
 
. You may also make a local database installation. (MySQL can be downlaoded from http://dev.mysql.com/downloads)
In this case change  springonaws-db.cyedmhnitszb.us-east-2.rds.amazonaws.com part to localhost in both of the mysql 
properties file under resources. 

. To install a local database;

Open MySql workbench and run three scripts respectively; 
    01-create-user.sql, 
    02-customer-tracker.sql, 
    03-setup-spring-security-bcrypt-demo-database 

These scripts would create a db user called springstudent, create the DB schema called web_customer_tracker, 
create a Customer table, populate the Customer table and create user and role tables that would be used in authentication 
and authorization.

. Open the source code for the appropriate version

. To run the application locally: 
   a. Select the root project folder
   b. Right-Click, select Run As > Run On Server (A tomcat server should have been installed in your local machine)
   c. The application is secured by using Spring security, for all available users and roles you may look at the .sql 
   script 03-setup-spring-security-bcrypt-demo-database.sql. (The password for all the users are 'fun123')
   
. Also aspects are added for logging the CRUD actions. You may check your console after each action for
the logs written by the aspects.
