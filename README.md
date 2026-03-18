# 🔐 Laravel Auth API

ระบบ Authentication แบบ RESTful API ที่พัฒนาด้วย Laravel สำหรับจัดการการสมัครสมาชิกและเข้าสู่ระบบด้วย Token

---

## 💡 เกี่ยวกับโปรเจกต์

โปรเจกต์นี้ถูกพัฒนาขึ้นเพื่อแสดงทักษะด้าน Backend Development โดยใช้ Laravel
เน้นการออกแบบ API ที่ปลอดภัย ใช้งานจริงได้ และมีโครงสร้างโค้ดที่เป็นมาตรฐาน

---

## 🚀 ความสามารถ (Features)

* สมัครสมาชิก (Register)
* เข้าสู่ระบบ (Login ด้วย Token)
* ออกจากระบบ (Logout)
* ดึงข้อมูลผู้ใช้งาน (User Profile)
* ป้องกันเส้นทาง API ด้วย Middleware

---

## 🛠 เทคโนโลยีที่ใช้

* Laravel (PHP Framework)
* MySQL
* Laravel Sanctum (Token Authentication)

---

## ⚙️ วิธีติดตั้ง (Installation)

```bash id="6a1d4v"
git clone https://github.com/zenxitz/laravel-auth-api.git
cd laravel-auth-api

composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```

---

## 🔑 API Endpoints

| Method | Endpoint      | รายละเอียด                   |
| ------ | ------------- | ---------------------------- |
| POST   | /api/register | สมัครสมาชิก                  |
| POST   | /api/login    | เข้าสู่ระบบ                  |
| GET    | /api/user     | ดึงข้อมูลผู้ใช้ (ต้อง login) |
| POST   | /api/logout   | ออกจากระบบ (ต้อง login)      |

---

## 🧪 ตัวอย่าง Request (Login)

```json id="p8y7c9"
{
  "email": "test@example.com",
  "password": "123456"
}
```

---

## 🧪 ตัวอย่าง Response

```json id="v0k3z2"
{
  "status": "success",
  "message": "เข้าสู่ระบบสำเร็จ",
  "token": "your_token_here"
}
```

---

## 🔒 ระบบความปลอดภัย

API นี้ใช้ Laravel Sanctum สำหรับจัดการ Token และการยืนยันตัวตน

---

## 📦 การทดสอบ API

สามารถทดสอบ API ได้ผ่าน:

* Postman
* Thunder Client
* หรือเครื่องมืออื่น ๆ

---

## 👨‍💻 ผู้พัฒนา

Zenxitz

---

## 📄 License

MIT
