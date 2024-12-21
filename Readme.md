# Backend Project - User Authentication and Management

This backend project offers a comprehensive API that handles user authentication and management, including essential features such as user registration, login, logout, and JWT-based authentication for secure access. It manages both access and refresh tokens to ensure a seamless user experience while keeping sessions secure. In addition to user account management, the API allows users to update their personal information and view their account details. Furthermore, the project integrates Cloudinary for handling image uploads, making it easy to store and retrieve user profile pictures or any other media associated with user accounts. This integration with Cloudinary enhances the functionality by enabling efficient and scalable media management alongside the core authentication features.

---

## **Table of Contents**
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Folder Structure](#folder-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Environment Variables](#environment-variables)

---

## **Features**
- **User Registration**: Users can register with an email and password.
- **User Login & Logout**: Secure login and logout functionality using JWT tokens.
- **Token Handling**: Access and refresh token management for user authentication.
- **Update User Info**: Users can update their personal information.
- **View User Details**: Display user details like name, email, and other personal information.
- **Image storage** : Integration with Cloudinary for image storage.

---

## **Tech Stack**
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Token)
- **Password Encryption**: bcrypt
- **Token Handling**: Refresh and Access tokens
- **File handling**: Cloudinary

---

## **Folder Structure**
Backend-project/<br> ├── controllers/ # Contains the logic for user authentication and management<br> ├── models/ # MongoDB models for User<br> ├── routes/ # Defines the API routes<br> ├── utils/ # Utility functions (e.g., token generation)<br> ├── .env # Environment variables<br> ├── index.js # Main entry point for the application<br> └── README.md # Project documentation<br>


---

## **Installation**

### Prerequisites
- Node.js (v16 or later)
- npm or yarn
- MongoDB (local or hosted on MongoDB Atlas)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/harshkg23/Backend-project.git
   cd Backend-project
   ```
2. Set up environment variables (see below).

3. Start the development server:
    ```bash
    npm install
    npm run dev
    ```

---

   ## **Usage**

- The backend will be accessible at [http://localhost:8000](http://localhost:8000).

- Use the following API routes:
  - **POST /api/v1/users/register**: Register a new user.
  - **POST /api/v1/users/login**: Login with email and password.
  - **POST /api/v1/users/loginout**: Logout the user and invalidate the tokens.
  - **GET /api/v1/users/current-user**: Get the current user’s details.
  - **PUT /api/v1/users/change-password**: Update user information (e.g., name, email).

---

## **Environment Variables**
Create a `.env` file in the backend folder and add the following variables:
```env
PORT=8000
CORS_ORIGIN=*
MONGODB_URI=mongodb+srv://<your-mongo-username>:<your-mongo-password>@<your-cluster-name>.mongodb.net/
ACCESS_TOKEN_SECRET=<your-access-token-secret>
ACCESS_TOKEN_EXPIRY=1d
REFRESH_TOKEN_SECRET=<your-refresh-token-secret>
REFRESH_TOKEN_EXPIRY=10d
CLOUDINARY_CLOUD_NAME=<your-cloudinary-cloud-name>
CLOUDINARY_API_KEY=<your-cloudinary-api-key>
CLOUDINARY_API_SECRET=<your-cloudinary-api-secret>
```

---

## **Contact**
- **Author**: Harsh Kumar Gupta  
- **Email**: harshkumargupta2023@gmail.com  
- **GitHub**: [https://github.com/harshkg23](https://github.com/harshkg23)





