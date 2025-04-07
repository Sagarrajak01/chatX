# 💬 chatX

A simple and powerful fullstack real-time chat application built with Node.js, Socket.IO, React, and Express.  
Supports login, signup, and instant messaging across multiple users.

---

## 🚀 Features

- 🔐 User authentication (login/signup)
- 💬 Real-time messaging with WebSockets (Socket.IO)
- 🟢 Online user tracking
- 📦 Fullstack: React frontend + Node.js/Express backend
- 🔒 Passwords hashed for security (bcrypt)

---

## 📁 Folder Structure
chatX/
│
├── backend/                        # ⚙️ Backend code (Node.js + Express + MongoDB)
│   ├── controllers/               # 🧠 Route logic
│   │   ├── authController.js
│   │   └── messageController.js
│
│   ├── models/                    # 🗃️ Mongoose schemas
│   │   ├── User.js
│   │   └── Message.js
│
│   ├── routes/                    # 🚦 API routes
│   │   ├── authRoutes.js
│   │   └── messageRoutes.js
│
│   ├── middleware/               # 🛡️ Auth or error middleware
│   │   └── authMiddleware.js
│
│   ├── config/                   # 🔧 DB & other config
│   │   └── db.js                 # MongoDB connection
│
│   ├── socket/                   # 📡 Socket.IO events
│   │   └── index.js
│
│   ├── server.js                 # 🚀 Main entry point
│   └── .env                      # 🔐 Env variables (e.g., MONGO_URI, JWT_SECRET)
│
├── frontend/                      # 💻 React frontend
│   ├── public/
│   │   └── index.html
│
│   ├── src/
│   │   ├── components/           # 🧩 Reusable UI components
│   │   │   ├── ChatBox.jsx
│   │   │   ├── Message.jsx
│   │   │   └── Navbar.jsx
│   │
│   │   ├── pages/                # 📄 Screens/pages
│   │   │   ├── Login.jsx
│   │   │   ├── Signup.jsx
│   │   │   └── Chat.jsx
│   │
│   │   ├── utils/                # 🛠️ Axios instance, helpers
│   │   │   └── api.js
│   │
│   │   ├── App.jsx
│   │   └── main.jsx
│
│   ├── .env                      # e.g., VITE_API_URL
│   └── vite.config.js
│
├── README.md
├── .gitignore
└── package.json

## ⚙️ How to Run Locally

### 🛠 Backend

```bash
cd backend
npm install
node server.js

🌐 Frontend
cd frontend
npm install
npm run dev

📦 Tech Stack
Frontend: React, Axios, Tailwind CSS (optional)
Backend: Node.js, Express, MongoDB (if using database), Socket.IO
Authentication: JWT / bcrypt
Real-time: WebSockets (via Socket.IO)
