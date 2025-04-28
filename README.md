

# Jobby App

In this project, I have developed the **Jobby App**, an application that provides a user-friendly platform for job seekers. Users can log in and access a comprehensive list of job opportunities with features like job title search and filtering options based on salary range and employment type.

## Key Features

- **User Interface**:  
  Developed distinct pages for Login, Home, Jobs, and Job Item Details using React components. These components utilize React's capabilities for handling props, state management, event handling, and form inputs.

- **Authentication**:  
  Users can log in by providing their username and password. The application performs an HTTP API call for login authentication. Upon successful login, a JSON Web Token (JWT) is generated and stored in the client's storage. This token is used in API requests to authorize the user.

- **Routing**:  
  Implemented routing using React Router components like `Route`, `Switch`, and `Link` to ensure seamless navigation between Login, Home, Jobs, and Job Item Details pages.

- **Filtering and Search**:  
  Users can refine job searches by applying filters for salary range and employment type. These filters are sent as query parameters in API calls to retrieve specific job listings.

- **Security**:  
  Protected routes are implemented to ensure secure access. Unauthorized users attempting to access Home, Jobs, or Job Item Details routes are redirected to the Login page.

## Technologies Used

- React JS
- JavaScript
- CSS
- React Router
- REST API Calls
- Local Storage
- Cookies
- JWT Token
- Authorization and Authentication

## Summary

The **Jobby App** is a comprehensive job-search platform leveraging React's capabilities to create a dynamic and secure user experience. It offers features like user authentication, job filtering, and seamless navigation while providing essential job details to help users find their ideal employment opportunities.

---

## Demo Videos

### Success View  

<div style="text-align: center;">
  <video style="max-width:80%; box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12); outline:none;" controls muted>
    <source src="https://assets.ccbp.in/frontend/content/react-js/jobby-app-success-output-v0.mp4" type="video/mp4">
  </video>
</div>

### Failure View  

<div style="text-align: center;">
  <video style="max-width:80%; box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12); outline:none;" controls muted>
    <source src="https://assets.ccbp.in/frontend/content/react-js/jobby-app-failure-output-v1.mp4" type="video/mp4">
  </video>
</div>

---

## Setup Instructions

1. Clone the repository.
2. Install dependencies by running:
   ```bash
   npm install
   ```
3. Start the application using:
   ```bash
   npm start
   ```

---

## API Documentation

### Login API

- **Endpoint**: `https://apis.ccbp.in/login`  
- **Method**: POST  
- **Request Body**:
  ```json
  {
    "username": "rahul",
    "password": "rahul@2021"
  }
  ```
- **Success Response**:
  ```json
  {
    "jwt_token": "token_string"
  }
  ```
- **Failure Response**:
  ```json
  {
    "status_code": 404,
    "error_msg": "Username is not found"
  }
  ```

### Profile API

- **Endpoint**: `https://apis.ccbp.in/profile`  
- **Method**: GET  

### Jobs API

- **Endpoint**: `https://apis.ccbp.in/jobs`  
- **Method**: GET  
- Example API Call:
  ```
  https://apis.ccbp.in/jobs?employment_type=FULLTIME,PARTTIME&minimum_package=1000000&search=
  ```

---

## Completion Instructions

The application includes the following routes and functionalities:

- **Login Route**: Handles user authentication.
- **Home Route**: Provides a button to navigate to the Jobs page.
- **Jobs Route**: Displays job listings with filters for employment type and salary range.
- **Job Item Details Route**: Displays detailed job information and allows users to visit the company's website.
- **Not Found Route**: Redirects users to a "Not Found" page for invalid paths.

---

#
