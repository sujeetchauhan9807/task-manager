# Laravel 12 Task Management Application

A Task Management Application built using Laravel 12 and Blade Template Engine with Authentication, CRUD Operations, File Uploads, Search, Filter, Pagination, and AJAX functionality.

---

# Features

## Authentication
- User Registration
- User Login
- Logout Functionality

---

## Task Management (CRUD)
- Create Task
- Edit Task
- Delete Task

---

## Task Fields
- Title
- Description
- Status (Pending / Completed)
- Due Date

---

## User-specific Tasks
Each logged-in user can only:
- View their own tasks
- Edit their own tasks
- Delete their own tasks

---

## File Upload Module
- Multiple File Uploads
- Upload Images & PDFs
- AJAX File Upload
- Preview Images before Upload
- Preview PDF Files


---

## Additional Features
- Pagination
- Search Functionality
- Filter by Status
- Responsive UI
- Toastr Notifications
- Validation & Error Handling

---

# Technologies Used

| Technology | Purpose |
|---|---|
| Laravel 12 | Backend Framework |
| Blade | Templating Engine |
| MySQL | Database |
| jQuery | AJAX Requests |
| Bootstrap / Custom CSS | Frontend UI |
| Laravel Breeze | Authentication |

---

# Installation Guide

## Step 1: Clone Repository

```bash
git clone https://github.com/sujeetchauhan9807/task-manager.git
```

---

## Step 2: Go to Project Folder

```bash
cd task-manager
```

---

## Step 3: Install Dependencies

```bash
composer install
```

```bash
npm install
```

---

## Step 4: Create Environment File

```bash
cp .env.example .env
```

---

## Step 5: Generate Application Key

```bash
php artisan key:generate
```

---

## Step 6: Configure Database

Update `.env` file:

```env
DB_DATABASE=task_manager
DB_USERNAME=root
DB_PASSWORD=
```

---

## Step 7: Run Migrations

```bash
php artisan migrate
```

---

## Step 8: Create Storage Link

```bash
php artisan storage:link
```

---

## Step 9: Run Vite

```bash
npm run dev
```

---

## Step 10: Start Server

```bash
php artisan serve
```

Open:

```text
http://127.0.0.1:8000
```

---

# Authentication Setup

Laravel Breeze used for authentication.

Install using:

```bash
composer require laravel/breeze --dev
```

```bash
php artisan breeze:install
```

```bash
php artisan migrate
```

---

# Project Structure

```text
app/
 ├── Http/
 │   ├── Controllers/
 │   ├── Requests/
 │
resources/
 ├── views/
 │   ├── dashboard.blade.php
 │   ├── task.blade.php
 │   ├── edit.blade.php
 │   ├── upload-files.blade.php
 │
public/
storage/
```

---

# Main Modules

## Dashboard
- Task Listing
- Search
- Filter
- Pagination

---

## Task Module
- Add Task
- Edit Task
- Delete Task

---

## File Upload Module
- AJAX Upload
- Image Preview
- PDF Preview


---

# Validation

Laravel Form Requests used:

- AddTaskRequest
- UpdateTaskRequest


