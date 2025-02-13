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



# Milestone 5: Frontend UI for User Registration and Form Validation 🎯

## Learning Goals 🎯
By the end of this milestone, you will:

1. **Create the Frontend UI for User Registration**: Design a user-friendly sign-up page where users can enter their details to create an account.
2. **Ensure Proper Form Validation**: Implement validation to ensure that user inputs (like email and password) are correct and meet the necessary criteria before submission.
3. **Update the README File**: Document your progress and what you have accomplished in this milestone.

---

## What’s a Sign-Up Page? 💻

The **Sign-Up page** is a crucial part of any web application where users can enter their details to create an account. It typically includes fields like:

- **Name**
- **Email**
- **Password**

This page allows users to provide their personal information, which will then be sent to the server for processing. A clean and well-designed sign-up form is essential for a good user experience.

---

## What is Form Validation? ✅

**Form Validation** ensures that the information users provide is correct and in the right format before being submitted to the server. For example:

- **Email Validation**: Ensures the email is in the correct format (e.g., user@example.com).
- **Password Validation**: Ensures the password meets specific security criteria (e.g., minimum length, mix of letters and numbers).

Form validation prevents errors, improves the overall user experience, and ensures that only clean, valid data is sent to the backend for further processing.

---

## Steps for Milestone 5 📝

In this milestone, you will focus on the **frontend** side of the application with guidance from your mentor. The steps include:

1. **Building the Sign-Up Page**:
   - Use **HTML** and **CSS** to create a clean and simple sign-up page with the following fields:
     - Name
     - Email
     - Password

2. **Adding Form Validation**:
   - Implement client-side validation to ensure that:
     - The email is in the correct format.
     - The password meets the required length and security criteria.
     - Proper error messages are shown if the user submits invalid data.

---

## How to Set Up and Run the Project 🚀

1. **Clone the Repository**:
   - Clone the repository to your local machine to start working on the frontend.

2. **Install Dependencies**:
   - If there are any frontend dependencies, install them using your preferred package manager (e.g., npm, yarn).

3. **Run the Application**:
   - Open the project folder in your code editor.
   - Open the HTML file to view the Sign-Up page in a web browser.

# Milestone 6: Encrypting Passwords and Storing User Data Securely 🔐

## Learning Goals 🎯
By the end of this milestone, you will:

1. **Understand how to encrypt passwords** before saving them in the database.
2. **Know how to securely store complete user data** in the database, ensuring that sensitive information like passwords remains protected.

---

## Why Encrypting Passwords? 🔑

Encrypting passwords is crucial for protecting user data and ensuring privacy. Here are the key reasons why it’s important:

- **Protect User Data**: Encryption helps safeguard passwords if the database is ever compromised by hackers.
- **Privacy**: Ensures that user passwords are not visible to anyone, even system administrators.
- **Compliance**: Follows important security laws and standards like **GDPR** and **PCI-DSS**, which require proper handling of sensitive information.
- **Prevents Password Theft**: Encrypted passwords cannot be easily stolen, guessed, or used in unauthorized access attempts.

---

## Steps for Milestone 6 📝

In this milestone, you will focus on **encrypting passwords** and **storing user data securely**. Here’s what we’ll cover in the live coding session:

### 1. **Encrypt the Password**
   - Use **bcrypt** to hash the user’s password during the sign-up process.
   - Store the **hashed password** in the database, ensuring that the password is never saved in plain text.

### 2. **Store Complete User Data Securely**
   - Save all the user's data, such as **name**, **email**, etc., in the database.
   - Ensure that only the **hashed password** is stored while protecting the rest of the user’s sensitive information.

---

## How to Set Up and Run the Project 🚀

1. **Clone the Repository**:
   - Clone the repository to your local machine to begin working on the backend.

2. **Install Dependencies**:
   - Install **bcrypt** and any other required dependencies using your package manager (e.g., npm or yarn).

3. **Run the Application**:
   - Start your server and test the registration process to ensure that passwords are encrypted before they’re saved.

---

## Future Improvements 🔮

- Implement password verification when users log in, using bcrypt to compare the hashed password.
- Integrate token-based authentication (e.g., JWT) to provide secure user login and access control.
- Add additional data validation and security measures for storing user data.

# Milestone 7: User Login Backend 🚀  

 *Learning Goals*  
- Validate user credentials during login.  
- Compare encrypted passwords securely.  

 *Why Encrypt Passwords?* 
- *Security*: Protects user data if the database is compromised.  
- *Privacy*: Prevents storing passwords in plain text.  
- *Compliance*: Meets security standards (GDPR, PCI-DSS).  
- *Prevention*: Makes password theft harder with hashing.  

 *How Login Authentication Works*  
1. *User Inputs Credentials* → Email/username & password.  
2. *Fetch User Data* → Check if the user exists in the database.  
3. *Validate Password* → Use bcrypt to hash & compare with stored hash.  

   *Steps to Implement*  
1. *Create Login Endpoint* → Accept email/username & password.  
2. *Retrieve User* → Fetch user data from the database.  
3. *Verify Password* → Hash input & compare with stored hash.  

 *Note:* Passwords are hashed (not decrypted). We compare hashes for authentication.