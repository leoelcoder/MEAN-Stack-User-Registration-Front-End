# MEAN Stack User Registration Application

A full-stack web application built with the MEAN stack (MongoDB, Express.js, Angular 6, Node.js) for user registration with password encryption and validation.

## Architecture

This application consists of:

- **Frontend**: Angular 6 application with user registration form
- **Backend**: Node.js/Express.js API server
- **Database**: MongoDB for data persistence

## Features

- User registration with form validation
- Password encryption using bcrypt
- Client-side and server-side validation
- RESTful API design
- Responsive Angular frontend

## Project Structure

```
├── Angular6/          # Angular 6 frontend application
├── server/           # Node.js backend API
└── README.md
```

## Getting Started

### Prerequisites

- Node.js (v8 or higher)
- MongoDB
- Angular CLI (for frontend development)

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd MEAN-Stack-User-Registration-Front-End
```

2. Install backend dependencies:
```bash
cd server
npm install
```

3. Install frontend dependencies:
```bash
cd ../Angular6
npm install
```

### Running the Application

1. Start MongoDB service

2. Start the backend server:
```bash
cd server
npm start
```

3. Start the frontend development server:
```bash
cd Angular6
ng serve
```

The application will be available at `http://localhost:4200`

## API Endpoints

- `POST /api/register` - Register a new user

## Technologies Used

- **Frontend**: Angular 6, TypeScript, HTML5, CSS3
- **Backend**: Node.js, Express.js
- **Database**: MongoDB, Mongoose
- **Security**: bcryptjs for password hashing
- **Validation**: Angular forms validation, Mongoose schema validation