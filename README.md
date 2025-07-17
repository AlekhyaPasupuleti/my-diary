# MyDiary

**MyDiary** is a full-stack web application that allows users to maintain a personal diary online. It includes a modern Angular frontend and a lightweight Node.js backend, with MongoDB used as the data store.

---

## 🌟 Features

- Create, edit, and delete diary entries
- Simple and intuitive UI
- Data persisted using MongoDB
- RESTful API for backend operations

---

## 🛠️ Tech Stack

### Frontend
- Angular
- TypeScript
- HTML/CSS

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose

---

## 📁 Project Structure

```
MyDiary-main/
├── backend/                  # Backend API built with Node.js and Express
│   ├── entry-schema.js       # Mongoose schema for diary entries
│   └── rest.js               # API endpoints
├── src/                      # Angular frontend application
│   └── app/                  # Angular components and modules
├── .vscode/                  # Editor config files
├── angular.json              # Angular CLI config
├── package.json              # Project dependencies
├── tsconfig.json             # TypeScript config
└── README.md                 # Project documentation
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/MyDiary.git
cd MyDiary-main
```

---

### 2. Install Dependencies

#### For Frontend (Angular)

```bash
npm install
```

#### For Backend

```bash
cd backend
npm install
```

---

### 3. Set Up MongoDB

Make sure you have MongoDB running locally on your machine (default port 27017). You can change the MongoDB connection string in `backend/rest.js` if needed.

---

### 4. Run the Application

#### Start the Backend Server

```bash
cd backend
node rest.js
```

By default, the backend server will run on `http://localhost:3000`.

#### Start the Frontend Angular App

In a new terminal:

```bash
cd ..
ng serve
```

This will run the frontend on `http://localhost:4200`.

---

## 🔍 Example API Endpoints

- `GET /api/entries` – Get all diary entries
- `POST /api/entries` – Create a new entry
- `DELETE /api/entries/:id` – Delete an entry by ID
