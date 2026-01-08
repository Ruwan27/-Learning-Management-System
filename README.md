📚 Learning Management System (LMS)
<p align="center"> <a href="https://nestjs.com/" target="_blank"> <img src="https://nestjs.com/img/logo-small.svg" width="120" alt="NestJS Logo" /> </a> </p> <p align="center"> A full-stack Learning Management System built with <b>NestJS</b>, <b>React</b>, <b>TypeScript</b>, <b>Vite</b>, and <b>Docker</b>. </p>
🚀 Tech Stack
Backend

Node.js

NestJS

TypeScript

REST API

JWT Authentication

PostgreSQL (via Prisma / TypeORM)

Docker

Frontend

React

TypeScript

Vite

React Router

Axios

Docker (Nginx for production)

🧩 Features (Planned & Implemented)
👤 User Management

User registration & login

Role-based access (Admin / Instructor / Student)

JWT authentication

📘 Courses

Create & manage courses

Course enrollment

Lessons & modules

🎥 Content

Video lessons

File uploads (PDF, slides)

Lesson progress tracking

📝 Assessments

Quizzes

Assignments

Grading system

🗂️ Project Structure
lms-project/
│
├── backend/                 # NestJS backend
│   ├── src/
│   │   ├── auth/
│   │   ├── users/
│   │   ├── courses/
│   │   ├── lessons/
│   │   └── main.ts
│   ├── Dockerfile
│   └── package.json
│
├── frontend/                # React + Vite frontend
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   ├── services/
│   │   └── main.tsx
│   ├── Dockerfile
│   └── package.json
│
├── docker-compose.yml
└── README.md

⚙️ Environment Variables
Backend (backend/.env)
PORT=3000
DATABASE_URL=postgresql://postgres:postgres@db:5432/lms
JWT_SECRET=supersecretkey

Frontend (frontend/.env)
VITE_API_URL=http://localhost:3000

🐳 Docker Setup
Run the Entire Stack
docker-compose up --build
