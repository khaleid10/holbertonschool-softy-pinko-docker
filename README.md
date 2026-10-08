# Softy Pinko Docker Project

## Description

This project demonstrates how to containerize a web application using Docker, Docker Compose, Flask, and Nginx.

The application consists of a front-end server, back-end API servers, and a reverse proxy that distributes incoming requests.

## Technologies

- Docker
- Docker Compose
- Ubuntu
- Python 3
- Flask
- Flask-CORS
- Nginx
- HTML, CSS, JavaScript

## Project Structure

### Task 0: First Docker Image
Create a Docker image based on Ubuntu that prints "Hello, World!".

### Task 1: Back-end
Create a Flask API running on port 5252.

Endpoint:
GET /api/hello

Response:
Hello, World!

### Task 2: Front-end
Set up an Nginx server to serve the Softy Pinko website on port 9000.

### Task 3: Connecting Front-end and Back-end
Connect the front-end to the Flask API using AJAX and enable CORS.

### Task 4: Docker Compose
Use Docker Compose to build and run the front-end and back-end containers together.

### Task 5: Reverse Proxy
Configure Nginx as a reverse proxy to route requests:

- / to the front-end server
- /api to the back-end server

### Task 6: Horizontal Scaling
Scale the back-end to two API servers using Docker Compose.

Nginx distributes API requests using Round Robin load balancing.

## How to Run

Navigate to the task6 directory:

    cd task6

Build the containers:

    docker compose build

Start the application with two API servers:

    docker compose up --scale back-end=2

Open the application in your browser:

    http://localhost

## Author

Khalid - Holberton School
