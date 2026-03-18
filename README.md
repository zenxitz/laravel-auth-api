<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

# 🔐 Laravel Auth API

RESTful Authentication API built with Laravel.

---

## 🚀 Features

* Register
* Login (Token-based)
* Logout
* Get User Profile
* Protected Routes (Middleware)

---

## 🛠 Tech Stack

* Laravel
* MySQL
* Laravel Sanctum

---

## ⚙️ Installation

```bash
git clone https://github.com/yourname/laravel-auth-api.git
cd laravel-auth-api

composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```

---

## 🔑 API Endpoints

| Method | Endpoint      | Description   |
| ------ | ------------- | ------------- |
| POST   | /api/register | Register user |
| POST   | /api/login    | Login user    |
| GET    | /api/user     | Get profile   |
| POST   | /api/logout   | Logout        |

---

## 🧪 Example Response

```json
{
  "status": "success",
  "message": "Login successful",
  "token": "your_token_here"
}
```

---

## 📄 License

MIT

