# Piyush-s-blog

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Flask](https://img.shields.io/badge/Flask-Framework-black?logo=flask)
![License](https://img.shields.io/badge/License-MIT-green)
![Database](https://img.shields.io/badge/Database-SQLite-orange)
![Status](https://img.shields.io/badge/Status-In%20Development-yellow)

## 📝 Description

Piyush’s Blog is a full-stack blogging web application built using the Flask framework.  
It allows users to create, read, update, and delete (CRUD) blog posts through a clean, responsive interface.  

The project includes user authentication, an admin dashboard, and a comment section powered by Flask extensions such as CKEditor, Bootstrap, and Gravatar.  

This project demonstrates skills in web development, backend logic, database management, and authentication systems.  

## ✨ Features

### 🧾 Blog Management
- 📝 Create, edit, delete, and view posts  
- 🧑‍💼 Admin-only access for managing content  
- 🎨 Rich text post editor with Flask-CKEditor  

### 🔐 Authentication System
- 👤 Register, log in, and log out securely  
- 🔒 Passwords hashed with Werkzeug Security  
- 🧭 Session-based login handling  

### 💬 Comment Section
- 💭 Logged-in users can comment on posts  
- 🧑‍🎨 Gravatar integration for avatars  

### 🎨 Responsive UI
- 📱 Built with Flask-Bootstrap for a modern, mobile-friendly layout  


## 🛠️ Tech Stack

| Category | Technologies |
|-----------|--------------|
| Backend | Python, Flask |
| Frontend | HTML, CSS, Bootstrap, CKEditor |
| Database | SQLite with SQLAlchemy ORM |
| Authentication | Flask-Login, Werkzeug Security |
| Other Tools | Flask-Gravatar, Flask-Bootstrap |


## 📦 Key Dependencies

```
Bootstrap_Flask: 2.2.0
Flask_CKEditor: 0.4.6
Flask_Login: 0.6.3
Flask-Gravatar: 0.5.0
Flask_WTF: 1.2.1
WTForms: 3.0.1
Werkzeug: 3.0.0
Flask: 2.3.2
flask_sqlalchemy: 3.1.1
SQLAlchemy: 2.0.25
```

## 📁 Project Structure

```
.
├── forms.py
├── instance
│   └── posts.db
├── main.py
├── requirements.txt
├── static
│   ├── assets
│   │   ├── favicon.ico
│   │   └── img
│   │       ├── about-bg.jpg
│   │       ├── contact-bg.jpg
│   │       ├── default-profile.jpg
│   │       ├── edit-bg.jpg
│   │       ├── home-bg.jpg
│   │       ├── login-bg.jpg
│   │       ├── post-bg.jpg
│   │       └── register-bg.jpg
│   ├── css
│   │   └── styles.css
│   └── js
│       └── scripts.js
└── templates
    ├── about.html
    ├── contact.html
    ├── footer.html
    ├── header.html
    ├── index.html
    ├── login.html
    ├── make-post.html
    ├── post.html
    └── register.html
```
## 🗂️ Database Models

👤 User  
- id, name, email, password  
- Relationship: One-to-Many with BlogPost and Comment  

📰 BlogPost  
- id, title, subtitle, body, date, img_url  
- Relationship: Many-to-One with User, One-to-Many with Comment  

💬 Comment  
- id, text, author_id, post_id  
- Relationship: Many-to-One with User and BlogPost
  
## 🛠️ Development Setup

### Python Setup
1. Install Python (v3.8+ recommended)
2. Create a virtual environment: `python -m venv venv`
3. Activate the environment:
   - Windows: `venv\Scripts\activate`
   - Unix/MacOS: `source venv/bin/activate`
4. Install dependencies: `pip install -r requirements.txt`


## 👥 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Clone** your fork: `git clone https://github.com/Piyushpal017/Piyush-s-blog.git`
3. **Create** a new branch: `git checkout -b feature/your-feature`
4. **Commit** your changes: `git commit -am 'Add some feature'`
5. **Push** to your branch: `git push origin feature/your-feature`
6. **Open** a pull request

Please ensure your code follows the project's style guidelines and includes tests where applicable.


