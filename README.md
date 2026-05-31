# 🚀 Thumblify – AI-Powered Thumbnail Generator

**Thumblify** is a full-stack MERN application that helps content creators generate, recreate, save, and manage high-quality YouTube thumbnails using AI. It combines **Groq-powered prompt optimization**, **Pollinations image generation**, **JWT authentication**, **credit-based usage tracking**, and a **community feed** into one seamless creator platform. 

---

## 📌 Features

### 🎨 AI Thumbnail Generation

* Generate thumbnails from a topic or title
* Select styles, color palettes, and aspect ratios
* AI optimizes prompts before image generation

### 🔄 Thumbnail Recreate Mode

* Upload or provide an existing image reference
* Describe desired modifications
* Generate improved variations of existing thumbnails

### 🔐 Secure Authentication

* User Signup & Login
* JWT-based authentication
* Protected creator workspace

### 💳 Credit System

* New users receive 15 credits
* One credit deducted per successful generation
* Prevents unlimited AI usage

### 📚 Personal Thumbnail Library

* Save generated thumbnails
* View generation history
* Delete unwanted thumbnails
* Download images anytime

### 🌍 Community Feed

* Browse public thumbnails
* Discover trending ideas
* Like community creations

### ⚡ Prompt Optimization

* Groq AI converts simple user inputs into optimized image-generation prompts
* Produces more visually appealing thumbnail outputs

---

## 🏗️ System Architecture

```text
User
 │
 ▼
React Frontend
 │
 ▼
Express API Server
 │
 ├── JWT Authentication
 ├── Credit Management
 ├── Prompt Optimization (Groq)
 ├── Thumbnail Controller
 │
 ▼
Generated Thumbnail
 │
 ▼
MongoDB Storage
```

---

## 🛠️ Tech Stack

### Frontend

* React 18
* Vite
* React Router v6
* Tailwind CSS
* Context API

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT
* bcryptjs
* Groq SDK
* dotenv
* cors
* morgan

### Database

* MongoDB Atlas

### AI Services

* Groq (Prompt Optimization)
* Pollinations AI (Image Generation)

---

## 📂 Project Structure

```text
Thumblify/
│
├── client/
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   ├── context/
│   │   ├── utils/
│   │   └── App.jsx
│
├── server/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   └── server.js
│
└── README.md
```

---


## 🔗 API Endpoints

### Authentication

| Method | Endpoint         | Description      |
| ------ | ---------------- | ---------------- |
| POST   | /api/auth/signup | Register User    |
| POST   | /api/auth/login  | Login User       |
| GET    | /api/auth/me     | Get Current User |

### AI Generation

| Method | Endpoint                   | Description                 |
| ------ | -------------------------- | --------------------------- |
| POST   | /api/ai/generate-thumbnail | Generate/Recreate Thumbnail |

### Thumbnail Management

| Method | Endpoint                           | Description         |
| ------ | ---------------------------------- | ------------------- |
| GET    | /api/thumbnails                    | Get User Thumbnails |
| DELETE | /api/thumbnails/:id                | Delete Thumbnail    |
| GET    | /api/thumbnails/community          | Community Feed      |
| POST   | /api/thumbnails/community/:id/like | Like Thumbnail      |
| GET    | /api/thumbnails/proxy              | Proxy Remote Images |


## 🎯 Workflow

1. Create an account or login.
2. Access the protected Studio.
3. Choose:

   * Generate Thumbnail
   * Recreate Thumbnail
4. Enter thumbnail details.
5. AI optimizes your prompt.
6. Pollinations generates the image.
7. Thumbnail is saved in MongoDB.
8. Credits are deducted.
9. Browse saved creations in **My Generations**.
10. Explore community thumbnails for inspiration.

---

## 🌟 Key Benefits

* Faster thumbnail creation
* Better prompt-to-image alignment
* AI-enhanced visual quality
* Personal thumbnail history
* Community-driven inspiration
* Secure creator workspace
* Free-tier friendly AI services
* Scalable MERN architecture

---

## 👨‍💻 Future Enhancements

* Premium subscription plans
* Thumbnail analytics
* Custom AI models
* Team collaboration
* Social sharing integrations
* Advanced editing tools
* Cloud image storage
* Real-time thumbnail previews

---

### 💡 Thumblify

**Transform Ideas into Click-Worthy Thumbnails with AI.** 🚀🎨

Source: Thumblify project documentation. 
