# Zync-It

Zync-It is a web-based **real-time collaborative code editor** that allows multiple users to join a shared room and write code together. Code changes are synchronized in real time between connected users, making it easier for users to collaborate on coding tasks.

The editor supports syntax highlighting for **21 programming languages** and provides **63 editor themes**.

## ✨ Features

* **Real-Time Collaboration** — Multiple users can work on the same code simultaneously.
* **Room-Based Collaboration** — Users can join a shared room using a room ID.
* **Real-Time Code Synchronization** — Code changes are automatically shared with other users in the same room.
* **21 Programming Languages** — Supports syntax highlighting for multiple programming languages.
* **63 Editor Themes** — Provides multiple themes for customizing the coding environment.
* **User Notifications** — Users are notified when other participants join or leave the room.
* **Responsive Design** — The application works across different screen sizes.

## 🛠️ Tech Stack

### Frontend

* **React.js** — User interface
* **Recoil** — State management
* **CodeMirror** — Code editor
* **React Router** — Client-side routing
* **Axios** — HTTP requests
* **React Hot Toast** — User notifications

### Backend

* **Node.js** — Server-side runtime
* **Express.js** — Backend server
* **Socket.io** — Real-time communication between users

## 🔄 How It Works

1. A user enters the application and creates or joins a collaboration room.
2. A Socket.io connection is established between the client and server.
3. The user's socket is added to the selected room.
4. Users inside the same room can edit code together.
5. When a user changes the code, the change is sent to other users in the room in real time.
6. When a new user joins, the current code can be synchronized with that user.
7. When a user disconnects, the remaining participants are notified.

## 📁 Project Structure

```text
Zync-It/
│
├── backend/
│   ├── server.js
│   └── package.json
│
├── public/
│
├── src/
│   ├── components/
│   ├── pages/
│   ├── Actions.js
│   └── ...
│
├── package.json
├── package-lock.json
└── README.md
```

## 🚀 Getting Started

### Prerequisites

Make sure the following are installed:

* Node.js
* npm
* Git

### 1. Clone the Repository

```bash
git clone https://github.com/Aayushi-800/Zync-It.git
cd Zync-It
```

### 2. Install Frontend Dependencies

```bash
npm install
```

### 3. Start the Frontend

```bash
npm start
```

The frontend will run at:

```text
http://localhost:3000
```

### 4. Start the Backend

Open another terminal and run:

```bash
cd backend
npm install
npm start
```

The backend will run on:

```text
http://localhost:5001
```

## 💡 Collaboration Flow

```text
User 1 ──┐
         │
User 2 ──┼──> Socket.io Server ──> Shared Room
         │
User 3 ──┘
              ↓
        Code Synchronization
```

All connected users in the same room receive code updates in real time.

## 🔮 Future Improvements

* User authentication
* Persistent code storage
* Save and load coding projects
* File and folder support
* Code execution
* Improved room management
* Better collaboration features
