# User Management API

## 📌 Overview
This is a **RESTful API** built using **Node.js, Express, and PostgreSQL with Sequelize ORM**. The API provides user authentication, CRUD operations, and JWT-based authentication.

## 🚀 Features
- **User Authentication** (Register, Login)
- **JWT Token Authentication**
- **CRUD Operations** for User Management
- **Pagination** for User Listings
- **Validation Middleware**
- **Swagger API Documentation**

---

## 🛠️ Tech Stack
- **Backend:** Node.js, Express.js
- **Database:** PostgreSQL with Sequelize ORM
- **Authentication:** JWT (JSON Web Token)
- **Validation:** Express Validator
- **API Documentation:** Swagger UI

---

## 📌 Installation

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-repo.git
cd restful-api
```

### 2️⃣ Install Dependencies
```sh
npm install
```

### 3️⃣ Configure Environment Variables
Create a **.env** file in the root directory and add:
```sh
PORT=5000
JWT_SECRET=your_secret_key
DATABASE_URL=your_database_connection_url
```

### 4️⃣ Run Database Migrations
```sh
npx sequelize-cli db:migrate
```

### 5️⃣ Start the Server
```sh
npm start
```

The server will start at `http://localhost:5000`.

---

## 📜 API Documentation
The API is documented using **Swagger UI**.

📄 **Visit:** [Swagger Docs](http://localhost:5000/api-docs)

---

## 🔥 API Endpoints

### **Authentication**
| Method | Endpoint        | Description             |
|--------|---------------|-------------------------|
| POST   | /users/register | Register a new user    |
| POST   | /users/login    | Login and get a token  |

### **User Management**
| Method | Endpoint       | Description            |
|--------|---------------|------------------------|
| GET    | /users        | Get all users (Paginated) |
| GET    | /users/:id    | Get user by ID         |
| POST   | /users        | Create a new user      |
| PUT    | /users/:id    | Update user details    |
| DELETE | /users/:id    | Delete a user          |

---

## 🔑 Authentication & Security
- Use JWT Token in `Authorization` header for protected routes.
- Example:
```sh
Authorization: Bearer your_jwt_token
```

---

## 📌 Running Tests
To run tests (if available), use:
```sh
npm test
```

---

## 📬 Contact
For queries, reach out to **rupendrakumar223.com@gmail.com** or open an issue on GitHub.

🚀 **Happy Coding!**

