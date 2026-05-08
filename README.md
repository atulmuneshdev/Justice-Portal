# ⚖️ Justice New - Legal Connectivity Platform

[![React](https://github.com/atulmuneshdev/Justice-Portal/blob/main/clint/public/Screenshot%202026-04-15%20193112.png)](https://reactjs.org/)
[![Node.js](https://github.com/atulmuneshdev/Justice-Portal/blob/main/clint/public/Screenshot%202026-04-15%20192606.png)](https://nodejs.org/)
[![Express](https://img.shields.io/badge/Express-5.x-000000?logo=express&logoColor=white)](https://expressjs.com/)
[![MongoDB](https://github.com/atulmuneshdev/Justice-Portal/blob/main/clint/public/Screenshot%202026-04-15%20192546.png)](https://www.mongodb.com/)
[![TailwindCSS](https://github.com/atulmuneshdev/Justice-Portal/blob/main/clint/public/Screenshot%202026-04-15%20192606.png)

A robust MERN stack application designed to bridge the gap between clients seeking legal aid and professional advocates. It provides a seamless interface for communication, case tracking, and community engagement.

---

## 📸 Screenshots

| Dashboard View | Chat Interface |
| :---: | :---: |
| ![Dashboard Placeholder](https://github.com/atulmuneshdev/Justice-Portal/blob/main/clint/public/Screenshot%202026-04-15%20192531.png) | ![Chat Placeholder](https://github.com/atulmuneshdev/Justice-Portal/blob/main/clint/public/Screenshot%202026-04-15%20193045.png) |
| *Comprehensive view of cases and stats* | *Instant messaging between clients and advocates* |

| Advocate Profile | Community Feed |
| :---: | :---: |
| ![Profile Placeholder](https://github.com/atulmuneshdev/Justice-Portal/blob/main/clint/public/Screenshot%202026-05-07%20141613.png) | ![Feed Placeholder](https://github.com/atulmuneshdev/Justice-Portal/blob/main/clint/public/Screenshot%202026-04-15%20192606.png) |
| *Detailed professional portfolio* | *Latest updates and posts from the legal community* |

---

## 🚀 Key Features

### 👥 User Roles & Profiles
- **Advocates**: Professional profiles with experience details, case history, and a blue/indigo themed dashboard.
- **Clients**: User-friendly profiles to manage personal cases and search for legal help, with a teal/emerald themed interface.

### 💬 Real-time Interaction
- **Instant Messaging**: Secure, real-time chat powered by **Socket.io**.
- **Notifications**: Real-time alerts for messages and case updates.

### 📁 Case & Post Management
- **Case Tracking**: Create, view, and update legal cases through a dedicated management portal.
- **Social Feed**: Create posts with image/video support (via **ImageKit**) to share knowledge or updates.
- **Engagement**: Like and comment on posts to interact with other professionals.

### 🔍 Discovery
- **Find Advocates**: Advanced search functionality to filter advocates based on location, expertise, and rating.

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: React 19 (Vite)
- **Styling**: Tailwind CSS 4, Framer Motion (Animations)
- **Icons**: Lucide React
- **State/Routing**: React Context API, React Router 7

### Backend
- **Server**: Node.js, Express 5
- **Database**: MongoDB (Mongoose ODM)
- **Real-time**: Socket.io
- **Media**: ImageKit (CDN), Multer

---

## 📁 Project Structure

```text
Collage/
├── backent/                # Express.js Backend
│   ├── src/
│   │   ├── controllers/    # Request handlers & logic
│   │   ├── models/         # MongoDB Schemas
│   │   ├── routes/         # API Endpoint definitions
│   │   ├── middleware/     # Auth & Upload middleware
│   │   └── socket/         # Socket.io events
│   └── server.js           # Server entry point
└── clint/                  # React Frontend
    ├── src/
    │   ├── components/     # UI building blocks
    │   ├── context/        # Global state (Auth, Notifications)
    │   ├── pages/          # Full-page components
    │   └── api/            # Axios configurations
    └── vite.config.js      # Build & Dev settings
```

---

## ⚙️ Getting Started

### 📋 Prerequisites
- **Node.js**: v18 or higher
- **MongoDB**: A local instance or MongoDB Atlas URI
- **ImageKit Account**: For handling media uploads

### 🔧 Installation & Setup

1. **Clone & Install Dependencies**
   ```bash
   git clone <repository-url>
   cd Collage
   
   # Backend
   cd backent
   npm install
   
   # Frontend
   cd ../clint
   npm install
   ```

2. **Environment Configuration**
   Create a `.env` file in the `backent/` directory:
   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_secure_random_string
   IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
   IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
   IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
   ```

### 🏃 Running Locally

**Method 1: Separate Terminals (Recommended)**
- **Terminal 1 (Backend)**: `cd backent && npm start`
- **Terminal 2 (Frontend)**: `cd clint && npm run dev`

---

## 📡 API Reference (Brief)

| Endpoint | Method | Description |
| :--- | :--- | :--- |
| `/api/auth/advocate/signup` | POST | Register as an Advocate |
| `/api/auth/client/login` | POST | Login as a Client |
| `/api/posts` | GET | Fetch all community posts |
| `/api/posts` | POST | Create a new post with media |
| `/api/messages/:id` | GET | Retrieve chat history |

---

## 📄 License
This project is licensed under the **ISC License**.
