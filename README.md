# 🟣 Ping – Real-Time Chat Application

Ping is a modern sleek and real-time chat app built using the MERN stack React Vite Tailwind and the real-time magic of Socket.IO
It’s clean fast and feature-packed with everything you'd expect from a proper chat platform — from typing indicators to JWT auth

---

## 📷 Visual Preview

You get three views because we're generous like that:

**🗨️ Chat Interface** — minimal white layout with purple accents built to stay out of your way while you chat
**🔐 Login Page** — smooth transitions quick auth and no-nonsense UI
**🧑 Signup Page** — lets users register with gender-based avatars because yes style matters

Images:

* `pingee.jpg` = main chat UI
* `login-image.jpg` = login page
* `signup-image.jpg` = signup form

Put them in your root folder and thank yourself later

---

## 🔥 Core Features

* Secure authentication using JWT stored in HTTP-only cookies
* Passwords hashed using bcryptjs (because we’re not animals)
* Real-time messaging with Socket.IO (rooms included)
* Online/offline tracking of users
* Typing indicators during convo (yes just like WhatsApp)
* Persistent chat messages saved in MongoDB
* Gender-based profile images auto-set at signup
* Responsive UI that’s sharp on both mobile and desktop
* Tailwind CSS with DaisyUI for that elegant finish

---

## 🧱 Full Tech Stack

**Frontend**

React 19 + Vite 7
Tailwind CSS 4 + DaisyUI 5
React Router DOM
Axios for HTTP calls
Socket.IO client
React Context API for Auth & Sockets
ESLint for code sanity

**Backend**

Node.js with Express 4
MongoDB + Mongoose ODM
JWT for authentication
Socket.IO server for messaging
bcryptjs for password hashing
cookie-parser dotenv cors all used wisely
Nodemon for dev reloads

---

## 🧠 Database Models (in human language)

**User** = name username password gender profilePic timestamps
**Message** = sender receiver content timestamps
**Conversation** = participants array messages array timestamps

---

## 🔌 Real-Time Socket Events

* `connection` = user joins the game
* `join` = user joins their own room
* `sendMessage` = message sent
* `newMessage` = message received
* `getOnlineUsers` = who’s online
* `disconnect` = someone just ghosted

---

## 🧪 REST API Endpoints

`POST /api/auth/signup` = new user
`POST /api/auth/login` = welcome back
`POST /api/auth/logout` = bye
`GET /api/users` = sidebar needs friends
`GET /api/messages/:id` = get convo messages
`POST /api/messages/send/:id` = send a message

---

## 📁 Folder Breakdown

**Backend**

controllers db middleware models routes utils server.js
Clean modular structure so even future you won’t cry

**Frontend**

components pages socket utils App.jsx main.jsx index.css
Split and organized like a fresh laundry basket

---

## ⚙️ How to Run Locally

**Step 1:** Make sure Node.js and MongoDB are installed
**Step 2:** Create a `.env` file in `backend/` and add:

```
MONGO_URI=your_mongo_connection_string
JWT_SECRET=super_secret_key
```

**Step 3:**

```bash
cd backend  
npm install  
npm run dev
```

**Step 4:**

```bash
cd frontend  
npm install  
npm run dev
```

Open `http://localhost:5173` and boom your chat app is alive 🎉

---

## 🔐 Security Highlights

* JWT stored in secure HTTP-only cookies
* bcryptjs with salt rounds for passwords
* Route protection middleware to stop intruders
* CORS setup for front-back communication
* Environment variables used like a responsible dev

---

## 🚀 Coming Soon (V2)

✅ Read Receipts
🖼 Media uploads (images emojis GIFs)
🧑‍🤝‍🧑 Group chat support
🔔 Push notifications
🔍 Search conversations
🗑 Delete and edit messages

Because one-on-one chats are just the beginning

---

## 🙋‍♂️ Made by

**Saad Tiwana**
---

Let me know if you want this in a PDF or embedded in your site bro
Or if you want a tagline like:

> **Ping** — *Where every message hits the mark*

Because let’s be honest
We write code that actually does what it says on the tin 💻📨
