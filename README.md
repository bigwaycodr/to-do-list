# Advanced MERN To-Do List Application

Internship project using React.js, Node.js, Express.js, and MongoDB.

## Features

- JWT-based register, login, logout, and protected user session
- Complete task CRUD with REST APIs
- React Hooks and reusable UI components
- Task status workflow: Pending, In-Progress, Completed
- Server-side validation and structured error messages
- Pagination, filtering, searching, and sorting
- Clean backend separation of routes, controllers, models, middleware, validators, and utilities
- Responsive dashboard UI

## Setup

1. Install all dependencies from the project root:

```bash
npm run install-all
```

2. Create environment files:

```bash
copy server\.env.example server\.env
copy client\.env.example client\.env
```

3. Update `server/.env` with your `MONGODB_URI` and a strong `JWT_SECRET`.

4. Start both frontend and backend:

```bash
npm run dev
```

Open `http://localhost:5173`.

## API Endpoints

- `POST /api/auth/register`
- `POST /api/auth/login`
- `GET /api/auth/me`
- `GET /api/tasks?page=1&limit=6&status=all&priority=all&sortBy=createdAt&order=desc`
- `POST /api/tasks`
- `PATCH /api/tasks/:id`
- `DELETE /api/tasks/:id`
