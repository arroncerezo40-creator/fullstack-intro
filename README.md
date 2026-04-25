# Full Stack Development Lab 1

## Project Overview
This project sets up the foundation for a MERN stack application.

## 1. Client-Server Architecture
The MERN stack architecture allows for a separation of concerns between the user interface and the data processing.

### Components:
* **Client (Browser):** The user's entry point that renders the UI and communicates with the server.
* **Frontend (UI Layer):** Built with technologies like React, this layer handles user interactions and display logic.
* **Backend (Server Layer):** Built with Node.js and Express, this acts as the API that processes requests, executes business logic, and handles data transmission.
* **Database (MongoDB):** A NoSQL database that persists application data.

### Request Flow:
1. The **Client** sends an HTTP request (GET, POST, etc.) to the **Backend**.
2. The **Backend** receives the request, processes it, and communicates with **MongoDB** to retrieve or store information.
3. The **Backend** returns a response (usually JSON) to the **Client**.
4. The **Frontend** receives the response and updates the user interface accordingly.

## 2. Project Structure
The repository is organized to separate the client and server environments:
* `/frontend`: Contains the client-side code.
* `/backend`: Contains the server-side code.