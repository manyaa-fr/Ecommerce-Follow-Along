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
