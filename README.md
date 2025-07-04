# 🗂️ Directus Backend – User Profile CRUD API

This backend uses **Directus** to provide a fast, secure, and modular **User Profile CRUD system** with built-in authentication, role-based access control, and REST API endpoints.

---

## 🚀 **Tech Stack**

- **Backend:** Directus (Node.js Headless CMS)
- **Database:** SQLite (for local rapid setup; can switch to MySQL/Postgres)
- **Auth:** Directus email/password login with JWT tokens

---

## ✅ **Features**

- Email/Password based authentication  
- JWT-secured API requests  
- User Profile CRUD with the following fields:
  - `name` (string)
  - `email` (string, unique)
  - `phone` (string)
  - `bio` (text)
  - `avatar` (file upload or URL)
- Role-based access control via Directus Roles & Permissions  
- Auto-generated REST API endpoints

---

## ⚙️ **Setup Instructions**

### 1. Clone Repository

```bash
git clone https://github.com/usman766/directus-crud-backend  
cd directus-crud-backend  

```

---

## 🐳 Docker Setup

You can run the backend using Docker Compose for easy local development:

```bash
docker-compose up -d
```

This will start Directus using the official image, exposing it on port 8055 and persisting data in the `data/` directory using SQLite. You can change the database settings in `docker-compose.yml` if you want to use Postgres or MySQL.

---

## 📬 Postman Collection

A ready-to-use Postman collection for all User Profile CRUD endpoints is included in the project root:

- [directus-postman-collection.json](./directus-postman-collection.json)

Import this file into Postman to quickly test authentication, CRUD, and file upload endpoints.

---
