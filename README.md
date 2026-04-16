# 🔍 College Lost and Found System

A high-fidelity, full-stack web application designed for college campuses to help students report and recover lost items. Featuring a premium **Dark Glassmorphism** UI, automated item matching, and a secure admin verification portal.

---

## ✨ Features

- **Premium UI/UX**: Modern dark-mode interface with glassmorphism effects, GSAP animations, and responsive layouts.
- **Lost & Found Reporting**: Easy-to-use forms for reporting lost or found items with image uploads.
- **Automated Matching**: The system automatically matches lost items with reported found items based on categories and descriptions.
- **Secure Authentication**: Student and Staff login/registration system with JWT-based security.
- **Admin Dashboard**: Specialized portal for admins to review matches, approve returns, and manage unmatched items.
- **History Tracking**: Personal dashboard for users to track the status of their reported items.

---

## 🚀 Getting Started

Follow these steps to set up the project on your local machine.

### 📋 Prerequisites

Before you begin, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v16 or higher)
- [MongoDB](https://www.mongodb.com/try/download/community) (Running locally on port `27017`)
- [Git](https://git-scm.com/)

### 🛠️ Installation & Setup

#### 1. Clone the Repository
```bash
git clone https://github.com/yashrajhande/college-lost-found-system.git
cd college-lost-found-system
```

#### 2. Backend Configuration
Navigate to the `backend` folder and install dependencies:
```bash
cd backend
npm install
```

Create a `.env` file in the `backend` directory and add the following configurations (or use the provided defaults):
```env
MONGODB_URI=mongodb://127.0.0.1:27017/lost_found_db
JWT_SECRET=your_secret_key
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password
```

#### 3. Frontend Setup
The frontend uses Tailwind CSS and GSAP via CDN, so no installation is required for the frontend package itself. However, you will need a way to serve the static files.

---

## 🏃 Running the Project

### 1. Start the Backend
From the `backend` directory, run:
```bash
npm run dev
```
The server will start at `http://localhost:5000`.

### 2. Start the Frontend
You can serve the `frontend` folder using any static file server or by opening `index.html` in your browser. Using `npx serve` is recommended:
```bash
# From the project root
cd frontend
npx serve
```
The frontend will typically be available at `http://localhost:3000`.

---

## 📂 Project Structure

```text
├── backend/
│   ├── config/         # Database connection
│   ├── controllers/    # API logic
│   ├── models/         # Mongoose schemas (User, Items)
│   ├── routes/         # API endpoints
│   ├── uploads/        # Stored item images
│   └── server.js       # Entry point
├── frontend/
│   ├── css/            # Premium design system (style.css)
│   ├── js/             # Frontend logic (auth, admin, animations)
│   ├── assets/         # Logos and static assets
│   └── *.html          # UI Pages (Dashboard, Lost, Found, etc.)
└── README.md
```

---

## 🛠️ Technologies Used

- **Frontend**: HTML5, Vanilla JavaScript, [Tailwind CSS](https://tailwindcss.com/), [GSAP](https://greensock.com/gsap/) (Animations).
- **Backend**: [Node.js](https://nodejs.org/), [Express.js](https://expressjs.com/).
- **Database**: [MongoDB](https://www.mongodb.com/) with [Mongoose](https://mongoosejs.com/).
- **Authentication**: JSON Web Tokens (JWT) & Bcrypt.
- **File Handling**: Multer (for image uploads).

---

## 🤝 Contributing

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

---

## 📝 License
Distributed under the ISC License. 