# Ecommerce-Follow-Along

## Milestone 1: 
Initialized README.md

## Milestone 2:

This milestone focuses on setting up the project structure, building the frontend with React, configuring styling with Tailwind CSS, and developing the login page.

## Project Folder Structure

The project is organized into two main directories:

*   `frontend`: Contains all the code for the user interface (what the user sees).
*   `backend`: Contains the server-side code (what handles data and logic).

e-commerce-app/
├── frontend/
│   ├── ... (React app files)
└── backend/
├── ... (Node.js server files)


### React Frontend Setup
A new React application was created in the `frontend` directory.  React is used to build a dynamic and interactive user interface.

### Node.js Backend Setup
A basic Node.js server was set up in the `backend` directory.  This server will be used later to connect to a database and handle API requests.

### Tailwind CSS Configuration
Tailwind CSS was integrated into the project for styling.  Tailwind CSS makes it easy to create modern and responsive designs using pre-defined utility classes.

### Login Page Development
The first user interface component, the login page, was developed. This page allows users to enter their credentials to access the application.  The login page was styled using Tailwind CSS.

## Milestone 3: Project Setup for Backend

In this milestone, we focused on setting up the backend of the e-commerce application. Here's what was achieved:

### Backend Folder Structure
- Created a structured hierarchy for organizing backend code:
  - `routes/`: Contains all API routes.
  - `controllers/`: Handles the logic for processing requests.
  - `models/`: Defines the database schemas and models.
  - `middlewares/`: (Future use) For adding middleware functions.
  - `utils/`: (Future use) For utility functions and helpers.

### Server Setup
- Initialized a Node.js server using Express.
- Configured the server to listen on port `3000`.
- Set up basic API routes for testing the server.

### Database Connection
- Integrated MongoDB using Mongoose for efficient data storage.
- Established a connection between the server and MongoDB.
- Created a basic schema for products to prepare for future data storage.

### Error Handling
- Implemented basic error handling middleware to catch and log errors.
- Added error responses for invalid routes and server errors.

### Updated README
- Added this section to document the progress made in Milestone 3.

# Milestone 4: User Model, Controller, and File Uploads 🚀

## Learning Goals 🎯
By the end of this milestone, you will:
1. **Create a User Model**: Design a blueprint for storing user data in the database.
2. **Create a User Controller**: Manage user data operations (e.g., adding a new user, fetching user information).
3. **Enable and Configure Multer**: Implement file upload functionality for user-uploaded files (e.g., profile pictures).
4. **Update the README File**: Document your progress and changes.

---

## Steps Completed ✅

### 1. User Model
- Created a **User Schema** using Mongoose to define the structure of user data.
- Included fields such as `name`, `email`, `password`, and `profilePicture`.
- Added validation rules (e.g., required fields, unique email).

# Milestone 4: User Model, Controller, and File Uploads 🚀

## Learning Goals 🎯
By the end of this milestone, you will:
1. **Create a User Model**: Design a blueprint for storing user data in the database.
2. **Create a User Controller**: Manage user data operations (e.g., adding a new user, fetching user information).
3. **Enable and Configure Multer**: Implement file upload functionality for user-uploaded files (e.g., profile pictures).
4. **Update the README File**: Document your progress and changes.

---

## Steps Completed ✅

### 1. User Model
- Designed a **User Schema** using Mongoose to structure user data in the database.
- Included key fields such as `name`, `email`, `password`, and `profilePicture`.
- Applied validation rules to ensure required fields, unique email addresses, and proper data formats.
- Implemented password hashing to enhance security.

### 2. User Controller
- Developed functions to manage user-related operations:
  - **User Registration**: Allows creating new users with proper validation.
  - **Fetching User Information**: Retrieve details of a user by their ID.
  - **Updating User Data**: Provides functionality for modifying user information.
  - **Deleting a User**: Enable user removal from the database.

### 3. Multer Configuration for File Uploads
- Integrated **Multer** for handling file uploads, specifically for user profile pictures.
- Configured Multer to save files with a specific storage destination and naming format.
- Implemented file validation to ensure only image files are accepted, along with size limitations.
- Linked uploaded files (profile pictures) to users, storing the file paths in the user model.

### 4. Testing and Validation
- Conducted manual tests using Postman to ensure that all user-related endpoints work as expected.
- Ensured that file uploads, validation, and error handling are functioning correctly.
- Validated that profile pictures are properly uploaded and saved in the right format and path.

### 5. Documentation
- Updated the README to accurately describe the application’s functionality and how to use the API.
- Detailed the routes for creating, updating, and deleting users, as well as for uploading files.
- Explained the Multer configuration and how file uploads are handled.



