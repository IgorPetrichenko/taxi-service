# taxi-service

Project description:
Taxi-Service is service for a taxi drivers, where drivers can register his own car, add another drivers who can work on this car, add information about manufacturer etc.

Features:
- registration like a driver;
- authentication like a driver;
- create/update/remove a car;
- create/update/remove a driver;
- create/update/remove a manufacturer;
- display list of all information about - car, manufacturer and driver

Used technology:
- Java 11
- Tomcat
- Amazon AWS (Elastic BeanStalk + RDS): hosting + DB
- MySQL
- HTML 

Instructions to run the project:
To start this project you need to do next steps:

Install and configure Apache Tomcat 9.0.65
Install MySQL and MySQL Workbench
Use the script from "src/main/resources/init_db.sql" to create schema and all tables.
Set credentials of your MySQL DB in "src/main/java/taxi/util/ConnectionUtil.java"
Add new run configuration in IDEA:
Run -> Edit configurations... -> Add new run configuration... -> Tomcat Server -> Local -> Fix -> Select "my-taxi-service:war exploded" (In graph "Application context" must be the only "/")
Run.
You can test my web-application: http://taxiservice-env.eba-tqqh3upt.us-east-1.elasticbeanstalk.com/login
