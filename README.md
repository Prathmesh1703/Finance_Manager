# Finance Manager – MERN Stack Application

A full-stack Finance Management web application built using the MERN stack (MongoDB, Express.js, React.js, Node.js). The application enables users to manage income, expenses, budgets, and financial insights through a secure and responsive interface.

---

## Table of Contents

- Overview
- Features
- Tech Stack
- System Architecture
- Project Structure
- Installation
- Environment Variables
- API Endpoints
- Security
- Deployment
- Future Enhancements
- License

---

## Overview

Finance Manager is designed to help individuals and small teams efficiently track financial activities. It provides transaction management, categorized expense tracking, budget monitoring, and summary dashboards to give users better control over their finances.

---

## Features

### Authentication & Authorization
- User Registration
- User Login
- JWT-based Authentication
- Protected Routes

### Transaction Management
- Add Income and Expense Entries
- Edit Transactions
- Delete Transactions
- Filter by Date
- Filter by Category

### Financial Dashboard
- Total Income Overview
- Total Expense Overview
- Current Balance Calculation
- Category-wise Breakdown
- Date-based Financial Summary

### Budget Management
- Set Budget Limits
- Track Budget Utilization
- Monitor Spending Trends

### UI & Experience
- Responsive Design
- Clean and Structured Layout
- RESTful API Integration

---

## Tech Stack

### Frontend
- React.js
- React Router
- Axios
- Context API / Redux (if implemented)
- Tailwind CSS / Bootstrap / Custom CSS

### Backend
- Node.js
- Express.js
- JWT (JSON Web Token)
- Bcrypt (Password Hashing)

### Database
- MongoDB
- Mongoose ODM

---

## System Architecture

Client (React)  
⬇  
REST API (Express + Node.js)  
⬇  
MongoDB Database  

The frontend communicates with backend APIs via HTTP requests. The backend handles authentication, business logic, and database operations.

---

## Project Structure


finance-manager/
│
├── client/ # Frontend (React)
│ ├── public/
│ ├── src/
│ │ ├── components/
│ │ ├── pages/
│ │ ├── context/
│ │ └── services/
│ └── package.json
│
├── server/ # Backend (Node + Express)
│ ├── controllers/
│ ├── models/
│ ├── routes/
│ ├── middleware/
│ ├── config/
│ └── server.js
│
└── README.md


---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/finance-manager.git
cd finance-manager
2. Backend Setup
cd server
npm install

Create a .env file inside the server directory:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

Start the backend server:

npm start

The backend will run on:

http://localhost:5000
3. Frontend Setup
cd client
npm install
npm start

The frontend will run on:

http://localhost:3000
Environment Variables
Variable	Description
PORT	Backend server port
MONGO_URI	MongoDB connection string
JWT_SECRET	Secret key for token generation
Sample API Endpoints
Authentication
POST   /api/auth/register
POST   /api/auth/login
Transactions
GET    /api/transactions
POST   /api/transactions
PUT    /api/transactions/:id
DELETE /api/transactions/:id
Security

Passwords hashed using bcrypt

JWT-based route protection

Middleware for authentication

Environment variables for sensitive configuration

Input validation and error handling

Deployment
Backend

Render

Railway

AWS EC2

Frontend

Vercel

Netlify

Future Enhancements

Advanced analytics and charts

Export reports (PDF/CSV)

Email notifications

Multi-user support

Role-based access control

Bank API integrations

Mobile-friendly PWA version

License

This project is licensed under the MIT License.
