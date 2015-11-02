# sparksports
chess tournament management application

The application was created for a final project during the winter season for KSU University, Nov 2nd 2015. 

The project is using Java 8, Spark Web Framework and Sql2o for the connection to MySQL database.

## Screenshots

### Login/Register screen 

#### Home Screen

##### Admin Screen


## Installation instructions

1. Run `Torneo.sql`
    * The script will create a MySQL schema, named `torneo` and a MySQL user `torneo` with a password `password`.    
```
mysql -u root -p < db/torneo.sql
```
2. Run `seedData_torneo.sql`    
    * The script will insert some initial data into the tables `teams`,'fixtures','user' and `ranks`.
```
mysql -u root -p < db/seedData_torneo.sql
```
3. Build project
```
mvn clean package
```
4. Run project
```
java -jar target/torneo-1.0-SNAPSHOT-jar-with-dependencies.jar
```
5. Browser automatically opens at [http://localhost:9990](http://localhost:9990), where you can start application :)

Technologies used are

1. MySQL
2. MySQL Workbench
3. JOOQ ( Java object oriented Query ) .. for scaffolding from database tables as like RoR.
4. Sql2o for database call.
5. lombok for POJO simulation without getters and setters.
6. jQuery UI as front end display
7. Maven for build and deployment
8. Jetty Server to run on dynamically from main method of a class.
9. Java 8
10.Spark REST Microservice 
