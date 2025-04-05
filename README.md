# Ecommerce-Follow-Along

# Milestone 1: 
Initialized README.md

-- 

# Milestone 2:

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

--

# Milestone 3: Project Setup for Backend

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

--

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

--

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

--

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

--

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

--

 # Milestone 8: Product Card Component and Homepage Layout

### 📝 **Objective:**
In this milestone, the goal was to create a reusable **Product Card Component** that displays product details such as name, price, and image. These cards are then displayed on the homepage, providing an organized and visually appealing layout for the products.

### 🎯 **Learning Goals:**
By the end of this milestone, I have learned:
- How to create a **card component** in React (or any framework being used).
- How to display these cards dynamically by passing product details as **props**.
- How to create a **homepage layout** to display multiple product cards using **grid layout** or **flexbox**.
  
### 🛠️ **Steps Taken:**

1. **Card Component:**
   - Designed a reusable `Card` component that takes props such as `name`, `image`, and `price`.
   - The component renders the product information neatly in a card format.

2. **Homepage Layout:**
   - Created a grid or flexbox layout for the homepage to display multiple product cards.
   - Used array mapping to dynamically render the product cards, ensuring each card is populated with the correct product data.

### ✨ **Key Features:**
- **Dynamic Product Cards**: Each product is passed as a prop, ensuring the design is reusable for any product.
- **Grid/Flexbox Layout**: Used CSS grid or flexbox for a clean, organized display of product cards on the homepage.

--

# Milestone 9: Product Input Form

### Overview
In this milestone, we created a frontend form that allows users to input product details, including multiple images. This form will help collect data that will be stored in the database and displayed on the product homepage from the previous milestone.

### Learning Outcomes
- Built a product input form.
- Enabled multiple image uploads for products.
- Gained experience with frontend form validation and handling file inputs.

### Implementation Steps
1. Designed a form with fields for product details like name, price, description, and category.
2. Implemented multiple image upload functionality.
3. Ensured validation for required fields.
4. Pushed all changes to the GitHub repository.

--

# Milestone 10: Product Schema and API Endpoint

### Overview
In this milestone, we created a Mongoose schema for products and built an endpoint to store product details in MongoDB. This ensures data validation and maintains integrity in the database.

### Learning Outcomes
- Defined a Mongoose schema for products.
- Implemented validation rules for required fields.
- Built a POST endpoint to accept product details.
- Integrated MongoDB for data storage.
- Ensured only valid data is saved in the database.

### Implementation Steps
1. Created a Mongoose schema defining product fields like name, description, price, and image URL.
2. Implemented validation for required fields and data types.
3. Built a POST API endpoint to accept product details from the frontend.
4. Connected to MongoDB and stored valid product data.
5. Committed and pushed all changes to the GitHub repository.

--

# Milestone 11 - Dynamic Home Page

## Overview
In this milestone, we implemented a dynamic home page that displays all the products retrieved from MongoDB. This involved creating an endpoint to fetch stored product data and rendering it dynamically on the frontend using the product card component.

## Learning Goals 🎯
- Write an endpoint to send product data from MongoDB to the frontend.
- Fetch and display data dynamically using React components.

## Implementation Steps 📝
1. **Backend:** Created a new API endpoint (`GET /products`) to retrieve all product data from MongoDB.
2. **Frontend:** Implemented a function to fetch product data from the backend.
3. **UI Update:** Passed retrieved data dynamically to the product card component for display.

--

# Milestone 12 - My Products Page

## Overview
In this milestone, we implemented a **My Products** page that displays all the products added by the logged-in user. This involved creating an endpoint to fetch products based on the user's email and dynamically rendering them on the frontend using the product card component.

## Learning Goals 🎯
- Write an endpoint to filter and send product data based on the logged-in user's email.
- Fetch and display filtered data dynamically using React components.

## Implementation Steps 📝
1. **Backend:** Created a new API endpoint (`GET /my-products?email=user@example.com`) to retrieve products associated with the given email.
2. **Frontend:** Implemented a function to fetch products using the logged-in user's email.
3. **UI Update:** Passed the filtered product data dynamically to the product card component for display.

--

# Milestone 13 - Edit Products Functionality

