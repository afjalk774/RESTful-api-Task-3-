# RESTful-api-Task-3-
# Blog Posts RESTful API
A RESTful API for managing blog posts, built with Node.js, Express, and MongoDB. This API allows users to perform CRUD operations on blog posts with a clean and scalable architecture.


📌 Features
✅ Create, Read, Update, and Delete (CRUD) blog posts

🔐 JWT-based authentication for protected routes (optional)

🧑 User model with registration & login (optional)

📂 MongoDB for data persistence

📄 Pagination and filtering support

🔍 Search posts by title or content

🧪 Ready for testing with tools like Postman

🛠️ Tech Stack
Node.js – Runtime

Express – Web framework

MongoDB + Mongoose – Database and ODM

dotenv – Environment variable management

cors – Cross-origin requests

body-parser – Parsing request bodies

(Optional: bcrypt, jsonwebtoken, multer, etc.)

📦 Installation
Clone the repository


Install dependencies

bash
Copy
Edit
npm install
Create a .env file

env
Copy
Edit
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
Start the server

bash
Copy
Edit
npm start
Server will run on http://localhost:5000 by default.

🔗 API Endpoints
Public
Method	Endpoint	Description
GET	/api/posts	Get all blog posts
GET	/api/posts/:id	Get a single blog post

Protected (JWT)
Method	Endpoint	Description
POST	/api/posts	Create a new post
PUT	/api/posts/:id	Update a post
DELETE	/api/posts/:id	Delete a post

(Optional: Include user endpoints if implementing authentication)

🧪 Testing
You can use Postman or cURL to test the API:

bash
Copy
Edit
curl http://localhost:5000/api/posts
🧱 Database Schema Example
js
Copy
Edit
{
  title: String,
  content: String,
  author: String,
  createdAt: Date,
  updatedAt: Date
}
