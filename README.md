# Referral-Rewards
# 🔗 Referral App

A full-stack Referral App built with React, Node.js, Express.js and MongoDB.

The application allows users to create an account, receive a unique referral code and referral link, share the link with others, and earn points when new users register through their referral link.

---

## 🚀 Features

### Authentication
- User Signup
- User Login
- Email validation
- Password validation
- Duplicate email prevention

### Referral System
- Unique referral code for every user
- Automatic referral link generation
- Referral code captured during signup
- Referral attribution
- Referral rewards
- Points system
- Prevention of changing an existing referral relationship

### Dashboard
- User information
- Referral code
- Referral link
- Total referrals
- Total points
- List of referred users

### Backend
- REST APIs
- Express.js routes
- MongoDB database
- Mongoose models
- Error handling

---

# 🛠️ Technologies Used

## Frontend

- React.js
- Vite
- React Router
- CSS

## Backend

- Node.js
- Express.js
- MongoDB
- Mongoose

---

# 📁 Project Structure

```text
Referral/
│
├── Backend/
│   │
│   ├── config/
│   │   └── db.js
│   │
│   ├── models/
│   │   └── User.js
│   │
│   ├── Routes/
│   │   └── Authroutes.js
│   │
│   ├── server.js
│   ├── package.json
│   └── package-lock.json
│
│
└── Frontend/
    │
    ├── public/
    │
    ├── src/
    │   │
    │   ├── components/
    │   │   ├── Dashboard.jsx
    │   │   ├── Signin.jsx
    │   │   └── Signup.jsx
    │   │
    │   ├── App.jsx
    │   ├── main.jsx
    │   └── index.css
    │
    ├── package.json
    ├── package-lock.json
    └── vite.config.js

    1. User signs up
        ↓
2. Backend creates referral code
        ↓
3. Referral link is created
        ↓
4. User shares the link
        ↓
5. New person opens the link
        ↓
6. New person signs up
        ↓
7. Backend finds the referrer
        ↓
8. Save "referredBy"
        ↓
9. Referrer gets +10 points
        ↓
10. Dashboard shows referrals + points
