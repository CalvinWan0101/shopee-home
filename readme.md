# ShopeeHome

A full-stack e-commerce web application built as a course project for the **2023 Database Systems** course at **National Taipei University of Technology (NTUT)**. The platform supports three roles:customers, shop owners, and administrators:with a complete shopping experience including product browsing, cart management, order tracking, and coupon systems.

## Tech Stack

- **Backend**:Java 21, Spring Boot 3.2.1, Maven
- **Database**:PostgreSQL
- **Frontend (Shop)**:React 18, TypeScript, Vite, Tailwind CSS, Material-UI
- **Frontend (User)**:React 18, TypeScript, Vite, Tailwind CSS, Material-UI

## Project Structure

```text
shopee-home/
├── backend/          # Spring Boot REST API
├── frontend/
│   ├── shop/         # Shop owner management interface
│   └── user/         # Customer-facing storefront
└── readme.md
```

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

![ER Model](./backend/image/entity_relationship_model.jpg)

### Database Schema

![Database Schema](./backend/image/database_schema.png)

### Functional Dependencies

![Functional Dependencies](./backend/image/functional_dependencies.png)

## Getting Started

See the README in each subdirectory for setup and usage instructions:

- [Backend Setup](./backend/readme.md)
- [Frontend (Shop) Setup](./frontend/shop/README.md)
- [Frontend (User) Setup](./frontend/user/README.md)
