# ShopeeHome:Backend

Spring Boot REST API backend for the ShopeeHome e-commerce platform. This is a course project for the **2023 Database Systems** course at **National Taipei University of Technology (NTUT)**.

## Tech Stack

- **Language**:Java 21
- **Framework**:Spring Boot 3.2.1
- **Build Tool**:Maven
- **Database**:PostgreSQL
- **Testing**:Spring Boot Test + EZSpec

## Features

### User Actions

- Register
- Login
- Logout
- View profile
- Edit profile
- View order history
- View order detail
- Add to cart
- Remove from cart
- Checkout
- Claim coupons

### Shop Actions

- Register
- Login
- Logout
- View profile
- Edit profile
- View product list
- View product detail
- Add product
- Edit product
- Remove product
- View order list
- Update shipping status
- Add seasoning coupons
- Add shipping coupons

### Admin Actions

- Login
- Logout
- View user list
- View user detail
- View shop list
- View shop detail
- Remove user
- Remove shop

## Database Design

### Entity-Relationship (ER) Model

![ER Model](./image/entity_relationship_model.jpg)

### Database Schema

![Database Schema](./image/database_schema.png)

### Functional Dependencies

![Functional Dependencies](./image/functional_dependencies.png)

## Environment Setup

1. Install [Java 21](https://www.oracle.com/tw/java/technologies/downloads/)
2. Install [IntelliJ IDEA](https://www.jetbrains.com/idea/)
3. Install [Git](https://www.git-scm.com/download/win)
4. Install [PostgreSQL](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)
5. Create a database named `shopeehome`
6. Set the following environment variables:
   - `POSTGRES_USERNAME`:your PostgreSQL username
   - `POSTGRES_PASSWORD`:your PostgreSQL password

## Running the Project

### 1. Open in IntelliJ IDEA

Open the `backend` folder in IntelliJ IDEA.

Run **Maven Install** to download all dependencies:

![Maven Install](./image/intellij/maven_install.png)

Set the project SDK to **Java 21** under Project Structure:

![Java 21](./image/intellij/java21.png)

### 2. Connect to the Database

Configure the PostgreSQL data source in IntelliJ:

![Database Step 1](./image/intellij/database_1.png)
![Database Step 2](./image/intellij/database_2.png)
![Database Step 3](./image/intellij/database_3.png)

### 3. Create Database Tables

Locate `src/main/resources/database/create.sql` and execute it to create all tables:

![Create Database](./image/intellij/create_database.png)

### 4. Run Tests

Run all tests to verify the backend is working correctly:

![Test Run 1](./image/intellij/test_1.png)
![Test Run 2](./image/intellij/test_2.png)

### 5. Generate Demo Data

Run `TestDataGenerator` to populate the database with sample data:

![Test Data](./image/intellij/test_data.png)

### 6. Start the Server

Run the application. The server starts on `http://localhost:8080`:

![Run](./image/intellij/run.png)
