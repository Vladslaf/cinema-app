# BASIC CINEMA APPLICATION
![drawing](https://cdn.pixabay.com/photo/2016/11/16/11/29/coupon-1828620_960_720.png)
---
### The diagram below shows entity relations
![pic](src/main/resources/images/Cinema_Entities.png)
---
## OERVIEW
#### Project is based on 3-layered architecture:
- Data access layer
- Application layer
- Presentation layer
---
#### Technologies used
- Spring (MVC, Security, Сore)
- Hibernate ORM
- Apache Tomcat - version 9.0.63
- MySQL - version 8.0.29
- Project builder: Apache Maven
---
#### Endpoints with user and admin access

- POST: /register - all
- GET: /cinema-halls - user/admin
- POST: /cinema-halls - admin
- GET: /movies - user/admin
- POST: /movies - admin
- GET: /movie-sessions/available - user/admin
- POST: /movie-sessions - admin
- PUT: /movie-sessions/{id} - admin
- DELETE: /movie-sessions/{id} - admin
- GET: /orders - user
- POST: /orders/complete - user
- PUT: /shopping-carts/movie-sessions - user
- GET: /shopping-carts/by-user - user
- GET: /users/by-email - admin
---
# Installation

### **Clone this project**

Сlone this project, and you are already halfway there :)

### **Apache Tomcat**

You need to install Apache Tomcat version 9.0.63 or latest on your computer as a web server.

### **MySQL**

Third things what you need is MySQL.

# Other informations and helpful tips

⚠️ If you wanna connect my project to your database, just add all the necessary information in the application.properties


```
Database properties

db.driver= DB DRIVER
db.url=DB URL
db.user=YOUR USERNAME
db.password=YOUR PASSWORD
#Hibernate properties
hibernate.show_sql=true
hibernate.hbm2ddl.auto=create
hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
```
After running the application you will be redirected to login page. You can use:
- username admin@i.ua with password admin123 to login as admin
- username user@i.ua with password user123 to login as user