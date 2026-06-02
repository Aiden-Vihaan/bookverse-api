BookVerse API

A RESTful backend platform for book search, user authentication, and review management built with Node.js and Express.js.

Overview

BookVerse API is a server-side application that allows users to browse books, search by ISBN, author, or title, and manage book reviews through secure authenticated endpoints. The project demonstrates modern backend development concepts including RESTful API design, JWT authentication, asynchronous programming, and review management.

This project was developed as part of the IBM Backend Development program and enhanced with professional project organization and documentation practices.

---

Features

Public Features

- Retrieve all available books
- Search books by ISBN
- Search books by author
- Search books by title
- View reviews for specific books

User Features

- User registration
- User login
- JWT-based authentication
- Add reviews to books
- Update existing reviews
- Delete reviews

Technical Features

- RESTful API architecture
- Express.js server
- JWT authentication
- Axios integration
- Async/Await implementation
- Promise-based operations
- JSON data handling
- API documentation

---

Tech Stack

Backend

- Node.js
- Express.js

Authentication

- JSON Web Token (JWT)

Libraries

- Axios
- CORS
- Dotenv
- Morgan
- Helmet
- Nodemon

Tools

- Git & GitHub
- Postman
- cURL

---

Project Structure

bookverse-api/
│
├── controllers/
│   ├── booksController.js
│   ├── authController.js
│   └── reviewController.js
│
├── routes/
│   ├── books.js
│   ├── auth.js
│   └── reviews.js
│
├── middleware/
│   └── authMiddleware.js
│
├── data/
│   ├── booksdb.json
│   └── users.json
│
├── docs/
│   └── API.md
│
├── screenshots/
│
├── tests/
│   └── api.test.js
│
├── app.js
├── package.json
├── README.md
├── .env.example
├── nodemon.json
└── LICENSE

---

API Endpoints

Public Endpoints

Method| Endpoint| Description
GET| /books| Retrieve all books
GET| /isbn/:isbn| Search book by ISBN
GET| /author/:author| Search books by author
GET| /title/:title| Search books by title
GET| /review/:isbn| Retrieve reviews for a book

Authentication

Method| Endpoint| Description
POST| /register| Register a new user
POST| /customer/login| Login user

Protected Endpoints

Method| Endpoint| Description
PUT| /customer/auth/review/:isbn| Add or update review
DELETE| /customer/auth/review/:isbn| Delete review

---

Installation

Clone the repository:

git clone https://github.com/your-username/bookverse-api.git

Navigate into the project directory:

cd bookverse-api

Install dependencies:

npm install

Create a ".env" file using the ".env.example" template.

Run the application:

npm start

Development mode:

npm run dev

---

Testing

API endpoints can be tested using:

- Postman
- cURL
- Browser (for GET requests)

Example:

curl http://localhost:5000/books

---

Learning Outcomes

This project demonstrates:

- RESTful API Development
- Authentication and Authorization
- JWT Security
- CRUD Operations
- Asynchronous JavaScript
- Promise Handling
- API Testing
- GitHub Project Management

---

Future Improvements

- Database integration (MongoDB/PostgreSQL)
- Swagger API Documentation
- Automated Testing with Jest
- Docker Containerization
- CI/CD with GitHub Actions
- Role-Based Access Control
- Book Recommendation Engine

---

License

This project is licensed under the MIT License.

---

Author

Aiden Vihaan

