# TAXI SERVICE
## Project description
   The main purpose of this project is to simulate basic taxi service application with simple authentication system. Using this app allows you:
   * Enter into the system or register you as a new user
   * Track all available cars and drivers and manage them. 
     * Add new cars
     * Add new drivers
     * Assign a driver to one or more cars
     * Delete cars, drivers and manufacturers
## Implementation details
   Project based on 3-layer architecture:
   1. DAO
   2. Application layer - services
   3. Presentation layers - controllers
### Following diagram shows relations between Car, Driver and Manufacturer
   ![EER Diagram](https://i.ibb.co/zGMzkWs/Screenshot-16.jpg)
## Used technologies
   * Apache Tomcat (v9.0.50)
   * MySQL
   * JDBC
   * JSP
   * Maven
   * HTML, CSS
   * JSTL
## Setup recommendations
   1. Install MySQL
   2. Configure Apache Tomcat
   3. Create all necessary tables using script from `init_db.sql` file.
      **WARNING! This script will drop `taxi` schema if you have it. So be careful**
   4. Clone this project into your IDE
   5. Replace `USERNAME` and `PASSWORD` values in `src/main/java/mate/util/ConnectionUtil.java` with your data
   6. Change `src/main/resources/log4j2.xml`. At line `<File name="LogToFile" fileName="E:\Mate\Projects\taxi_service\logs\app.log">` 
replace fileName with absolute path to `.log` file
   7. Run the application


