# 📌 Real-Time Chat App with Node.js & Socket.IO

## 🚀 Project Overview
This is a real-time chat application built using **Node.js**, **Express**, and **Socket.IO**. It allows users to join a chat room, send and receive messages instantly, and see online users.

---

## 📂 Project Structure
```
├── public
│   └── index.html  # Frontend for the chat app
├── server.js       # Express & Socket.IO server
├── package.json    # Project dependencies
└── README.md       # Documentation
```

---

## ⚙️ Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/socket-chat-app.git
cd socket-chat-app
```

### 2️⃣ Install Dependencies
```bash
npm install
```

### 3️⃣ Start the Server
```bash
npm start
```
Server will run on: **http://localhost:3000**

---

## 🛠 Features
- ✅ Real-time messaging using **Socket.IO**  
- ✅ User join/leave notifications  
- ✅ Displays list of active users  
- ✅ Lightweight & easy to deploy  

---

## 📡 How It Works
1. A user enters a username when they visit the app.  
2. The username is sent to the server and stored in a **Set**.  
3. When a user sends a message, it's broadcasted to all connected users.  
4. When a user leaves, they are removed from the user list and notified.  

![Screenshot 2025-02-03 142618](https://github.com/user-attachments/assets/160ba692-94dd-4f2d-85de-aa2a0add5f85)

---

## 🏗️ Technologies Used
- **Node.js** - Backend server
- **Express.js** - Web framework
- **Socket.IO** - WebSockets for real-time communication
- **HTML, CSS, JavaScript** - Frontend

---

## 🔌 API & Socket Events

### **🔹 Events from Client to Server**
| Event Name  | Data Sent | Description |
|------------|----------|-------------|
| `join`  | `{ userName }` | User joins the chat |
| `chatMessage` | `{ userName, text }` | Sends a chat message |
| `disconnect` | `null` | User leaves |

### **🔹 Events from Server to Client**
| Event Name  | Data Received | Description |
|------------|--------------|-------------|
| `userJoined`  | `userName` | Notifies when a new user joins |
| `userLeft`  | `userName` | Notifies when a user leaves |
| `userList`  | `users[]` | Updates the list of online users |
| `chatMessage` | `{ userName, text }` | Receives a chat message |

---

## 📜 License
This project is licensed under the **MIT License**.

---

## 💬 Contact
For any issues or suggestions, feel free to open an issue or contact me at **rkrishan894@gmail.com**.

Happy coding! 🚀
