![Screenshot (1403)](https://github.com/user-attachments/assets/f774975c-22a0-4bff-8483-10ce26604fde)## Collaborative Book List App

Welcome to the Collaborative Book List App! This full-stack application allows multiple users to contribute, view, upvote, and delete books in a shared book list. Users can interact with the list by adding their favorite books, providing upvotes, and removing books they no longer wish to keep. The app is designed to be responsive and visually appealing across desktop and mobile devices.

# Features

--> Book List Display: View a list of books with title, author, description (optional), and upvote count.
--> Add New Book: Users can add books to the list, including a title, author, and an optional description.
--> Upvote Feature: Users can upvote books, increasing their visibility in the list.
--> Delete Book: Users can delete books from the list.
--> Responsive Design: The app is fully responsive, with a fluid layout optimized for both desktop and mobile devices.
--> Animations: Smooth animations and interactions using Framer Motion for a dynamic user experience.

# Technologies Used
  ## Frontend
-->  React.js: JavaScript library for building user interfaces.
-->  React Bootstrap: A UI toolkit for building responsive and attractive components.
-->  Framer Motion: A library for adding animations and transitions.
-->  CSS/Media Queries: Custom CSS with media queries for advanced responsiveness and styling.
  ## Backend
-->  Node.js: JavaScript runtime used for building the backend.
-->  Express.js: Web framework for building RESTful APIs.
-->  MongoDB: NoSQL database used for storing book data. MongoDB Atlas is recommended for hosting the database.
-->  Mongoose: ODM (Object Document Mapper) for MongoDB, used to interact with the database.

#  Setup Instructions
-->  Prerequisites
Before you start, make sure you have the following installed:

- Node.js (v14 or higher)
- npm or yarn
- MongoDB (Local or MongoDB Atlas account)

1. Clone the Repository
Clone the repository to your local machine:

git clone https://github.com/your-username/collaborative-book-list-app.git

2. Install Backend Dependencies
Navigate to the backend directory and install the required dependencies:
cd backend
npm install

3. Set Up Environment Variables
Create a .env file in the backend directory and set the following variables:

MONGO_URI=your-mongodb-uri
PORT=5000
Replace your-mongodb-uri with your actual MongoDB connection string. If you are using MongoDB Atlas, you can get this connection string from the MongoDB Atlas dashboard.

4. Start the Backend Server
Start the backend server using:
npm start
The backend server will be running on http://localhost:5000.

5. Install Frontend Dependencies
Navigate to the frontend directory and install the required dependencies:
cd frontend
npm install

6. Start the Frontend Server
Start the frontend development server using:
npm start

The frontend app will be running on http://localhost:3000.
# SCREENSHOTS:

![Screenshot (1401)](https://github.com/user-attachments/assets/e5d4006c-9ad9-4eb2-934d-92cbfab82fbd)
![Screenshot (1402)](https://github.com/user-attachments/assets/073af9ba-2c1e-4c2e-9f77-c8ba3a81fe87)
![Screenshot (1403)](https://github.com/user-attachments/assets/64cbd9c4-de96-48be-bd6e-96ff68495656)
![Screenshot (1405)](https://github.com/user-attachments/assets/bf7422ef-9eb8-4164-9e82-c4dd63d3dc7a)
![Screenshot (1404)](https://github.com/user-attachments/assets/a1f79b11-3138-471b-a6a7-d2964efb3e2e)
![Screenshot (1407)](https://github.com/user-attachments/assets/3e8f54d1-a9fb-40a7-9d0a-5f6e27ee580a)
![Screenshot (1406)](https://github.com/user-attachments/assets/865aa1ec-0eec-457c-ab1b-783f00b70385)
![Screenshot (1409)](https://github.com/user-attachments/assets/04c3b0be-ce4e-4b36-93db-91f1bd0fc66d)
![Screenshot (1410)](https://github.com/user-attachments/assets/2b936c92-fba7-4a1f-9bb5-1b66c41e1d9c)



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

# Styling and Responsiveness
The app uses a fluid layout with custom media queries for different screen sizes. It is designed to be fully responsive for:
Large screens (Desktops)
Medium screens (Tablets)
Small screens (Mobile devices)

# Key CSS Techniques:

Gradient Backgrounds: Subtle background gradients for a modern aesthetic.
Card Hover Effects: Slight elevation on hover to make cards feel interactive.
Responsive Design: The layout adjusts automatically to different screen sizes using CSS grid and flexbox.
Media Queries: Custom styles for tablet and mobile devices to ensure the app looks great on smaller screens.

# Additional Features (Optional)
User Authentication: Secure user login and session management (optional for added complexity).
Book Categories: Implement filtering by book categories (e.g., Fiction, Non-Fiction).
Comments: Enable users to leave comments on individual books.
Top Books: Sort books by upvotes and display the top ones at the top of the list.

# Future Enhancements
Add pagination to the book list for better performance with large datasets.
Implement real-time updates using WebSockets to notify users of new books or upvotes.
Integrate advanced search functionality to allow users to filter books by title, author, or category.3
