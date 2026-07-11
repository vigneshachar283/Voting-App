# 🗳️ Voting App REST API

A secure backend-based Voting Application built using **Node.js, Express.js, MongoDB, JWT Authentication, and Mongoose**. The application allows users to register, authenticate, vote for candidates, and enables administrators to manage candidates while ensuring that each voter can vote only once.

---

## 🚀 Features

### User Features
- User Registration (Signup)
- Secure Login using JWT Authentication
- Password Hashing using bcrypt
- View User Profile
- Update Password
- One Person, One Vote Policy
- Aadhaar Number Validation
- Duplicate Account Prevention

### Admin Features
- Add Candidates
- Update Candidate Details
- Delete Candidates
- View All Candidates
- View Vote Count

### Voting System
- Secure JWT Protected Routes
- Only authenticated users can vote
- Admins cannot vote
- Each user can vote only once
- Automatic vote counting
- Live vote tally endpoint

---

## 🛠️ Tech Stack

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication
- bcrypt
- dotenv
- Body Parser

---

## 📁 Project Structure

```
Voting-App
│
├── models/
│   ├── user.js
│   └── candidate.js
│
├── routes/
│   ├── userRoutes.js
│   └── candidateRoutes.js
│
├── db.js
├── jwt.js
├── server.js
└── .env
```

---

## 🔐 Authentication

JWT (JSON Web Token) is used for securing private routes.

Protected operations include:
- View Profile
- Change Password
- Vote
- Candidate Management (Admin)

---

## 📌 API Endpoints

### User

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/user/signup` | Register User |
| POST | `/user/login` | Login |
| GET | `/user/profile` | View Profile |
| PUT | `/user/profile/password` | Update Password |

### Candidate

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/candidate` | Add Candidate (Admin) |
| PUT | `/candidate/:candidateID` | Update Candidate |
| DELETE | `/candidate/:candidateID` | Delete Candidate |
| GET | `/candidate` | Get All Candidates |
| GET | `/candidate/vote/:candidateID` | Cast Vote |
| GET | `/candidate/vote/count` | Vote Count |

---

## 🔒 Security Features

- Password hashing using bcrypt
- JWT Authentication
- Protected Routes
- Admin Authorization
- Aadhaar Validation
- Duplicate User Prevention
- One Vote Per User

---

## ⚙️ Installation

```bash
git clone https://github.com/vigneshachar283/Voting-App.git

cd Voting-App

npm install

npm start
```

---

## Environment Variables

Create a `.env` file.

```env
PORT=3000

MONGODB_URL_LOCAL=your_mongodb_connection_string

JWT_SECRET=your_secret_key
```

---

## 📚 Concepts Practiced

- REST API Development
- Express Routing
- MongoDB CRUD Operations
- Mongoose Models
- Authentication & Authorization
- Password Hashing
- JWT Tokens
- Middleware
- Environment Variables
- Role-Based Access Control
- Schema Validation

---

## 👨‍💻 Author

**Vignesh Achar**

GitHub: https://github.com/vigneshachar283