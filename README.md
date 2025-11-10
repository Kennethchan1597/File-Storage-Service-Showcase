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

## File Access Flow
<p align="center">
  <img src="/File.png" alt="authAxios" width="100%" />
</p>

## Docker Setup
<p align="center">
  <img src="/docker-setup.png" alt="authAxios" width="100%" />
  <img src="/docker.png" alt="authAxios" width="100%" />
</p>

## API testing example
<p align="center">
  <img src="/postman.png" alt="authAxios" width="100%" />
</p>
