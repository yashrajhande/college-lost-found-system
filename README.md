# 🔍 College Lost and Found System

A high-fidelity, full-stack web application designed for college campuses to help students report and recover lost items. Featuring a premium **Dark Glassmorphism** UI, automated item matching, and a secure admin verification portal.

---

## 🚀 Core Features

- **🤖 Intelligent Auto-Matching Engine**: Our system doesn't just store data—it works for you. It automatically analyzes descriptions, categories, and keywords to identify potential matches between lost and found reports in real-time.
- **🛡️ Secure Claim Verification**: To prevent false claims, every match undergoes a rigorous manual verification process by campus admins before an item is released.
- **📸 Evidence-Based Reporting**: Upload high-resolution images and tag items with specific keywords to create a comprehensive digital footprint for every reported object.
- **🔔 Proactive Notifications**: Get instantly notified the moment a potential match is found for your lost item, cutting down recovery time from days to minutes.
- **👥 Role-Based Orchestration**: Separate tailored experiences for Students, Staff, and Admins, ensuring a smooth and secure workflow for the entire campus community.
- **📊 Item Audit Trail**: Full transparency with a detailed history of your reports, including their current status (Pending, Matched, or Returned).
- **🛠️ Centralized Admin Command Center**: A powerful interface for campus authorities to oversee all activities, manage unmatched items, and orchestrate successful returns with ease.

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