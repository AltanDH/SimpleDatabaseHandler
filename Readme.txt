Name: Altan Dogan Hoca
SID: 101311866
Assignment: Assignment 3, part 1

-- Introduction --
Context:
- This code uses JDBC and Maven to setup a connection to the postgreSQL database with Java JDK 17
- JDBC acts as an interpreter between the Java code and database
- Maven fetches the drivers required to do this (pom.xml file)
- I used IntelliJ Community Edition which simplified the setup process with Maven by automatically setting it up when
    creating the project

Documentation:
- Postgres documentation for JDBC: https://jdbc.postgresql.org/documentation/setup/
- Maven: https://mvnrepository.com/artifact/org.postgresql/postgresql/42.7.7

Prerequisites:
- Java 17 installed (will likely work with higher versions assuming backwards compatibility)
- Maven installed
- PostgreSQL
- Database exists (Mine is called: 3005A3), and is defined by you in SimpleDatabaseHandler.Java file
- PostgreSQL username and password is defined by you in SimpleDatabaseHandler.Java file

Steps to Run:
1. Create a database in Postgres using pgAdmin4
2. Run the database with the dml.sql file provided in pgAdmin4
3. Create a project in IntelliJ Community Edition with Maven selected (otherwise you're on your own)
4. Go into SimpleDatabaseHandler.Java and set your database name, username, and password (pgAdmin4 data)
5. Place the pom.xml file in the root
6. Run the SimpleDatabaseHandler.Java file


-- Files --
dml.sql:
- Rebuilds and displays the table with base tuples each time you run the file in a PostgreSQL database in pgAdmin4

pom.xml:
- File which uses Maven to help setup JDBC
- Specifies project dependencies which Maven automatically downloads

SimpleDatabaseHandler.Java
- Java class which connects to the PostgreSQL database and asks the user what kind of CRUD operation they would like to
    perform (create, read, update, delete)
- Requires the user to enter their database name, username, and password BEFORE running the code

Video Link: https://youtu.be/7DC8rvsaJ1s 


