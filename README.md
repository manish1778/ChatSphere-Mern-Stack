# 💬 ChatSphere – Real-Time Chat Application (MERN Stack)

ChatSphere is a **real-time one-to-one chat application** built using the **MERN stack**. It supports secure authentication, live messaging with Socket.io, online user tracking, message seen status, profile management, and image sharing.

---

## 🚀 Features

* 🔐 User authentication (Signup & Login using JWT)
* 💬 Real-time messaging with Socket.io
* 🟢 Online users indicator
* 👁️ Seen / Unseen message tracking
* 📷 Image sharing in chat (Cloudinary)
* 🧑 Profile update (name, bio, profile picture)
* 📱 Responsive and clean UI
* 🔒 Protected routes for authenticated users

---

## 🛠️ Tech Stack

### Frontend

* React (Vite)
* Context API (Global State Management)
* Axios
* Socket.io Client
* React Hot Toast
* CSS

### Backend

* Node.js
* Express.js
* MongoDB & Mongoose
* Socket.io
* JWT Authentication
* Bcrypt.js
* Cloudinary

---

## 📂 Project Structure

```
ChatSphere-MERN/
│
├── client/
│   ├── context/
│   │   ├── AuthContext.jsx
│   │   └── ChatContext.jsx
│   │
│   ├── public/
│   │
│   ├── src/
│   │   ├── assets/
│   │   │
│   │   ├── components/
│   │   │   ├── ChatContainer.jsx
│   │   │   ├── RightSidebar.jsx
│   │   │   └── Sidebar.jsx
│   │   │
│   │   ├── lib/
│   │   │   └── utils.js
│   │   │
│   │   ├── pages/
│   │   │   ├── HomePage.jsx
│   │   │   ├── LoginPage.jsx
│   │   │   └── ProfilePage.jsx
│   │   │
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   │
│   ├── .env
│   ├── index.html
│   ├── eslint.config.js
│   ├── package.json
│   └── .gitignore
│
├── server/
│   ├── controllers/
│   │   ├── userController.js
│   │   └── messageController.js
│   │
│   ├── models/
│   │   ├── User.js
│   │   └── Message.js
│   │
│   ├── routes/
│   │   ├── userRoutes.js
│   │   └── messageRoutes.js
│   │
│   ├── middleware/
│   │   └── auth.js
│   │
│   ├── lib/
│   │   ├── db.js
│   │   ├── cloudinary.js
│   │   └── utils.js
│   │
│   ├── server.js
│   └── package.json
│
└── README.md
```

---

## ⚙️ How It Works (High Level)

1. Users sign up or log in using JWT authentication.
2. After login, a Socket.io connection is established.
3. Online users are tracked in real time.
4. Messages are sent and received instantly using sockets.
5. Messages are stored in MongoDB.
6. Unseen messages are counted and marked as seen when opened.
7. Images are uploaded and served via Cloudinary.

---

## 🔐 Authentication Flow

* JWT token generated on login/signup
* Token stored in localStorage
* Token sent in request headers
* Protected routes validated using middleware

---

## 🧪 Environment Variables

### Client (`client/.env`)

```
VITE_BACKEND_URL=http://localhost:5000
```

### Server (`server/.env`)

```
PORT=5000
MONGODB_URI=your_mongodb_url
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

---

## ▶️ Run Locally

### Backend

```bash
cd server
npm install
npm start
or
npm server
```

### Frontend

```bash
cd client
npm install
npm run dev
```

---

## 📌 Future Enhancements

* Group chats
* Typing indicators
* Message reactions
* Read receipts for group chats
* Push notifications

---

## 👨‍💻 Author

**Manish Gautam**
Full Stack Developer (MERN)
📍 India

