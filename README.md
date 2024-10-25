# User Management Web Application

This project is a simple web-based user management system that allows you to send GET and POST requests to manage a list of users. Users can be added or deleted, and the application displays the current list of users dynamically. The frontend is built with HTML, CSS, and JavaScript, while the backend is a Python server. The entire application can be run using Docker with NGINX as a reverse proxy.

## Features

- **GET Requests**: Retrieve the list of current users from the backend server.
- **POST Requests**: Add new users to the backend.
- **DELETE Requests**: Remove users from the backend.
- **Frontend**: A simple HTML/CSS form to send GET, POST, and DELETE requests using JavaScript.
- **Backend**: A Python server using `http.server` to handle user data and serve it as JSON.


## How It Works

### Frontend
The frontend consists of:
- A form that sends **GET**, **POST**, and **DELETE** requests to the backend.
- A dynamically generated user list that displays the current users in the system.
- JavaScript functions to handle asynchronous requests using the Fetch API.

### Backend
The backend:
- Handles **GET** requests to serve the list of users.
- Handles **POST** requests to add a new user.
- Handles **DELETE** requests to remove users based on their first and last name.
- Stores user data in-memory (temporary storage while the server is running).

### Docker
The project uses Docker for containerized deployment:
- **NGINX** is used as a reverse proxy for the frontend and backend.
- **Python HTTP Server** serves the user data and handles requests.

## Prerequisites

- Docker and Docker Compose installed on your machine.

