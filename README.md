Task 2 – User Authentication System
Internship: BucketStudy – Full Stack Development
Student ID: BS1765869829324
Duration: 1 Month


Project Overview
----------------
This project implements a secure user authentication system using Node.js, Express, and MongoDB.
It supports user registration, login, and protected routes using JWT-based authentication and
password hashing.


Tech Stack
----------
Backend: Node.js, Express.js
Database: MongoDB (NoSQL)
Authentication: JWT (JSON Web Tokens)
Security: bcrypt for password hashing
Tools: VS Code, Thunder Client


Project Structure
-----------------
BS1765869829324_Task2_UserAuthentication
|
|-- middleware
|   |-- authMiddleware.js
|
|-- models
|   |-- User.js
|
|-- routes
|   |-- auth.js
|
|-- screenshots
|   |-- register.png
|   |-- login.png
|
|-- server.js
|-- package.json
|-- package-lock.json
|-- README.txt


Features
--------
- User Registration
- User Login
- Password Hashing using bcrypt
- JWT Token Generation
- Protected API Routes
- Clean and modular code structure


API Endpoints
-------------

Register User
POST /api/auth/register

Request Body:
{
  "email": "user@example.com",
  "password": "password123"
}


Login User
POST /api/auth/login

Request Body:
{
  "email": "user@example.com",
  "password": "password123"
}

Response:
{
  "token": "JWT_TOKEN"
}


Protected Route
GET /api/auth/profile

Header:
Authorization: Bearer JWT_TOKEN


Environment Variables
---------------------
Create a .env file in the root directory and add:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key

Note: The .env file is not uploaded to GitHub for security reasons.


How to Run the Project
----------------------
1. Clone the repository
2. Install dependencies:
   npm install
3. Start MongoDB
4. Run the server:
   node server.js
5. Test APIs using Thunder Client or Postman


Screenshots
-----------
Screenshots of registration and login API testing are included in the screenshots folder.


Notes
-----
- This project follows security best practices
- Code is properly structured and readable
- All work is original and created for the BucketStudy internship


Conclusion
----------
This project demonstrates backend authentication skills using modern technologies and secure
coding practices as required for Task 2 of the BucketStudy Full Stack Development Internship.
