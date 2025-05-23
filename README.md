# Restaurant Management MERN Application

## Project Overview

This is a **MERN stack** application for managing restaurant operations, including user authentication, order management, menu management, analytics, and restaurant management. It uses:

* **Frontend:** React (with Vite)
* **Backend:** Node.js with Express
* **Database:** MongoDB
* **Authentication:** JWT
* **Containerization & Deployment:** Docker, Kubernetes (Minikube)

## Features

* **User Authentication:** Register and login users.
* **Protected Routes:** Only authenticated users can access management and analytics.
* **Order Management:** View and manage customer orders.
* **Menu Management:** Create, update, and remove menu items.
* **Analytics Dashboard:** View sales and performance reports.
* **Restaurant Management:** Manage restaurant details and staff.

## Tech Stack

| Component  | Technology         |
| ---------- | ------------------ |
| Frontend   | React, Vite, Axios |
| Backend    | Node.js, Express   |
| Database   | MongoDB            |
| Auth       | JWT, bcrypt        |
| Deployment | Docker, Kubernetes |

---

## Prerequisites

* [Node.js](https://nodejs.org/) v16+
* [npm](https://npmjs.com/) or [yarn](https://yarnpkg.com/)
* [Docker](https://www.docker.com/)
* [Minikube](https://minikube.sigs.k8s.io/docs/) (for local Kubernetes)
* [kubectl](https://kubernetes.io/docs/tasks/tools/)

---

## Installation & Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/AffanWajid12/restaurant-app
   cd restaurant-app
   ```

2. **Environment variables**

   * **Backend**: Create a `.env` in `resturant-backend-main/`:

     ```env
     MONGO_URI=mongodb://<host>:27017/restaurant-db
     PORT=5000
     JWT_SECRET=your_jwt_secret
     JWT_EXPIRES_IN=30d
     ORIGIN=http://localhost:5173
     ```

   * **Frontend**: Create a `.env` in `resturant-frontend-main/`:

     ```env
     VITE_API_URL="http://localhost:5000/api"
     ```

3. **Install dependencies**

   ```bash
   # Backend
   cd resturant-backend-main
   npm install

   # Frontend
   cd ../resturant-frontend-main
   npm install
   ```

---

## Running Locally with Node.js

### Backend

```bash
cd resturant-backend-main
npm run dev       # starts server on http://localhost:5000
```

### Frontend

```bash
cd resturant-frontend-main
npm run dev       # starts Vite dev server on http://localhost:5173
```

Navigate to `http://localhost:5173` in your browser. You should be able to register, login, and explore the dashboard.

---


