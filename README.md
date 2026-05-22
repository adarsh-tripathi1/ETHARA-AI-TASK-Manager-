# TeamFlow — Smart Workspace & Task Collaboration Platform

A scalable full-stack workspace management platform built to simplify how teams plan projects, assign responsibilities, and monitor execution in real time.
Designed with a clean developer-first architecture, secure authentication flow, and an intuitive UI, the application focuses on productivity, collaboration, and performance.

The platform enables teams to organize projects efficiently, manage deadlines, distribute work across members, and maintain clear visibility of ongoing progress — all from a single workspace dashboard.

---

##  Live Application

* Frontend:
  [TeamFlow Frontend](https://ethara-ai-team-task-manager-production-e5ab.up.railway.app?utm_source=chatgpt.com)

* Backend API:
  [TeamFlow Backend API](https://ethara-ai-task-manager-production-2159.up.railway.app?utm_source=chatgpt.com)

---

#  Core Highlights

###  Secure Authentication System

* User Registration & Login
* JWT Access Token Authentication
* Password Encryption with bcrypt
* Persistent Login Sessions
* Route Protection Middleware
* Unauthorized Access Handling
* Secure API Communication

---

###  Role-Based Workspace Control

#### Admin Capabilities

* Create and manage projects
* Assign tasks to team members
* Edit project workflows
* Monitor task completion
* Manage overall workspace activity

#### Team Member Access

* View assigned projects
* Update task progress
* Change work status
* Track pending and completed tasks

---

#  Project Management

* Create multiple projects
* Add detailed project descriptions
* Track ownership and responsibilities
* Responsive project workspace
* Centralized project overview

---

#  Task Management System

### Task Creation & Assignment

* Assign tasks to specific members
* Add deadlines and priorities
* Manage project workflows efficiently

### Priority Levels

* Low
* Medium
* High

### Task Lifecycle

* Todo
* In Progress
* Under Review
* Completed

### Productivity Utilities

* Deadline tracking
* Overdue task alerts
* Status-based filtering
* Progress monitoring

---

#  Dashboard & Workspace Insights

* Real-time task statistics
* Pending vs completed task tracking
* Overdue task indicators
* Workspace activity overview
* Team progress visibility

---

#  User Experience

* Modern responsive interface
* Dark UI theme
* Optimized mobile responsiveness
* Toast notifications
* Interactive modal handling
* Accessible keyboard interactions
* Clean component-based architecture

---

#  Technology Stack

## Frontend

* React.js
* TypeScript
* Vite
* Tailwind CSS
* React Router DOM
* Context API

## Backend

* Node.js
* Express.js
* TypeScript

## Database

* PostgreSQL
* Neon Database

## Deployment & Hosting

* Railway

---

#  System Architecture

```text
Client (React + TypeScript)
        │
        ▼
REST API Layer (Express.js)
        │
        ▼
Authentication Middleware (JWT)
        │
        ▼
Business Logic & Services
        │
        ▼
Prisma ORM
        │
        ▼
PostgreSQL Database
```

---

#  Application Workflow

```text
User Login/Register
        │
        ▼
JWT Token Generated
        │
        ▼
Protected Dashboard Access
        │
        ▼
Project Creation / Task Assignment
        │
        ▼
Team Members Update Status
        │
        ▼
Real-Time Progress Tracking
```

---

#  Project Structure

```bash
workspace-manager/
│
├── backend/
│   ├── prisma/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── validators/
│   │   ├── helpers/
│   │   └── server.ts
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── layouts/
│   │   ├── context/
│   │   ├── routes/
│   │   ├── api/
│   │   └── App.tsx
│
└── README.md
```

---

#  Environment Configuration

## Backend `.env`

```env
PORT=5000
NODE_ENV=production

DATABASE_URL=your_database_url

JWT_SECRET=your_secret_key
JWT_EXPIRES_IN=7d

CLIENT_URL=your_frontend_url
```

---

## Frontend `.env`

```env
VITE_API_URL=your_backend_url/api
```

---

#  Local Development Setup

## Clone Repository

```bash
git clone https://github.com/adarsh-tripathi1/ETHARA-AI-TASK-Manager-.git
```

---

## Backend Setup

```bash
cd backend
npm install
```

### Prisma Setup

```bash
npx prisma generate
npx prisma db push
```

### Run Backend Server

```bash
npm run dev
```

Backend Server:

```bash
http://localhost:5000
```

---

## Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Frontend Server:

```bash
http://localhost:5173
```

---

#  Deployment

## Frontend Hosting

* Railway Deployment
* Root Directory: `frontend`

## Backend Hosting

* Railway Deployment
* Root Directory: `backend`

## Database Service

* Neon PostgreSQL

---

#  REST API Endpoints

## Authentication

```http
POST   /api/auth/signup
POST   /api/auth/login
GET    /api/auth/profile
```

---

## Projects

```http
GET     /api/projects
POST    /api/projects
PUT     /api/projects/:id
DELETE  /api/projects/:id
```

---

## Tasks

```http
GET      /api/tasks
POST     /api/tasks
PATCH    /api/tasks/:id/status
PUT      /api/tasks/:id
DELETE   /api/tasks/:id
```

---

#  Security & Validation

* Zod-based request validation
* JWT authorization middleware
* Protected API architecture
* Role-based access handling
* Secure password hashing
* Environment variable protection
* Structured backend validation flow

---

#  Planned Enhancements

* Team invitation system
* Real-time collaboration
* Activity timeline logs
* Drag-and-drop Kanban board
* Advanced filtering & search
* File attachments support
* Email notifications
* WebSocket-based live updates

---

#  Developer Focus

This project demonstrates:

* Full-stack application development
* REST API architecture
* Secure authentication systems
* Scalable backend structure
* Database schema design
* State management
* Responsive UI engineering
* Production deployment workflow

---

## 👨‍💻 Author

### Adarash Tripathi

Full Stack Developer | AIML Enthusiast | Backend & System Design Learner

* Passionate about building scalable web applications and solving real-world problems through technology.
* Interested in Full Stack Development, Artificial Intelligence, and modern cloud-based architectures.
* Focused on writing clean backend services, secure APIs, and responsive frontend experiences.

### Connect

* GitHub: `https://github.com/adarsh-tripathi1`
* LinkedIn: `https://www.linkedin.com/in/adarsh-tripathi-47a06024a/`


---

## 🌟 Acknowledgements

Special thanks to all mentors, peers, and open-source communities whose resources and guidance helped during the development and deployment of this project.

---

## 📌 Project Status

The project is actively maintained and continuously improved with new features, performance optimizations, and better collaboration capabilities.

