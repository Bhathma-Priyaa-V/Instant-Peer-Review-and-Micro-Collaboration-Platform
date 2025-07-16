# 🚀 Infinity: Instant Peer Review and Micro-Collaboration Platform

## 💡 Project Overview
**Infinity** is a full-stack web platform designed to enable instant peer reviews and micro-collaboration among students working on academic or personal projects.  
Students can showcase their work at various stages (idea, prototype, final), receive meaningful feedback, track growth, and co-work on project tasks.

Built by **Team Infinity**, this platform aims to bridge the feedback gap in student project development, enhance learning, and promote community-driven collaboration.

---

## ✨ Key Features
- ✅ Upload and manage projects in stage-wise format  
- 💬 Threaded peer reviews with structured comments  
- 🤝 Micro-Collaboration invites for task-specific co-working  
- 🧠 AI-generated feedback summaries using Google Gemini API  
- 📊 Skill tagging and growth analytics  
- 🔔 Like/comment/notification system  
- 📨 Real-time in-app messaging between collaborators  

---

## 🔧 Tech Stack

| Layer       | Technology              |
|------------|--------------------------|
| Frontend   | HTML, CSS, JavaScript    |
| Backend    | Python Flask             |
| Database   | MongoDB                  |
| AI         | Google Gemini API        |
| Messaging  | Threaded in-app messaging|

---

## 🧠 AI & Gemini Integration
The platform integrates **Google Gemini API** to generate concise summaries of peer feedback for each project.

- You must manually insert your Gemini API key in the backend route: `/summarize_feedback`

---

## 🗄️ MongoDB Configuration
MongoDB is used to store all essential data such as users, projects, comments, likes, notifications, microcollabs, and messages.

- Ensure MongoDB is running locally on the default port: `mongodb://localhost:27017/`
- **Database used:** `infinityDB`
- **Collections:**
  - `users`
  - `projects`
  - `comments`
  - `notifications`
  - `likes`
  - `microcollabs`
  - `messages`

---

## 🔑 Authentication
- Session-based login system using Flask.
- Supports **Signup, Login, Logout**
- Role-based UI:
  - Project Owner
  - Collaborator
  - Reviewer

---

## 📁 Project Modules

### 1. Project Dashboard
- Add/Edit/Delete your projects  
- Tag skills & add external links  
- View likes, comments, and suggestions  

### 2. Review Center
- View peer feedback  
- Summarize suggestions using Gemini AI  
- Like or reply to comments  

### 3. MicroCollab Board
- View invites and accept/decline tasks  
- Message thread per collaboration  
- Organized into:
  - **Discover** – Public microcollabs  
  - **My Collabs** – Your created collabs  
  - **Accepted** – Joined collaborations  

---

## 🧪 How to Run Locally

1. **Clone the repository**

2. **Install dependencies**

3. **Make sure MongoDB is running on** `localhost:27017`

4. **Start the Flask server**
   ```bash
   python app.py

 5. **Visit the app on:**
  ```bash
  http://127.0.0.1:5000/

❗ Notes
Gemini API Key is used in /summarize_feedback route (backend).

For public GitHub usage, do not include the API key. Keep it private.

👥 Team Infinity
Shiva Nandhini R 

Bhathma Priyaa V

Suja Bala J
