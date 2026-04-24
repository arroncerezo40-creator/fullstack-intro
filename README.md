Full Stack Development - Lab 1
Project Overview
This repository contains the foundational structure for a MERN stack application. This project demonstrates my understanding of client-server architecture and the separation of concerns in web development.

1. System Architecture & Flow
The application follows a standard MERN stack architecture:

Frontend (UI Layer): Built with React. This is the client-side interface that captures user inputs and displays data returned from the server.

Backend (Server Layer): Built with Node.js and Express. This layer acts as the API, handling client requests, processing business logic, and querying the database.

Database (Data Layer): MongoDB. This is a NoSQL database used to persist application data.

Request Flow:

The Client (Browser) sends an HTTP request to the Backend (Server).

The Backend processes the request and communicates with the Database (MongoDB) to read or write data.

The Database returns the data to the Backend.

The Backend sends the requested data back to the Client in JSON format, which the Frontend then renders for the user.

2. Environment Setup
IDE: Visual Studio Code is being used for development, chosen for its excellent support for JavaScript, Node.js, and version control.

Directory Structure: The project is modularized into frontend/ and backend/ directories to maintain a clean separation of code.