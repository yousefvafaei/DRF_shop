# DRF_shop API

DRF_shop API is a Django Rest Framework (DRF) based backend for an e-commerce platform. It supports functionalities including product management, cart operations and order processing.

---

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [API Endpoints](#api-endpoints)
    - [Product Endpoints](#product-endpoints)
    - [Category Endpoints](#category-endpoints)
    - [Comment Endpoints](#comment-endpoints)
    - [Cart Endpoints](#cart-endpoints)
    - [Customer Endpoints](#customer-endpoints)
    - [Order Endpoints](#order-endpoints)
---

## Installation

To get started with TechnoShop API, follow these steps:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yousefvafaei/DRF_shop.git
    cd DRF_shop
    ```

2. **Create and activate a virtual environment using pipenv:**
    ```bash
    pipenv install
    pipenv shell
    ```

3. **Apply the migrations:**
    ```bash
    python manage.py migrate
    ```

4. **Create a superuser:**
    ```bash
    python manage.py createsuperuser
    ```

5. **Run the development server:**
    ```bash
    python manage.py runserver
    ```

---

## Usage

Use the provided API endpoints to interact with the TechnoShop platform. Tools like Postman or curl can be used to test the endpoints.

---

## API Endpoints

### Product Endpoints

- **List Products**: `GET /store/products/`
- **Retrieve a Product**: `GET /store/products/{id}/`
- **Create a Product**: `POST /store/products/`
- **Update a Product**: `PUT /store/products/{id}/`
- **Delete a Product**: `DELETE /store/products/{id}/`

### Category Endpoints

- **List Categories**: `GET /store/categories/`
- **Retrieve a Category**: `GET /store/categories/{id}/`
- **Create a Category**: `POST /store/categories/`
- **Update a Category**: `PUT /store/categories/{id}/`
- **Delete a Category**: `DELETE /store/categories/{id}/`

### Comment Endpoints

- **List Comments for a Product**: `GET /store/products/{product_id}/comments/`
- **Create a Comment for a Product**: `POST /store/products/{product_id}/comments/`

### Cart Endpoints

- **Retrieve a Cart**: `GET /store/carts/{id}/`
- **Create a Cart**: `POST /store/carts/`
- **Delete a Cart**: `DELETE /store/carts/{id}/`

### Customer Endpoints

- **Retrieve Current Customer**: `GET /store/customers/me/`
- **Update Current Customer**: `PUT /store/customers/me/`

### Order Endpoints

- **List Orders**: `GET /store/orders/`
- **Retrieve an Order**: `GET /store/orders/{id}/`
- **Create an Order**: `POST /store/orders/`
- **Update an Order**: `PATCH /store/orders/{id}/`
- **Delete an Order**: `DELETE /store/orders/{id}/`

---
