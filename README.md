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
├── backend/                      
│   ├── controllers/              # 🧠 Logic for routes
│   │   └── authController.js
│   │   └── chatController.js
│
│   ├── models/                   # 🗃️ Mongoose schemas
│   │   └── User.js
│   │   └── Message.js
│
│   ├── routes/                   # 📬 API routes
│   │   └── authRoutes.js
│   │   └── chatRoutes.js
│
│   ├── config/                   # 🔧 MongoDB connection setup
│   │   └── db.js
│
│   ├── middleware/               # 🛡️ JWT/auth middleware
│   │   └── authMiddleware.js
│
│   ├── socket.js                 # 📡 Socket.IO real-time messaging
│   ├── server.js                 # 🚀 Express app entry point
│   └── .env                      # 🔐 Backend secrets (Mongo URI, JWT secret)
│
├── frontend/                     
│   ├── public/                   
│   │   └── index.html
│
│   ├── src/
│   │   ├── components/           
│   │   │   └── ChatBox.jsx
│   │   │   └── Message.jsx
│   │   │   └── Navbar.jsx
│   │
│   │   ├── pages/                
│   │   │   └── Login.jsx
│   │   │   └── Signup.jsx
│   │   │   └── Chat.jsx
│   │
│   │   ├── api.js                # Axios base instance
│   │   ├── App.jsx               
│   │   └── main.jsx              
│
│   ├── .env                      # VITE_API_URL
│   └── vite.config.js            
│
├── README.md
├── .gitignore
└── package.json                 
---

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
