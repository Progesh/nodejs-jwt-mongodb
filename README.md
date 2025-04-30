# Node.js JWT Authentication with MongoDB
This project provides a foundational setup for generating JSON Web Tokens (JWT) to access RESTful APIs using Node.js and MongoDB. The application is built with Express.js and includes user authentication functionality.

## Features
- User Authentication: Secure user login and registration using JWT.
- API Endpoints: RESTful APIs for user management and authentication.
- Database Integration: MongoDB for data storage.
- Dependencies:
  - bcryptjs for password hashing.
  - body-parser for parsing request bodies.
  - express for server setup.
  - jsonwebtoken for token generation and validation.
  - mongoose for MongoDB interaction.

## Installation

1. Clone the repository:

bash
git clone https://github.com/Progesh/nodejs-jwt-mongodb.git
cd nodejs-jwt-mongodb

<pre> ```bash git clone https://github.com/Progesh/nodejs-jwt-mongodb.git cd nodejs-jwt-mongodb ``` </pre>

2. Install the dependencies:

bash
npm install

3. Start the MongoDB server:

bash
mongod

4. Start the Node.js server:

bash
node server.js

5. Test the APIs using tools like Postman.

## Project Structure
- app.js: Main application entry point. Configures routes for user and authentication functionalities.
- user/UserController.js: Handles user-related routes and operations.
- auth/AuthController.js: Implements authentication logic, including login and token validation.
- db.js: Database connection setup for MongoDB.

## API Endpoints

### User Routes
- POST /users/register: Register a new user.
- GET /users: Retrieve a list of users.

### Authentication Routes
- POST /api/auth/login: User login and token generation.
- GET /api/auth/validate: Validate a JWT.
