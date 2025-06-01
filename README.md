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
- **EJS (Embedded JavaScript Templates)** – Server-side rendering for dynamic views (`/views`)
- **HTML5, CSS3, Bootstrap** – For styling and responsive layout

### 🧠 Backend
- **Node.js** – JavaScript runtime for the server
- **Express.js** – Web application framework (`app.js`, `/routes/`)

### 🗃️ Database
- **MongoDB** – NoSQL database to store users, listings, and reviews
- **Mongoose** – ODM to model and query MongoDB (`/models/`)

### ☁️ Cloud & APIs
- **Cloudinary** – Image upload and hosting (`cloudConfig.js`)
- **Mapbox** – Location services and interactive maps (used in views/listings)

### 🔐 Authentication & Authorization
- **Passport.js** – Used for local authentication
  - `app.js` – Initialization and session setup
  - `models/user.js` – User schema using `passport-local-mongoose`
  - `routes/users.js` – Routes for login, signup using `passport.authenticate('local')`
- **express-session & connect-mongo** – Session and cookie storage with MongoDB

### ⚙️ Utilities & Middleware
- **Multer** – Handles image uploads
- **method-override** – Enables HTTP verbs like PUT & DELETE in forms
- **connect-flash** – Flash messages for alerts
- **Custom Middleware** – Error handling and async wrappers (`/utils/ExpressError.js`, `/utils/wrapAsync.js`)

### 📦 Dev Tools
- **Nodemon** – Auto-restart server during development
- **dotenv** – Manage environment variables
- **Git & GitHub** – Version control and collaboration
## ⚙️ Setup Instructions

Follow these steps to set up and run the WanderLust project locally on your machine.

### 📁 1. Clone the Repository

Clone the project using Git:

```bash
git clone https://github.com/IshaGala/WanderLust.git
cd WanderLust

📦 2. Install Dependencies
Make sure you have Node.js and npm installed. Then run: 
npm install

🔐 3. Configure Environment Variables
Create a .env file in the root directory and add the following:
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_KEY=your_cloudinary_key
CLOUDINARY_SECRET=your_cloudinary_secret
MAPBOX_TOKEN=your_mapbox_token
DB_URL=mongodb://localhost:27017/wanderlust
SECRET=your_session_secret

▶️ 4. Run the Application
Start the server using:
nodemon app.js
