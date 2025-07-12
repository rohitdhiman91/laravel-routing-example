# Laravel Routing Example — `web.php` vs `api.php`

This mini-project demonstrates how Laravel separates routes for web and API using `web.php` and `api.php`.

## 🧠 Concept

Laravel provides two primary route files:

- `routes/web.php`: For routes using session, CSRF, and cookies (e.g., web pages).
- `routes/api.php`: For stateless API endpoints (e.g., JSON responses for mobile or SPA).

## 📂 Route Examples

### Web Route
- URL: `/dashboard`
- File: `routes/web.php`
- Middleware: `web`
- Returns: Blade view

### API Route
- URL: `/api/users`
- File: `routes/api.php`
- Middleware: `api`
- Returns: JSON

## 🚀 Setup

```bash
git clone https://github.com/rohitdhiman91/laravel-routing-example.git
cd laravel-routing-example
composer install
cp .env.example .env
php artisan key:generate
php artisan serve
```

## Visit the Routes

- `http://127.0.0.1:8000/dashboard`  
  👉 This loads a **Blade view** from the `DashboardController` via a route defined in `web.php`.  
  It uses session, CSRF protection, and other `web` middleware features.

- `http://127.0.0.1:8000/api/users`  
  👉 This returns a **JSON response** from the `UserController` via a route defined in `api.php`.  
  It uses the `api` middleware group, which is stateless — perfect for APIs.

---

## 📩 Stay Connected

Follow me for beginner-friendly Laravel content on:

* GitHub: [@rohitdhiman91](https://github.com/rohitdhiman91)
* Substack: https://rohitdhiman91.substack.com
* Instagram: [@rohitdhiman91](https://instagram.com/rohitdhiman91)

---

## 🏷️ Tags

`#Laravel` `#PHP` `#MVC` `#WebDevelopment` `#Blade` `#Eloquent` `#LaravelForBeginners`

```

