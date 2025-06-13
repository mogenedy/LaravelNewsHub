# 📰 Laravel News Hub

**Laravel News Hub** is a simple yet powerful content management system (CMS) built with Laravel, designed for managing and publishing news articles efficiently.

---

## 📌 Project Overview

Laravel News Hub allows admins and users to manage and browse news content through a clean and organized interface. It includes:

- 🧑‍💼 Admin dashboard for managing news and categories  
- 📰 News article creation, editing, and deletion  
- 🗂️ Category management  
- 👤 User authentication and roles (admin/user)  
- 📄 Blade templating for front-end views  
- 📦 Laravel 10 modern structure  
- 🔌 RESTful API support  

---

## 🚀 Features

- ✅ Admin & user role management  
- ✅ Article CRUD operations  
- ✅ Category management  
- ✅ RESTful API endpoints  
- ✅ Blade-powered frontend  
- ✅ Middleware-protected routes  

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/mogenedy/LaravelNewsHub.git
cd LaravelNewsHub
```

### 2️⃣ Install Dependencies

```bash
composer install
npm install && npm run dev
```

### 3️⃣ Configure Environment

```bash
cp .env.example .env
```

Edit the `.env` file and provide your database credentials.

### 4️⃣ Generate Application Key

```bash
php artisan key:generate
```

### 5️⃣ Run Migrations

```bash
php artisan migrate
```

### 6️⃣ Serve the Application

```bash
php artisan serve
```

Open your browser at: `http://localhost:8000`

---

## 🔐 Authentication & Roles

- Built-in Laravel authentication system
- Role-based access control using middleware
- Admin users can be seeded or created manually in the database

---

## 📡 API Endpoints

All API routes are prefixed with `/api`.

### 🔑 Auth

| Method | Endpoint             | Description           |
|--------|----------------------|-----------------------|
| POST   | `/api/register`      | Register new user     |
| POST   | `/api/login`         | Login and get token   |
| POST   | `/api/logout`        | Logout current user   |

### 📰 Articles

| Method | Endpoint                | Description               |
|--------|-------------------------|---------------------------|
| GET    | `/api/articles`         | Get all articles          |
| GET    | `/api/articles/{id}`    | Get single article        |
| POST   | `/api/articles`         | Create new article (admin) |
| PUT    | `/api/articles/{id}`    | Update article (admin)    |
| DELETE | `/api/articles/{id}`    | Delete article (admin)    |

### 🗂️ Categories

| Method | Endpoint                 | Description                |
|--------|--------------------------|----------------------------|
| GET    | `/api/categories`        | Get all categories         |
| POST   | `/api/categories`        | Create category (admin)    |
| PUT    | `/api/categories/{id}`   | Update category (admin)    |
| DELETE | `/api/categories/{id}`   | Delete category (admin)    |

⚠️ Most admin API routes are protected with auth middleware and require a valid token.

---

## 📂 Folder Structure Highlights

- `app/Http/Controllers` – Web & API controllers
- `routes/web.php` – Web routes
- `routes/api.php` – API routes
- `resources/views` – Blade templates
- `database/migrations` – Database schema

---

