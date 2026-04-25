# Full Stack Development - MERN Lab 1

## 1. MERN Stack Architecture
The MERN stack (MongoDB, Express, React, Node.js) follows a **Client-Server Architecture** where the application is split into two distinct environments that communicate via an API.

* **Frontend (Client Layer - React):** This is the "View." It runs in the user's browser. Its role is to capture user events (clicks, forms) and present the UI. It does not store data; it merely requests data from the backend.
* **Backend (Server Layer - Node.js/Express):** This is the "Controller." It acts as a bridge. It creates an API (endpoints) that the frontend talks to. Node.js provides the runtime environment, and Express provides the framework to handle routing (e.g., getting a list of users or saving a new user).
* **Database (Data Layer - MongoDB):** This is the "Model." It is a NoSQL database that stores data in JSON-like documents. 

## 2. Component Interaction & Data Flow
A critical part of full-stack development is the request-response cycle. Here is the interaction process for a data request (e.g., displaying a list of products):

1.  **Request Initiation:** The user interacts with the **React** frontend. The frontend sends an HTTP request (e.g., `GET /api/products`) to the backend.
2.  **Backend Processing:** The **Express** server receives this request. It validates the request and prepares a query for the database.
3.  **Database Interaction:** The backend connects to **MongoDB**. It performs a database operation (like `find()`) to retrieve the requested information.
4.  **Response:** The backend receives the data from MongoDB, converts it into a JSON object, and sends it back as an HTTP response to the frontend.
5.  **Rendering:** The **React** frontend receives the JSON data and updates the Virtual DOM, which causes the browser to re-render the UI to display the products to the user.

## 3. Why Full Stack?
Using the MERN stack allows for the use of **JavaScript across the entire application**. This "universal language" approach simplifies development because the data format (JSON) is consistent from the database (MongoDB) all the way through the server and into the browser (React). This separation of concerns—where the database handles persistence, the server handles logic, and the browser handles presentation—ensures the application is scalable and maintainable.