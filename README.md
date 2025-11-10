# File-Storage-Service-Showcase

## Introduction 💸
A robust file storage service for managing files with options for public / private access, supporting local storage / AWS S3, and easily testable via Swagger UI.
This repository is a showcase of the project; the full source code is private.🙇🏻‍♂️

## Features
- **File Operations**
  - Upload files
  - Download files
  - Delete files

- **Access Control**
  - Public files: accessible without authentication  
  - Private files: JWT-secured endpoints

- **Storage Options**
  - Local filesystem storage  
  - AWS S3 cloud storage  

- **API Testing**
  - Swagger UI support for interactive API testing
- **Docker Support**
  - Preconfigured Docker environment for easy setup
- **Extensibility**
  - Switch between storage types through configuration
  - Add custom features without breaking core functionality

## Repository Structure 🔥
- **Finance-Tracker-App**
    - A **React Native** mobile application
    - Communicates with the backend Java Spring APIs via **Axios HTTP requests**
- **Finance-Service**
  - Java Spring Boot RESTful API handling all transaction logic:
    - Create, Read, Update, Delete (CRUD) transactions
    - Persist data to a database
    - JWT authentication for secure API access
- **Login-Service**
  - Java Spring Boot RESTful API for user authentication
    - User registration and login
    - Password forgot and reset
    - JWT-based authentication
    - Persist user data to a database
  
## Setup Instructions ⚙️
- Backend Setup
  - Login-Service and Finance-Service:
    - Run both Spring Boot applications on your local machine or server
    - Ensure each service is connected to a database (H2, MySQL, or PostgreSQL)
- Frontend Setup
  - Navigate to Finance-Tracker-App and install dependencies:
    - npm install
  - Update API endpoints in the following files before running the app:
    - Finance-Tracker-App/api/api/authApi.js
    - Finance-Tracker-App/api/api/transactionApi.js
    - Replace **localhost** with the **IP Adress** that host the backend services
  - Start the React Native app(Expo):
    - npm start
<p align="center">
  <img src="/README_images/transactionAxios.png" alt="transactionAxios" width="50%" />
</p>
<p align="center">
  <img src="/README_images/authAxios.png" alt="authAxios" width="50%" />
</p>

## Architecture Diagram 🏛️
<p align="center">
  <img src="/README_images/Finance-Tracker-App.png" alt="authAxios" width="100%" />
</p>

## Feature Demonstration
**Login and Create**
<br>
<div>
  <p align="center">
    <img src="/README_images/Login_gif.gif" alt="Login Demo" width="40%" />
    <img src="/README_images/Create_gif.gif" alt="Create Transaction Demo" width="40%" />
  </p>
</div>

**Update and Delete**
<br>
<div>
  <p align="center">
    <img src="/README_images/Update_gif.gif" alt="Login Demo" width="40%" />
    <img src="/README_images/Delete_gif.gif" alt="Create Transaction Demo" width="40%" />
  </p>
</div>
