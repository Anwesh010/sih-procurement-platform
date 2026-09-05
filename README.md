# Simple Login System (Node.js + MongoDB)

A clean and minimal login / register system built with:

- **Node.js** + **Express**
- **MongoDB** + **Mongoose**
- **bcryptjs** (password hashing)
- **express-session** (session management)

## Features

- User Registration
- User Login
- Password hashing
- Session-based authentication
- Protected Dashboard
- Logout

## Setup

### 1. Install dependencies

```bash
cd node-login
npm install
```

### 2. Start MongoDB

Make sure MongoDB is running on your machine:

```bash
# If using local MongoDB
mongod
```

Or use **MongoDB Atlas** (cloud) and put the connection string in `.env`.

### 3. Create `.env` file (optional)

```bash
cp .env.example .env
```

Edit `.env` if needed:

```
PORT=3000
MONGO_URI=mongodb://127.0.0.1:27017/simple-login
SESSION_SECRET=your-secret-key
```

### 4. Run the server

```bash
npm start
```

Open: **http://localhost:3000**

## Pages

- `/login` → Login page
- `/register` → Register page
- `/dashboard` → Protected page (only after login)

## Project Structure

```
node-login/
├── server.js
├── package.json
├── .env.example
├── public/
│   ├── login.html
│   ├── register.html
│   └── dashboard.html
└── README.md
```
