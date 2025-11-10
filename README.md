# File-Storage-Service-Showcase

## Introduction 💸
A robust file storage microservice for managing files with options for public / private access, supporting local storage / AWS S3, and easily testable via Swagger UI.
This repository is a showcase of the project; the full source code is private.🙇🏻‍♂️

## Features 🔥
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

## Architecture 🎪
- Spring Boot REST API
- JWT-based authentication with `SecurityFilterChain`
- Supports **local and cloud storage providers**
- Containerized for consistent environments using Docker
  
## How It Works ❔

### Public vs Private Files
- Public files can be accessed without login  
- Private files require a **JWT token** for authentication

### Storage Options
- **Local storage:** files saved on the server filesystem  
- **AWS S3 storage:** files uploaded to a cloud bucket
  - AWS bucket-name, region, accesskey are needed for configuration   

## Architecture Diagram 🏛️
<p align="center">
  <img src="/architecture.png" alt="authAxios" width="100%" />
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
