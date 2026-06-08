# Task Management Application

A full-stack Task Management Application built using the MERN stack (MongoDB, Express.js, React, Node.js). The application allows users to register, log in, manage tasks, and perform CRUD operations with JWT-based authentication and role-based access control.

## Features

### Authentication & Authorization

* User Registration
* User Login
* Password Hashing using bcrypt
* JWT Authentication
* Protected Routes
* Role-Based Access Control (User/Admin)

### Task Management

* Create Task
* View Tasks
* Update Task Status
* Delete Task (Soft Delete)
* User-specific Tasks
* Admin Access Controls

### API Documentation

* Swagger UI Documentation
* Interactive API Testing

### Frontend

* Register Page
* Login Page
* Dashboard
* Create Task Form
* View Tasks
* Mark Task as Completed
* Delete Task
* Logout Functionality

---

## Tech Stack

### Frontend

* React.js
* React Router DOM
* Axios
* CSS

### Backend

* Node.js
* Express.js
* MongoDB Atlas
* Mongoose
* JWT
* bcryptjs
* Swagger

---

## Project Structure

```text
backend-assignment
│
├── backend
│   ├── src
│   │   ├── config
│   │   ├── controllers
│   │   ├── middleware
│   │   ├── models
│   │   ├── routes
│   │   └── app.js
│   │
│   ├── server.js
│   ├── package.json
│   └── .env
│
├── frontend
│   ├── src
│   │   ├── pages
│   │   │   ├── Login.jsx
│   │   │   ├── Register.jsx
│   │   │   └── Dashboard.jsx
│   │   ├── api.js
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

---

## API Endpoints

### Authentication

#### Register User

```http
POST /api/v1/auth/register
```

Request Body:

```json
{
  "name": "Shimpi",
  "email": "shimpi@gmail.com",
  "password": "123456"
}
```

---

#### Login User

```http
POST /api/v1/auth/login
```

Request Body:

```json
{
  "email": "shimpi@gmail.com",
  "password": "123456"
}
```

---

### Tasks

#### Create Task

```http
POST /api/v1/tasks
```

#### Get Tasks

```http
GET /api/v1/tasks
```

#### Update Task

```http
PUT /api/v1/tasks/:id
```

#### Delete Task

```http
DELETE /api/v1/tasks/:id
```

---

### Admin

#### Get All Users

```http
GET /api/v1/admin/users
```

Admin access only.

---

## Environment Variables

Create a `.env` file inside the backend folder:

```env
PORT=5001

MONGODB_URI=your_mongodb_connection_string

JWT_SECRET=your_secret_key
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/shimpi789/task-management-app.git
```

---

### Backend Setup

```bash
cd backend

npm install

npm run dev
```

or

```bash
node server.js
```

---

### Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

---

## Swagger Documentation

After starting the backend server:

```text
http://localhost:5001/api-docs
```

Swagger provides interactive API documentation and testing.

---

## Security Features

* Password Hashing using bcrypt
* JWT Authentication
* Protected Routes
* Role-Based Authorization
* Ownership Validation for Tasks
* Environment Variables for Sensitive Data

---

## Future Improvements

* Task Categories
* Task Due Dates
* Search and Filtering
* Pagination
* Dark Mode
* Email Notifications
* Deployment using Render/Vercel

---

## Author

Shimpi Rajawat

Computer Science Engineering Student

Jabalpur Engineering College
