📓 Table of Contents

About the Project

Tech Stack

Features

Environment Variables

Getting Started

Prerequisites

Run Locally

Run with Docker

To-do

Contributing

License

Contact

Acknowledgements

⭐ About the Project

A web application for conducting online multiple-choice tests (MCQs) for students, teachers, and admins.

👾 Tech Stack

🎯 Features

Student User

View available tests

Register for tests

Attempt tests

View results with explanations

Teacher User

Create and update questions

Create and manage tests

Admin User

Create and manage teacher accounts

Manage subjects and categories

🔑 Environment Variables

To run this project, create a backend/config.json file with:

{
  "mongodb": {
    "connectionString": "<your_mongo_uri>"
  },
  "jwt": {
    "secret": "<your_jwt_secret>"
  }
}

🛠️ Getting Started

‼️ Prerequisites

Node.js and npm

MongoDB (local or cloud)

🏃‍♂️ Run Locally

git clone https://github.com/chintan-golakiya/online-exam-portal.git
cd online-exam-portal

Install dependencies:

cd backend && npm install
cd ../frontend && npm install
cd ../user-portal-frontend && npm install

Start each service:

cd backend && npm start
cd ../frontend && npm start
cd ../user-portal-frontend && npm start

Default admin user is created on the first run.
Username: sysadmin, Password: systemadmin
Logic inside addAdminIfNotFound() in backend/services/admin.js

🚢 Run With Docker

docker-compose build
docker-compose up

Access services:

Backend: http://localhost:5000/

Admin Frontend: http://localhost:3100/

Student/Teacher Frontend: http://localhost:3200/

📄 To-do



👋 Contributing

Contributions are welcome!

Fork -> Clone -> Create Branch -> Commit Changes -> Open Pull Request

⚠️ License

This project is currently not under any license.

💫 Acknowledgements

Material UI

Passport.js

Awesome Readme Template

