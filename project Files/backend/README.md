# Study App Backend

A Node.js Express backend for the Study App, providing RESTful APIs for user authentication, course management, enrollment, and payments.

## Features

- User authentication (JWT)
- Role-based access (Admin, Teacher, Student)
- Course CRUD operations
- Enrollment and payment processing
- MongoDB integration via Mongoose
- Secure endpoints with middleware

## Getting Started

### Prerequisites
- Node.js (v16+ recommended)
- npm
- MongoDB instance (local or cloud)

### Installation

1. Navigate to the backend directory:
	```
	cd backend
	```
2. Install dependencies:
	```
	npm install
	```
3. Create a `.env` file in the backend directory with the following variables:
	```
	MONGO_URI=your_mongodb_connection_string
	JWT_SECRET=your_jwt_secret
	PORT=8000
	```

### Running the Server

- Start the server:
  ```
  npm run start
  ```
- For development with auto-reload:
  ```
  npm run dev
  ```

## Project Structure

- `index.js` - Entry point
- `config/` - Database connection
- `controllers/` - Route logic
- `middlewares/` - Authentication and other middleware
- `routers/` - API route definitions
- `schemas/` - Mongoose models

## API Endpoints

- `/api/user/register` - Register user
- `/api/user/login` - Login user
- `/api/user/getallcourses` - Get all courses
- `/api/user/enrolledcourse/:courseId` - Enroll in course
- `/api/user/deletecourse/:courseId` - Delete course (teacher)

## License

MIT
