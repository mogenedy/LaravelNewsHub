# 📰 Laravel News Hub

A simple content management system (CMS) for publishing and managing news articles, built with Laravel.

---

## 📌 Project Overview

Laravel News Hub allows admins and users to manage and browse news content through a clean and organized interface. It includes authentication, role-based access (admin/user), article posting, category management, and more.

---

## 🚀 Features

- 🧑‍💼 Admin dashboard to manage news and categories
- 📰 News article creation, editing, and deletion
- 🗂️ Category management
- 👤 User authentication and roles
- 📄 Blade templating for front-end views
- 📦 Laravel 10 project structure
- 🔌 RESTful API for article and user management

---

## 🛠️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/mogenedy/LaravelNewsHub.git
cd LaravelNewsHub

2. Install Dependencies

composer install
npm install && npm run dev

3. Configure Environment

cp .env.example .env

Then edit .env and set your database credentials.

4. Generate App Key

php artisan key:generate

5. Run Migrations

php artisan migrate

6. Serve the App

php artisan serve

Open: http://localhost:8000


---

🔐 Authentication

Laravel built-in authentication used

Admin/user roles handled via middleware

You may seed or manually create an admin user in the database



---

📡 API Endpoints

Here’s a basic list of the available API routes (assuming prefix /api):

🔑 Auth

Method	Endpoint	Description

POST	/api/register	Register new user
POST	/api/login	Login and get token
POST	/api/logout	Logout current user


📰 Articles

Method	Endpoint	Description

GET	/api/articles	Get all articles
GET	/api/articles/{id}	Get single article
POST	/api/articles	Create new article (admin)
PUT	/api/articles/{id}	Update article (admin)
DELETE	/api/articles/{id}	Delete article (admin)


🗂️ Categories

Method	Endpoint	Description

GET	/api/categories	Get all categories
POST	/api/categories	Create new category (admin)
PUT	/api/categories/{id}	Update category (admin)
DELETE	/api/categories/{id}	Delete category (admin)


> ⚠️ Most admin routes are protected with auth middleware and require a valid token.
