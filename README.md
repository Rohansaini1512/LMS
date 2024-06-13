# Learning Management System (LMS) Backend

This repository contains the backend code for a Learning Management System (LMS). The backend is built using Node.js, Express, and MongoDB. It provides APIs for user authentication, course management, and basic CRUD operations.

## Features

- User registration and authentication
- Course creation, retrieval, updating, and deletion
- User roles (admin and student)
- Secure password hashing
- Token-based authentication

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT (JSON Web Token)
- Bcrypt.js

## Getting Started

### Prerequisites

- Node.js
- MongoDB

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Rohansaini1512/LMS.git
    cd lms-backend
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Create a `.env` file in the root directory and add the following environment variables:

    ```env
    PORT=5000
    MONGO_URI=your_mongodb_uri
    JWT_SECRET=your_jwt_secret
    ```

4. Start the server:

    ```bash
    npm run dev
    ```

    The server will start on `http://localhost:5000`.


### API Endpoints

#### Auth Routes

- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Authenticate a user and get a token

#### Course Routes

- `POST /api/courses` - Create a new course (admin only)
- `GET /api/courses` - Get all courses
- `GET /api/courses/:id` - Get a course by ID
- `PUT /api/courses/:id` - Update a course by ID (admin only)
- `DELETE /api/courses/:id` - Delete a course by ID (admin only)

#### User Routes

- `GET /api/users` - Get all users (admin only)
- `GET /api/users/:id` - Get a user by ID (admin only)
- `PUT /api/users/:id` - Update a user by ID (admin only)
- `DELETE /api/users/:id` - Delete a user by ID (admin only)

### Sample .env File

```env
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret


