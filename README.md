# 🔐 Multi-Factor Authentication (MFA) – Fullstack Example

This project demonstrates how to implement **Multi-Factor Authentication (MFA)** using a fullstack setup with:

- **ReactJS** frontend
- **ExpressJS** backend
- **MongoDB** for storage
- **TOTP** (Time-based One-Time Password) for 2FA

It’s a minimal project built for **educational purposes** to showcase the workflow of user login + MFA using an authenticator app like **Google Authenticator** or **Authy**.

---

## ⚙️ Tech Stack

- **Frontend**: React + Bootstrap
- **Backend**: Express.js
- **Database**: MongoDB
- **MFA**: TOTP via `speakeasy` library
- **QR Code** generation via `qrcode` package

---

## 🔑 Features

- User registration with email and password
- MFA setup using QR code + authenticator app
- Secure login flow with MFA challenge
- Simple frontend (Bootstrap) to demo the full workflow

---

## 🛠️ Setup Instructions

### 🚀 Backend

1. Clone the repo and navigate to the backend folder
2. Create a `.env` file based on the `.env.example`

```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/mfa-demo
JWT_SECRET=your_jwt_secret
```
3. Install dependencies and run:

- npm install
- npm run dev

🖥️ Frontend

Navigate to the frontend folder

```Run:
npm install
npm start
```

The app will open on http://localhost:3000
📸 Demo Flow
    
- Register a new user
- Scan the QR code using an authenticator app
- Enter the 6-digit OTP to verify
- On next login, you’ll be prompted for the OTP

/frontend     → React frontend  
/Backend      → Express backend  
/Backend/.env.example → Environment config sample  
- Password reset
- Email verification
- Session timeout / Remember device toggle
