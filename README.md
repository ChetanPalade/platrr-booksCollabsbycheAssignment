# platrr-booksCollabsbycheAssignment
This Collaborative Book List App is a full-stack project that demonstrates how to build a responsive, modern, and dynamic web application. The use of React.js for the frontend and Node.js with Express for the backend showcases the flexibility of the MERN stack. By adding features like animations, user interactions, and a polished UI, we’ve created a seamless experience for users to contribute to and interact with a shared book list.
# Collaborative Book List App

  Welcome to the Collaborative Book List App! This full-stack application allows multiple users to contribute, view, upvote, and delete books in a shared book list. Users can interact with the list by adding their favorite books, providing upvotes, and removing books they no longer wish to keep. The app is designed to be responsive and visually appealing across desktop and mobile devices.

# Features
 - Book List Display: View a list of books with title, author, description (optional), and upvote count. -
 - Add New Book: Users can add books to the list, including a title, author, and an optional description.
 - Upvote Feature: Users can upvote books, increasing their visibility in the list.
 - Delete Book: Users can delete books from the list.
 - Responsive Design: The app is fully responsive, with a fluid layout optimized for both desktop and mobile devices.
 - Animations: Smooth animations and interactions using Framer Motion for a dynamic user experience.

# Technologies Used
  ## Frontend

 --> React.js: JavaScript library for building user interfaces.
 --> React Bootstrap: A UI toolkit for building responsive and attractive components.
 --> Framer Motion: A library for adding animations and transitions.
 --> CSS/Media Queries: Custom CSS with media queries for advanced responsiveness and styling.

  ## Backend
 --> Node.js: JavaScript runtime used for building the backend.
 --> Express.js: Web framework for building RESTful APIs.
 --> MongoDB: NoSQL database used for storing book data. MongoDB Atlas is recommended for hosting the database.
 --> Mongoose: ODM (Object Document Mapper) for MongoDB, used to interact with the database.

# Setup Instructions

Prerequisites
Before you start, make sure you have the following installed:

Node.js (v14 or higher)
npm or yarn
MongoDB (Local or MongoDB Atlas account)

1. Clone the Repository
Clone the repository to your local machine:

git clone https://github.com/your-username/collaborative-book-list-app.git
cd collaborative-book-list-app

2. Install Backend Dependencies
Navigate to the backend directory and install the required dependencies:

cd backend
npm install

3. Set Up Environment Variables
Create a .env file in the backend directory and set the following variables:

MONGO_URI=your-mongodb-uri
PORT=3000

Replace your-mongodb-uri with your actual MongoDB connection string. If you are using MongoDB Atlas, you can get this connection string from the MongoDB Atlas dashboard.

4. Start the Backend Server
Start the backend server using:
npm start
The backend server will be running on http://localhost:5000.

5. Install Frontend Dependencies
Navigate to the frontend directory and install the required dependencies:

cd frontend
npm install

7. Start the Frontend Server
Start the frontend development server using:

npm start

The frontend app will be running on http://localhost:3000.

# API Endpoints
The backend exposes the following RESTful API endpoints:

GET /api/books: Retrieve all books from the database.
POST /api/books: Add a new book to the list (requires title and author).
PUT /api/books/
/upvote: Upvote a book by its ID.
DELETE /api/books/
: Delete a book from the list by its ID.

Example API Request (Postman, Curl, or Axios)
# POST: Add a New Book
json

{
  "title": "The Great Gatsby",
  "author": "F. Scott Fitzgerald",
  "description": "A classic novel of the 1920s."
}

# PUT: Upvote a Book
json
{
  "upvotes": 1
}
# DELETE: Delete a Book
json
{
  "id": "book-id-here"
}
