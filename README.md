To-Do List Web Application
A full-stack task management application built with Flask (backend) and React + TypeScript (frontend).
Setup Instructions
Backend

Navigate to backend/: cd backend
Create and activate a virtual environment:
Windows: python -m venv venv and venv\Scripts\activate
Mac/Linux: python -m venv venv and source venv/bin/activate


Install dependencies: pip install -r requirements.txt
Create .env file with:SECRET_KEY=your-secure-secret-key-12345
DATABASE_URL=sqlite:///tasks.db

Generate a secure key using openssl rand -hex 32.
Run the backend: python app.py

Frontend

Navigate to frontend/: cd frontend
Install dependencies: npm install
Start the development server: npm run dev
Open http://localhost:5173 in your browser.

Features

User authentication (login, register, logout)
Task management (create, update, delete, filter, search)
Drag-and-drop task reordering
Task comments and attachments
Task categories
Task reminders with browser notifications
Task sharing with other users
Task analytics (pie chart)
Dark/light mode toggle
Export tasks to CSV

Folder Structure

backend/: Flask backend code
app.py: Main application
models.py: Database models
auth_routes.py: Authentication routes
task_routes.py: Task-related routes
uploads/: Stores uploaded files


frontend/: React frontend code
src/components/: React components (Login, Register, Dashboard, etc.)
src/services/: API service layer
src/App.tsx: Main app with routing
src/index.css: Global CSS with Tailwind


