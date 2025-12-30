🌟 Backend API
Backend API is a Node.js and Express-based backend project that allows user registration, login, and protected routes using JWT authentication.
It is connected to MongoDB for storing user data.

This project is designed as an individual learning task to strengthen API development skills.

✨ Features

User registration (/api/auth/register)

User login (/api/auth/login) with JWT authentication

Protected routes for user profile (/api/users/profile)

MongoDB integration with Mongoose

Error handling middleware

🛠 Technologies Used

Node.js

Express.js

MongoDB / Mongoose

JWT (JSON Web Token)

dotenv

🚀 Installation

1.Clone the repository

git clone https://github.com/laviee143/taskboot2.git
cd taskboot2


2.Install dependencies

npm install


3.Create a .env file in the root folder

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key


4.Start the server

node server.js
nodemon server.js

📡 API Endpoints

✅ Root Route
GET /


Response:

{
  "message": "API is running successfully"

  🔑 Auth Routes
Method	Endpoint            Description
POST	/api/auth/register    Register a new user
POST	/api/auth/login       Login user & return JWT token

taskboot/
│
├── controllers/
│   ├── authController.js
│   └── userController.js
│
├── routes/
│   ├── authRoutes.js
│   └── userRoutes.js
│
├── middleware/
│   └── errorMiddleware.js
│
├── config/
│   └── db.js
│
├── .env
├── package.json
└── server.js

⚡ Usage

Start MongoDB locally or connect to Atlas.

Start server using node server.js.

Test endpoints using Postman.

Use JWT token for protected routes.
  
