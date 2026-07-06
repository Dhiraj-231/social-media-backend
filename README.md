# 🌐 Social Media Platform Backend

<div align="center">

A **feature-rich social media backend** with user management, posts, comments, and real-time interactions.

[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)](https://spring.io/)
[![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)](https://www.java.com/)
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![REST API](https://img.shields.io/badge/REST%20API-009688?style=for-the-badge)](https://restfulapi.net/)
[![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge)](https://jwt.io/)

</div>

---

## ✨ Core Features

✅ **User Management** - Registration, profiles, follow/unfollow  
✅ **Posts & Comments** - Create, edit, delete posts and comments  
✅ **Likes & Reactions** - Like/unlike functionality  
✅ **User Feed** - Personalized feed based on follows  
✅ **Search** - Search users and posts  
✅ **Notifications** - Activity notifications  
✅ **Authentication** - Secure JWT-based auth  
✅ **Media Support** - Image uploads and storage  

---

## 🏗️ Database Schema

```
Users
  ├── id (PK)
  ├── username
  ├── email
  ├── password (encrypted)
  └── profile_data

Posts
  ├── id (PK)
  ├── user_id (FK)
  ├── content
  ├── created_at
  └── updated_at

Comments
  ├── id (PK)
  ├── post_id (FK)
  ├── user_id (FK)
  └── content

Likes
  ├── user_id (FK)
  ├── post_id (FK)
  └── liked_at
```

---

## 🛠️ Tech Stack

- **Backend:** Spring Boot, Java
- **Database:** MySQL with JPA
- **Authentication:** JWT
- **API Documentation:** Swagger
- **File Storage:** Local/Cloud
- **Caching:** Redis (optional)

---

## 📡 API Endpoints

```
Authentication
  POST   /api/auth/register
  POST   /api/auth/login

Users
  GET    /api/users/{id}
  PUT    /api/users/{id}
  POST   /api/users/{id}/follow
  DELETE /api/users/{id}/follow

Posts
  GET    /api/posts/feed
  POST   /api/posts
  DELETE /api/posts/{id}
  POST   /api/posts/{id}/like

Comments
  POST   /api/posts/{id}/comments
  DELETE /api/comments/{id}
```

---

## 🚀 Installation

```bash
git clone https://github.com/Dhiraj-231/social-media-backend.git
cd social-media-backend
gradle build
gradle bootRun
```

---

## 👨‍💻 Author

**Dhiraj Ray** - [GitHub](https://github.com/Dhiraj-231)

---

<div align="center">**Connect. Share. Inspire.**</div>
