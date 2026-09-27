# 🎓 Student Management REST API - Web Development Assignment

A robust, production-ready RESTful API built with **Node.js** and **Express.js** designed to efficiently manage student records through complete CRUD (Create, Read, Update, Delete) operations using local JSON data persistence.

---

## 🌟 Table of Contents
1. [Project Overview](#-project-overview)
2. [Technology Stack](#-technology-stack)
3. [Project Architecture & Directory Structure](#-project-architecture--directory-structure)
4. [Key Features & Implementation Details](#-key-features--implementation-details)
5. [API Endpoints Documentation](#-api-endpoints-documentation)
6. [Getting Started & Local Installation](#-getting-started--local-installation)
7. [API Testing Guide (Postman)](#-api-testing-guide-postman)
8. [Error Handling Strategy](#-error-handling-strategy)

---

## 📌 Project Overview
This project was developed as part of the Web Development coursework. It implements a complete backend server architecture following REST principles. It handles incoming HTTP requests, processes student data structures, executes custom logging middleware for tracking traffic, and returns appropriate JSON payloads alongside standard HTTP status codes.

---

## 🛠️ Technology Stack
* **Runtime Environment:** Node.js (v18+ recommended)
* **Framework:** Express.js (v5.1.0)
* **Data Storage:** Local JSON file handling (`students.json`)
* **Environment Control:** Nodemon (for smooth local development)
* **Testing Tool:** Postman / cURL

---

## 📂 Project Architecture & Directory Structure
The application follows a clean, modular MVC-inspired file structure to ensure separation of concerns, scalability, and maintainability:

```text
-Student-Management-REST-API/
│
├── data/
│   └── students.json          # JSON file storing persistent student records
│
├── middleware/
│   └── logger.js              # Custom middleware tracking HTTP methods, URLs, and timestamps
│
├── routes/
│   └── studentRoutes.js       # Modular router handling all student-specific endpoints
│
├── app.js                     # Main application entry point and Express server configuration
├── package.json               # Project metadata, scripts, and dependency definitions
├── package-lock.json          # Dependency tree lock file
└── .gitignore                 # Specifies intentionally untracked files (e.g., node_modules)