## Overview
In this milestone, we implemented a feature to **edit uploaded products**. This involved creating an endpoint to update product details in MongoDB and enhancing the frontend to allow users to edit product information dynamically.

## Learning Goals 🎯
- Write an endpoint to update existing product data in MongoDB.
- Auto-fill the form with previous product details and allow users to modify them.

## Implementation Steps 📝
1. **Backend:** Created a new API endpoint (`PUT /products/:id`) to update product details in MongoDB.
2. **Frontend:**
   - Added an **Edit** button to the product card.
   - Clicking the edit button fills the form with existing product data.
   - Provided an option to update and save the changes.

   --

   # Milestone 14 - Delete Product Functionality

## Overview
In this milestone, we implemented a delete functionality that allows users to remove a product from the database using its unique ID. This involved updating both the frontend and backend to support the delete operation.

## Learning Outcomes
By completing this milestone, we learned:
- How to create an API endpoint to delete a product from MongoDB using its ID.
- How to integrate the delete feature in the frontend.
- How to handle delete requests and update the UI accordingly.

## Steps Implemented
1. **Backend:**
   - Created an Express.js endpoint to handle DELETE requests.
   - Used MongoDB's delete operation to remove the product by its ID.

2. **Frontend:**
   - Added a delete button to each product card.
   - Implemented an event listener to send a delete request to the server when the button is clicked.
   - Updated the UI dynamically after a successful deletion.

## API Endpoint
**Method:** DELETE  
**Endpoint:** `/api/products/:id`  
**Description:** Deletes a product from the database using the provided ID.

--

# Milestone 15: Navbar Component  

### What was achieved in this milestone  

- Created a reusable `Nav` component with navigation links to all pages:  
  - Home  
  - My Products  
  - Add Product  
  - Cart  
- Ensured the Navbar is responsive to all screen sizes.  
- Integrated the Navbar component into all pages for seamless navigation.  

--

# Milestone 16: Product Info Page  

### What was achieved in this milestone  

- Created a new **Product Info** page to display detailed product data.  
- Added an option to choose the quantity of the product.  
- Implemented an **"Add to Cart"** button for easy product addition.  

--

# Milestone 17 - Cart Functionality

## Overview
In this milestone, we implemented the backend functionality to add products to a cart and store them in a database.

## Learning Goals 🎯
- Edited the user schema to store cart products.
- Created a cart schema to store product details.
- Implemented an endpoint to receive and store product details in the cart.

## Steps Completed 📝
1. **Updated User Schema**: Modified the schema to include cart-related fields.
2. **Created Cart Schema**: Defined a schema to store product details in the cart.
3. **Implemented API Endpoint**: Wrote an endpoint to add products to the cart and store them in the database.
4. **Tested Functionality**: Verified the API using Postman to ensure products are correctly stored in the cart.

--

# Milestone 18 - Fetch Cart Products

## Overview
In this milestone, we implemented the backend functionality to fetch all products inside a user's cart and display them on the cart page.

## Learning Goals 🎯
- Created an endpoint to receive requests from the cart page.
- Implemented a backend endpoint to fetch all products inside the cart using the user's email.

## Steps Completed 📝
1. **Created Backend Endpoint**: Implemented an API endpoint to retrieve cart products.
2. **Integrated User Authentication**: Ensured that only authenticated users can access their cart details.
3. **Fetched Cart Data**: Retrieved products stored in the cart based on the user's email.
4. **Tested Functionality**: Verified the API response using Postman to ensure correct retrieval of cart items.

--

# Milestone 19: Cart Page and Quantity Update API

## Overview
In this milestone, I implemented the cart functionality, allowing users to view products in their cart and adjust quantities using + and - buttons. I also created backend endpoints to handle quantity updates.

## Features Implemented
- **Cart Page UI**: Displays products added to the cart.
- **Quantity Adjustment**: Each product has `+` and `-` buttons to increase or decrease quantity.
- **Backend Endpoints**:
  - `POST /cart/increase/:productId`: Increases the quantity of a product.
  - `POST /cart/decrease/:productId`: Decreases the quantity of a product.

  --

  # Milestone 20: Profile Page and User Data API

