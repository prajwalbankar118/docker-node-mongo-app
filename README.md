# 🚀 Node.js + MongoDB CRUD API with Docker

A simple RESTful API built using **Node.js**, **Express.js**, and **MongoDB**, containerized with **Docker** and orchestrated using **Docker Compose**. This app supports full **CRUD** operations on user data.

This project demonstrates how to build, run, and manage a Node.js backend with MongoDB using Docker. It supports basic CRUD (Create, Read, Update, Delete) operations on users.

---

## 📁 Project Structure

docker-node-mongo-app-project/
│
├── backend/
│ ├── Dockerfile
│ ├── server.js
│ ├── models/
│ │ └── User.js
│ ├── package.json
│ └── package-lock.json
├── docker-compose.yml
└── README.md


---

## 🚀 Tech Stack

- **Node.js**
- **Express.js**
- **MongoDB**
- **Docker**
- **Docker Compose**

---

## ⚙️ Prerequisites

Make sure the following are installed on your system:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- [Postman](https://www.postman.com/downloads/)
---

## ▶️ How to Run the App

```bash
# Clone the repo
git clone https://github.com/prajwalbankar118/docker-node-mongo-app.git
cd docker-node-mongo-app

# Build and run containers
docker-compose up --build

The backend API will be available at:
📍 http://localhost:3000

MongoDB will be accessible internally on:
📍 mongodb://mongo:27017/users

📡 API Endpoints (CRUD)
Method	Endpoint	Description	Example (using curl)
POST	/users	Create a user	curl -X POST http://localhost:3000/users -H "Content-Type: application/json" -d '{"name": "Prajwal"}'
GET	/users	Get all users	curl http://localhost:3000/users
DELETE	/users/:id	Delete a user by ID	curl -X DELETE http://localhost:3000/users/<user_id>

## 📬 API Testing

You can test all CRUD endpoints using the included postman_collection.json.
Import it into Postman and start testing instantly.

🔧 Steps to Import:
Open Postman

Click Import

Select the file:  postman_collection.postman_collection.jsonpostman_collection.json

Start testing your endpoints!

Make sure the server (http://localhost:3000) is running before sending requests.


📝 .gitignore
The following files/folders are ignored from version control:

node_modules/
.env


👤 Author
Prajwal Bankar
📧 prajwalbankar118@gmail.com
🔗 GitHub


📌 Notes
MongoDB runs as a Docker service via docker-compose.yml.
The User model is defined in backend/models/User.js.
API requests can be tested using curl, Postman, or any REST client.


🪪 License
This project is licensed under the MIT License.

