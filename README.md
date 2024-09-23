# Product Rebalancing Management System

## Overview
The **Product Rebalancing Management System** is a web-based application designed to help businesses manage their inventory across multiple stores effectively. It provides functionalities for adding, updating, and viewing products and stores, as well as redistributing stock based on store capacities.

## Features

### Store Management:
- Add, remove, and view stores.
- Manage store capacities and current stock levels.

### Product Management:
- Add, update, and remove products.
- View product details and quantities across stores.

### Stock Management:
- Add and remove stock from stores.
- Ensure stock levels do not exceed store capacities.

### Product Rebalancing:
- Automatically rebalance products across stores based on their capacities.

## Technologies Used

- **Backend**: Spring Boot
- **Frontend**: HTML, CSS, JavaScript
- **Database**: MySQL
- **IDE (Backend)**: IntelliJ IDEA
- **IDE (Frontend)**: Visual Studio Code

## Getting Started

### Prerequisites
- Java 11 or higher
- Maven
- MySQL Database
- IntelliJ IDEA

### Configure Database Connection
1. Open the `src/main/resources/application.properties` file.
2. Update the following properties:
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/productrebalancing?createDatabaseIfNotExist=true
    spring.datasource.username=user-id
    spring.datasource.password=your-password
    spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
    spring.jpa.hibernate.ddl-auto=update
    spring.h2.console.enabled=true
    spring.jpa.show-sql=true
    spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
    logging.level.org.springframework=DEBUG
    logging.level.com.ProductRebalancing=DEBUG
    ```

### Running the Application

#### Backend:
1. Open IntelliJ IDEA.
2. Import the project and ensure all dependencies are set up (you can use Spring Initializr to generate the initial project).
3. Navigate to `src/main/java/com/ProductreBalancing/ProductRebalancing/ProductRebalancingApplication.java`.
4. Run the Spring Boot application.

#### Frontend:
1. Open the `index.html` file in Visual Studio Code.
2. You can use Live Server or open the HTML file directly in a web browser to view the application.
