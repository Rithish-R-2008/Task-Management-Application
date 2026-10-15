# Task Management Application

A full-stack Task Management Application built using **React, Node.js, Express.js, MongoDB, and Socket.IO**. It helps users organize, manage, and track their daily tasks through a modern, responsive dark-themed dashboard.

## 🚀 Features

- **User Authentication:** Secure registration and login using JWT.
- **Task Management:** Create, view, update, and delete tasks.
- **Priority Management:** Organize tasks by priority levels.
- **Status Tracking:** Track tasks based on their progress.
- **Due Dates:** Set deadlines for tasks.
- **Search and Filter:** Find tasks easily.
- **Real-Time Updates:** Receive task updates using Socket.IO.
- **Responsive Dashboard:** Modern dark-themed interface for desktop and mobile devices.
- **Database Integration:** Store user and task information in MongoDB.

## 🛠️ Technologies Used

**Frontend**
- React.js
- Vite
- CSS
- Socket.IO Client

**Backend**
- Node.js
- Express.js
- Socket.IO
- JSON Web Token (JWT)
- bcryptjs

**Database**
- MongoDB
- Mongoose

## 📁 Project Structure

```text
task-management-app/
├── backend/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── server.js
│   ├── package.json
│   └── .env
├── frontend/
│   ├── src/
│   ├── index.html
│   ├── package.json
│   └── vite.config.js
├── README.md
└── START-HERE.txt
```

## ⚙️ Installation and Setup

### Prerequisites

Install the following before running the application:

- [Node.js](https://nodejs.org/)
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) or a local MongoDB installation
- [Visual Studio Code](https://code.visualstudio.com/)

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd task-management-app
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your repository's actual URL.

### 2. Configure the Backend

```bash
cd backend
npm install
```

Create a `.env` file inside the `backend` folder and add:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_long_random_secret
CLIENT_URL=http://localhost:5173
```

Replace the MongoDB connection string with your own database URI. Keep your `.env` file private and never upload real credentials to GitHub.

Start the backend:

```bash
npm run dev
```

### 3. Configure the Frontend

Open a **second terminal** in the project root and run:

```bash
cd frontend
npm install
npm run dev
```

### 4. Open the Application

Open the local URL displayed in the frontend terminal, usually:

```text
http://localhost:5173
```

Register an account and start managing your tasks.

## 🔄 How It Works

1. Users register or log in securely.
2. The frontend sends authenticated requests to the Express.js backend.
3. The backend validates requests and interacts with MongoDB.
4. Users can create, update, delete, search, and filter their tasks.
5. Socket.IO delivers real-time task updates to connected users.

## 🔒 Security

- Passwords are hashed using bcryptjs.
- JWT is used for authentication.
- Protected routes require a valid token.
- Tasks are associated with their respective users.
- Environment variables keep configuration and secrets outside the source code.

## 🎯 Project Objective

The main objective of this project is to simplify task organization and improve productivity through a secure, responsive, and real-time task management system.

## 🔮 Future Enhancements

- Task reminders and notifications
- Team collaboration and task assignment
- Calendar integration
- Drag-and-drop task organization
- Deployment to a cloud platform

## 👨‍💻 Author

**Rithish R**

Computer Science and Engineering — Artificial Intelligence and Machine Learning

## 📄 License

This project is intended for learning and educational purposes. Add a license file if you plan to distribute it under a specific open-source license.
