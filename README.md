🧩 Django-React Full Stack App

A full-stack web application built with Django REST Framework as the backend and React.js as the frontend.
This project demonstrates a complete CRUD (Create, Read, Update, Delete) flow where users can register, authenticate, and manage notes through a seamless API-driven interface.

🧠 Overview

The Django-React Full Stack App integrates two powerful technologies — Django for backend logic and database handling, and React for the frontend user interface.
It serves as a practical example of connecting a RESTful API with a modern frontend, handling authentication, and managing persistent data.

The app allows users to:

Register an account

Log in securely

Create, view, update, and delete notes

View notes filtered by the authenticated user

⚙️ Core Features

👤 User Authentication

User registration and login using Django’s built-in User model.

Secure password hashing and authentication handled by Django REST Framework (DRF).

JWT or session-based authentication for API access (depending on configuration).

🧾 Notes Management (CRUD)

Authenticated users can create, edit, delete, and view personal notes.

Notes are tied to the user who created them (via the author field).

Each note includes:

title

content

created_at

author (read-only, auto-assigned)

⚡ REST API Endpoints

Built using Django REST Framework, the API exposes endpoints such as:

POST /api/register/ → User registration

POST /api/token/ → Login and retrieve access token

GET /api/notes/ → List user’s notes

POST /api/notes/ → Create a note

PUT /api/notes/<id>/ → Update a note

DELETE /api/notes/<id>/ → Delete a note

🎨 React Frontend

Responsive and intuitive UI for interacting with the API.

Axios is used for API requests.

React Router for navigation between pages.

Real-time UI updates on CRUD operations.

🛠️ Tech Stack

Layer	Technology

Frontend	React.js (JavaScript, JSX, Axios, React Router)

Backend	Django & Django REST Framework

Database	SQLite (default)

Authentication	Django’s built-in auth system

Deployment Ready	Procfile & requirements.txt for Render

📦 Installation & Setup
🔹 Backend (Django)

1️⃣ Navigate to backend folder:

cd backend


2️⃣ Create and activate a virtual environment:

python -m venv venv

venv\Scripts\activate 


3️⃣ Install dependencies:

pip install -r requirements.txt


4️⃣ Run migrations:

python manage.py migrate


5️⃣ Start the development server:

python manage.py runserver


Backend runs at: http://127.0.0.1:8000/

🔹 Frontend (React)

1️⃣ Navigate to frontend folder:

cd frontend


2️⃣ Install dependencies:

npm install


3️⃣ Create .env file:

REACT_APP_API_URL=http://127.0.0.1:8000/api


4️⃣ Run the frontend:

npm start


Frontend runs at: http://localhost:3000

🧠 Objectives

Understand backend API creation with Django REST Framework

Consume APIs from a React frontend

Manage authentication securely

Implement CRUD operations with persistence

Connect and deploy a Django + React application

🚀 Deployment

This project is deployable on platforms such as:

Choreo

Make sure to include:

Procfile for backend startup command

Environment variables for production settings

CORS configuration to allow your frontend domain

🏁 Conclusion

The Django-React Full Stack App showcases the full workflow of building, connecting, and deploying a modern web application using Python and JavaScript technologies.
It’s an ideal foundation for expanding into task management, blogging platforms, or note-taking SaaS applications.
