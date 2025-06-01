# WanderLust 🌍 – Your Gateway to Memorable Stays
## Overview
WanderLust is a full-stack web application enabling users to explore, list, and book unique accommodations across the globe. It provides an intuitive interface for both hosts and travelers to interact seamlessly on a dynamic platform.

The application is built using the MERN-like stack, combining the power of MongoDB, Express.js, and Node.js, along with server-side rendering using EJS templates. WanderLust incorporates features like user authentication, CRUD operations for listings, image uploads, flash messaging, session handling, and secure authorization middleware.

Whether you're looking to share your space or discover new stays, WanderLust offers a simplified and elegant solution for modern travel experiences.
## ✨ Features

- 🔐 **User Authentication (Sessions & Cookies)**  
  Users can register, log in, and log out securely using sessions and cookies.

- 🏠 **CRUD Listings**  
  Authenticated users can create, update, and delete their property listings.

- 🖼️ **Image Upload with Cloudinary**  
  Upload and manage multiple images per listing, stored securely on Cloudinary.

- 📍 **Location-Based Listings**  
  Listings include location details. Mapbox integration allows users to visualize stays on an interactive map.

- 💬 **Reviews & Ratings**  
  Users can post reviews and ratings for listings, helping others make informed decisions.

- 💻 **Responsive Design**  
  Optimized layout for seamless experience across desktops, tablets, and mobile devices.

- ⚙️ **Flash Messaging & Error Handling**  
  Get instant feedback on actions like login, signup, review submission, etc.

- 🔒 **Authorization & Ownership Control**  
  Only listing owners can modify or delete their own content using authorization middleware.

- 📦 **RESTful Routing Architecture**  
  Modular route structure following REST conventions for scalability and maintainability.
## 🛠️ Tech Stack

### 🌐 Frontend
- **EJS (Embedded JavaScript Templates)** – Server-side templating engine for rendering dynamic HTML content
- **HTML5, CSS3, Bootstrap** – For styling and responsive layout

### 🧠 Backend
- **Node.js** – JavaScript runtime environment
- **Express.js** – Web application framework for building RESTful APIs and handling server logic

### 🗃️ Database
- **MongoDB** – NoSQL database for storing listings, users, and reviews
- **Mongoose** – ODM for modeling MongoDB data in Node.js

### ☁️ Cloud & APIs
- **Cloudinary** – Image storage and management
- **Mapbox** – Interactive map API for location visualization

### 🔐 Authentication & Authorization
- **Passport.js** – Middleware for user authentication
- **express-session & connect-mongo** – Session management and persistent login with MongoDB

### ⚙️ Utilities & Middleware
- **Multer** – Handling file uploads (images)
- **method-override** – Supporting PUT and DELETE HTTP methods in HTML forms
- **connect-flash** – Flash messages for alerts and notifications
- **Custom Middleware** – `wrapAsync`, `isLoggedIn`, `isAuthor`, `validateListing`, etc.

### 📦 Dev Tools
- **Nodemon** – Development server with live-reload
- **dotenv** – Environment variable management
- **Git & GitHub** – Version control and collaboration
