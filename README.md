# Prescripto – Doctor Appointment Booking Platform

Prescripto is a **full-stack MERN web application** that allows patients to book doctor appointments online.
The platform provides **separate panels for users, doctors, and administrators**, making healthcare appointment management simple and efficient.

The system supports appointment booking, doctor management, secure authentication, and optional payment integration.

---

## Features

### User Panel

* Browse available doctors
* Book appointments online
* Manage personal profile
* View appointment history

### Doctor Panel

* Doctor login dashboard
* Manage appointment schedule
* View patient booking details

### Admin Panel

* Manage doctors and users
* Monitor appointments
* Platform management dashboard

---

## Tech Stack

### Frontend

* React.js
* Vite
* CSS

### Backend

* Node.js
* Express.js
* MongoDB
* JWT Authentication

### Cloud & Integrations

* Cloudinary (Image storage)
* Razorpay (Payments – optional)
* Stripe (Payments – optional)

---

## Project Structure

```id="projstruct1"
Prescripto
│
├── backend
│   ├── controllers
│   ├── models
│   ├── routes
│   └── server.js
│
├── frontend
│   └── React patient panel
│
├── admin
│   └── React admin dashboard
```

---

# Installation & Setup

## 1. Clone the Repository

```id="clone1"
git clone https://github.com/kaif8077/Prescripto.git
cd Prescripto
```

---

# Backend Setup

Open terminal inside backend folder:

```id="backend1"
cd backend
npm install
```

Create a `.env` file inside the **backend** folder.

Example `.env`:

```id="envexample1"
CURRENCY="INR"

JWT_SECRET="your_jwt_secret"

# Admin Credentials
ADMIN_EMAIL="admin@example.com"
ADMIN_PASSWORD="admin_password"

# MongoDB
MONGODB_URI="your_mongodb_connection_string"

# Cloudinary
CLOUDINARY_NAME="your_cloudinary_name"
CLOUDINARY_API_KEY="your_api_key"
CLOUDINARY_SECRET_KEY="your_secret_key"

# Razorpay (Optional)
RAZORPAY_KEY_ID="your_key"
RAZORPAY_KEY_SECRET="your_secret"

# Stripe (Optional)
STRIPE_SECRET_KEY="your_stripe_key"
```

Run backend server:

```id="backendrun1"
npm run server
```

Backend will start on:

```id="backendport1"
http://localhost:4000
```

---

# Frontend Setup

Open terminal inside **frontend** folder:

```id="frontend1"
cd frontend
npm install
npm run dev
```

Frontend runs on:

```id="frontendport1"
http://localhost:5173
```

---

# Admin Panel Setup

Open terminal inside **admin** folder:

```id="admin1"
cd admin
npm install
npm run dev
```

Admin dashboard runs on:

```id="adminport1"
http://localhost:5174
```

---

# External Services Setup

## MongoDB

1. Create account on MongoDB Atlas
2. Create a new cluster
3. Create database user
4. Copy connection string
5. Add it to `.env` as `MONGODB_URI`

---

## Cloudinary

1. Create account at https://cloudinary.com
2. Open Dashboard
3. Copy

   * Cloud Name
   * API Key
   * API Secret
4. Add them in `.env`

---

## Payment Integration (Optional)

### Razorpay

Create account → get keys → add to `.env`.

### Stripe

Create account → get secret key → add to `.env`.

---

# Running the Project

Start servers in this order:

1️⃣ Backend
2️⃣ Frontend
3️⃣ Admin panel

Make sure backend is running before starting frontend or admin.

---

# Author

Mohd Kaif

GitHub
https://github.com/kaif8077

LinkedIn
https://www.linkedin.com/in/kaif8077/

LeetCode
https://leetcode.com/u/kaif807/
