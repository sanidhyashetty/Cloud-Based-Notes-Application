# ☁️ Cloud-Based Online Notes Application

A simple **cloud-based notes management web application** that allows users to **create, edit, and delete notes** securely after logging in.  
The project demonstrates user authentication, data storage on the cloud using **MongoDB Atlas**, and a clean, responsive frontend built using **HTML, CSS, and JavaScript**.

---

## 🚀 Features
- 🔐 **User Authentication:** Signup and login functionality with validation.
- 🗒️ **Add, Edit, and Delete Notes** dynamically.
- ☁️ **Cloud Storage:** All notes are stored in **MongoDB Atlas** for remote access.
- 💻 **Responsive UI:** Built with clean and minimal HTML, CSS, and JS.
- 👥 **User-Specific Data:** Each user can manage their own notes securely.

---

## 🛠️ Tech Stack
**Frontend:**  
- HTML5  
- CSS3  
- JavaScript (Vanilla JS)

**Backend:**  
- Node.js  
- Express.js  

**Database:**  
- MongoDB Atlas (Cloud-based NoSQL Database)

---

## 📦 Project Structure
cloud-notes-app/
│
├── server.js                 # Main Express server file
├── package.json              # Node.js dependencies and scripts
├── .env                      # Environment variables (Mongo URI, PORT, JWT secret)
├── .gitignore                # Git ignore configuration
│
├── models/                   # Database models (Mongoose schemas)
│   ├── User.js               # Defines User schema (name, email, password)
│   └── Note.js               # Defines Note schema (title, content, userId)
│
├── routes/                   # Backend routes (APIs)
│   ├── auth.js               # Signup/Login routes
│   └── notes.js              # CRUD routes for notes (Add, Edit, Delete, View)
│
├── middleware/               # Middleware functions
│   └── authMiddleware.js     # Verifies JWT token and authenticates user
│
├── public/                   # Frontend files served to users
│   ├── index.html            # Main frontend page (UI for login/signup and notes)
│   ├── script.js             # Handles frontend logic and API communication
│   └── style.css             # Styling for the app
│
└── node_modules/             # Auto-generated folder containing dependencies



---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/<your-username>/cloud-notes-app.git
cd cloud-notes-app


2️⃣ Install Dependencies
npm install


3️⃣ Configure MongoDB Atlas

Visit MongoDB Atlas
Create a new cluster and database.
Whitelist your current IP address.

*Get your connection string (example):
mongodb+srv://<username>:<password>@cluster.mongodb.net/cloudnotesdb

*Create a .env file in the project root and add:
PORT=5000
MONGO_URI=your_mongodb_atlas_uri
JWT_SECRET=mySuperSecretKey1234

4️⃣ Run the Application
node server.js

If successful, you’ll see:

Connected to MongoDB Atlas!
Server running on port 5000

5️⃣ Open in Browser
http://localhost:5000

Now you can signup, login, and manage notes stored in the cloud 📝


📚How It Works

User Authentication: The user can sign up or log in.
Notes Management: After logging in, the user can create, edit, and delete notes.
Cloud Database: All notes are stored in MongoDB Atlas, so they remain available even after closing the browser or switching devices.
Data Security: Each user’s notes are linked to their own account using secure JWT authentication.

🧠 Skills Demonstrated

Frontend: HTML, CSS, JavaScript
Backend: Node.js, Express.js
Database: MongoDB Atlas
Cloud Integration: Cloud data storage and access
API Development: RESTful routes for CRUD operations
Version Control: Git & GitHub

📸Demo Preview
<img width="1920" height="873" alt="cloud notes output 2" src="https://github.com/user-attachments/assets/4639a67b-5105-4052-9274-5951854f6959" />


🧑‍🎓 Developer Information

Name: Sanidhya Shetty
🎓 B.E. in Computer Science
📍 Mangalore, India

🏁 Future Enhancements
Add user profile management
Integrate Firebase or Google Authentication
Implement note sharing between users
Deploy on AWS EC2, Render, or Vercel


🪄 Quick Execution Summary

Clone repository
Run npm install
Add .env with MongoDB Atlas URI
Run node server.js
Visit http://localhost:5000
