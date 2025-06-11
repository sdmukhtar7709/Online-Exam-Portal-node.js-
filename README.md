<div align="center">
  <h1>Online Exam Portal</h1>
  <p>
    A full-featured online examination portal with a Node.js backend and a React.js frontend.
  </p>
</div>

---

# 📓 Table of Contents

* [About the Project](#star2-about-the-project)

  * [Tech Stack](#space_invader-tech-stack)
  * [Features](#dart-features)
  * [Environment Variables](#key-environment-variables)
* [Getting Started](#toolbox-getting-started)

  * [Prerequisites](#bangbang-prerequisites)
  * [Run Locally](#running-run-locally)
  * [Run with Docker](#run-with-docker)
* [To-do](#notes-to-do)
* [Contributing](#wave-contributing)
* [License](#warning-license)
* [Contact](#handshake-contact)
* [Acknowledgements](#gem-acknowledgements)

---

## ⭐ About the Project

A web application for conducting online multiple-choice tests (MCQs) for students, teachers, and admins.

---

### 👾 Tech Stack

<details>
  <summary>Frontend</summary>
  <ul>
    <li><a href="https://reactjs.org/">React.js</a></li>
    <li><a href="https://react-redux.js.org/">React-Redux</a></li>
    <li><a href="https://mui.com/">Material UI</a></li>
    <li>HTML5</li>
    <li>CSS3</li>
  </ul>
</details>

<details>
  <summary>Backend</summary>
  <ul>
    <li><a href="https://nodejs.org/">Node.js</a></li>
    <li><a href="https://expressjs.com/">Express.js</a></li>
    <li><a href="https://www.passportjs.org/">Passport.js</a></li>
  </ul>
</details>

<details>
  <summary>Database</summary>
  <ul>
    <li><a href="https://www.mongodb.com/">MongoDB</a></li>
  </ul>
</details>

---

### 🎯 Features

#### Student User

* View available tests
* Register for tests
* Attempt tests
* View results with explanations

#### Teacher User

* Create and update questions
* Create and manage tests

#### Admin User

* Create and manage teacher accounts
* Manage subjects and categories

---

### 🔑 Environment Variables

To run this project, create a `backend/config.json` file with:

```json
{
  "mongodb": {
    "connectionString": "<your_mongo_uri>"
  },
  "jwt": {
    "secret": "<your_jwt_secret>"
  }
}
```

---

## 🛠️ Getting Started

### ‼️ Prerequisites

* Node.js and npm
* MongoDB (local or cloud)

---

### 🏃‍♂️ Run Locally

```bash
git clone https://github.com/chintan-golakiya/online-exam-portal.git
cd online-exam-portal
```

Install dependencies:

```bash
cd backend && npm install
cd ../frontend && npm install
cd ../user-portal-frontend && npm install
```

Start each service:

```bash
cd backend && npm start
cd ../frontend && npm start
cd ../user-portal-frontend && npm start
```

> Default admin user is created on the first run.
> Username: `sysadmin`, Password: `systemadmin`
> Logic inside `addAdminIfNotFound()` in `backend/services/admin.js`

---

### 🚢 Run With Docker

```bash
docker-compose build
docker-compose up
```

Access services:

* Backend: `http://localhost:5000/`
* Admin Frontend: `http://localhost:3100/`
* Student/Teacher Frontend: `http://localhost:3200/`

---

## 📄 To-do

* [ ] Add more test types
* [ ] Integrate email notifications
* [ ] Add analytics dashboard

---

## 👋 Contributing

Contributions are welcome!

```bash
Fork -> Clone -> Create Branch -> Commit Changes -> Open Pull Request
```

<a href="https://github.com/chintan-golakiya/online-exam-portal/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=chintan-golakiya/online-exam-portal" />
</a>

---

## ⚠️ License

This project is currently not under any license.

---

## 💫 Acknowledgements

* [Material UI](https://mui.com)
* [Passport.js](https://www.passportjs.org/)
* [Awesome Readme Template](https://github.com/Louis3797/awesome-readme-template)