## Overview  
In this milestone, I implemented a profile page where users can view their details, including their profile photo, name, email, and addresses. Additionally, I created a backend endpoint to fetch user data.  

## Features Implemented  

### Backend  
- **User Data API**:  
  - Endpoint: `GET /user/profile`  
  - Sends user details, including name, email, profile photo URL, and addresses.  

### Frontend  
- **Profile Page UI**:  
  - Displays the user's profile photo, name, and email in one section.  
  - Shows the user’s saved addresses in another section.  
  - Includes an "Add Address" button.  
  - Displays "No address found" if the user has no saved addresses.  

  --

  # Milestone 21 - Address Input Form

## Overview
In this milestone, I created a frontend page for address input. The form allows users to enter their address details, including country, city, address lines, zip code, and address type.

## Features
✅ Address input form with fields:
   - Country  
   - City  
   - Address Line 1  
   - Address Line 2  
   - Zip Code  
   - Address Type (e.g., Home, Work)  
✅ State management to store input values  
✅ Navigation from the profile page to the address form  

--

# Milestone 22 - Save Address in User Profile

## Overview
In this milestone, I created a backend endpoint to save the address inside the user profile in the database. The endpoint receives the address from the frontend and updates the user collection.

## Features
✅ Backend endpoint to store user address  
✅ Adds the address to the address array inside the user collection  
✅ Connects with the frontend form to receive user input  

--

# 🛍️ Milestone 23  

## 📌 Milestone Overview  
In this milestone, we have implemented the **Place Order** functionality in our React app. This includes:  
- Adding a **"Place Order"** button in the cart page.  
- Creating a **Select Address** page where users can view and choose a delivery address.  
- Setting up a **backend endpoint** to fetch user addresses.  
- Writing the **Mongoose schema** for storing order details in the database.  

---

## 🏗️ Features Implemented  
✅ **Cart Page Update:** Added a "Place Order" button that redirects to the Select Address page.  
✅ **Select Address Page:** Displays all saved addresses with an option to select one.  
✅ **Backend API:** Created an endpoint to fetch user addresses.  
✅ **Order Schema:** Defined a Mongoose schema to store order details.  

--

# Milestone 24: Order Confirmation Page  

## Overview  
In this milestone, I implemented an Order Confirmation page that displays:  
- The list of products being ordered  
- The selected delivery address  
- The total cart value  
- A "Place Order" button to proceed with the order  

## Key Features  
- Dynamically renders ordered products and user-selected address  
- Calculates and displays total price  
- Includes a functional "Place Order" button  

--

# Milestone 25: Implementing 'Place Order' Endpoint

## Learning Goals 🎯
By completing this milestone, we:
- Created a backend endpoint for placing an order.
- Retrieved the user ID using their email.
- Stored order details in MongoDB using the `Order` schema.

---

## Steps Implemented 📝
1. **Created an Express route** to handle order placement.
2. **Extracted user email** from the request and fetched the `_id` from the database.
3. **Iterated over products** to create separate orders for each product with the same address.
4. **Stored order details** in the MongoDB `orders` collection.

--

# Milestone 26: Fetching User Orders Endpoint

## Learning Goals 🎯
By completing this milestone, we:
- Created a backend endpoint to retrieve all orders of a specific user.
- Retrieved the user ID using their email.
- Queried the MongoDB `orders` collection to fetch the user's orders.
- Sent all retrieved orders in the response.

---

## Steps Implemented 📝
1. **Created an Express route** to fetch user orders.
2. **Extracted user email** from the request and fetched the `_id` from the database.
3. **Queried MongoDB** using the `_id` to get all orders of that user.
4. **Sent all retrieved orders** in the response.

--

# Milestone 27 - My Orders Page 🛍️

In this milestone, I created a new frontend page named **`my-orders`**, which allows users to view all their orders.

#### ✅ What was achieved:
- Developed the `my-orders` page to display all orders related to a logged-in user.
- Integrated a **GET request** to the `my-orders` endpoint (created in a previous milestone).
- Fetched orders using the user's email as a query parameter.
- Rendered all user orders dynamically on the page.
- Updated the **navigation bar** to include a link to the `my-orders` page for easy access.
- Ensured responsive UI and smooth UX for checking user order history.
