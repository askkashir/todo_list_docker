# Simple Todo List Application with Docker

This is a simple todo list application demonstrating Docker Compose with a frontend and backend.

## Project Structure

```
.
├── backend/
│   ├── Dockerfile
│   ├── package.json
│   └── server.js
├── frontend/
│   ├── Dockerfile
│   ├── index.html
│   ├── style.css
│   └── app.js
└── docker-compose.yml
```

## Components

- Backend: Node.js Express API (Port 3000)
- Frontend: Static HTML/CSS/JS served by Nginx (Port 8080)

## Running the Application

1. Start the application:
```bash
docker-compose up --build -d
```

2. Access the application:
- Frontend: http://localhost:8080
- Backend API: http://localhost:3000/api/todos

3. Check running containers:
```bash
docker ps
```

4. Stop the application:
```bash
docker-compose down
```

## Features

- Add new todos
- Mark todos as completed/uncompleted
- Delete todos
- Simple and clean UI

## API Endpoints

- GET /api/todos - Get all todos
- POST /api/todos - Create a new todo
- PUT /api/todos/:id - Toggle todo completion
- DELETE /api/todos/:id - Delete a todo

