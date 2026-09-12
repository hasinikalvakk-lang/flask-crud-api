# Flask CRUD REST API

A simple **CRUD REST API** built using **Python, Flask, SQLAlchemy, PostgreSQL, and Docker**.

This project was created by following a Flask REST API tutorial and practicing how to build and test API endpoints.

## 🛠️ Technologies Used

- Python
- Flask
- Flask-SQLAlchemy
- PostgreSQL
- Docker & Docker Compose
- REST API
- Postman

## ✨ Features

- Create products using a REST API
- Read product data
- Update product data
- Delete product data
- Database integration using PostgreSQL
- SQLAlchemy ORM for database operations
- Dockerized application
- API testing using Postman

## 📂 Project Structure

```text
flask-crud-api/
│
├── app.py
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── screenshots/
    ├── postman-product-created.png
    └── test-route.png
```

## 🚀 Running the Project

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

### 2. Start the Flask application

```bash
docker compose up flask_app
```

The API runs on:

```text
http://localhost:4000
```

## 🧪 Testing the API

The API can be tested using **Postman**.

### Test Route

Open:

```text
http://localhost:4000/test
```

Expected response:

```json
{
  "message": "test route"
}
```

![Test Route](<img width="800" alt="Test Route" src="https://github.com/user-attachments/assets/91ac154c-f6fc-4809-8992-f937761a5d50" />
)

### Create a Product

**Method:** `POST`

**URL:**

```text
http://localhost:4000/products
```

**Body → raw → JSON:**

```json
{
  "name": "hp",
  "price": "999999"
}
```

Expected response:

```json
{
  "message": "product created"
}
```

![Product Created in Postman](<img width="800" alt="Postman API Test" src="https://github.com/user-attachments/assets/d2bea76b-5833-4dbd-b76d-24dd0ca949b9" />
)

## 🔄 CRUD Operations

| Operation | HTTP Method | Endpoint |
|---|---|---|
| Create | POST | `/products` |
| Read | GET | `/products` |
| Update | PUT | `/products/<id>` |
| Delete | DELETE | `/products/<id>` |

## 🗄️ Database

The project uses **PostgreSQL** as the database and **SQLAlchemy** to communicate with the database from Flask.

Docker Compose is used to run the application and database services together.

## 📌 Learning Outcomes

Through this project, I practiced:

- Building REST APIs with Flask
- Understanding CRUD operations
- Connecting Flask with PostgreSQL
- Using SQLAlchemy ORM
- Working with Docker and Docker Compose
- Testing APIs using Postman
- Sending and receiving JSON data

## 👩‍💻 Author

**Kalva Hasini**

---

⭐ If you find this project useful, feel free to star the repository!
