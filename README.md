# LAAS CMS 🚀
**Modern, secure & framework-less Content Management System (PHP 8.4+)**

LAAS CMS is a **security-first, frontend-agnostic CMS** built with pure PHP.
No frameworks, no magic — just predictable architecture, strong security, and full developer control.

> Successor of **SLAED CMS**, redesigned for modern PHP, operations, and long-term maintainability.

---

## ✨ Key Features

- 🔒 **Security-first architecture**
  - RBAC, CSRF protection, rate limiting, session hardening
  - 2FA / TOTP, secure password reset flows
  - Sanitized HTML with trust markers and raw-output guards
- ⚙️ **Pure PHP (no frameworks)**
  - PHP 8.4+, strict types
  - No Laravel, Symfony, or hidden dependencies
- 🧩 **Modular system**
  - Self-contained modules (routes, controllers, repositories, migrations, translations)
- 🧠 **Predictable & explicit**
  - No magic methods, no global state
  - Clear request lifecycle and data flow
- 🌍 **Frontend-agnostic**
  - HTML or JSON via content negotiation
  - Headless mode supported
- 🛠️ **Ops-friendly**
  - Health checks, backups, audit log, performance budgets
- 🤖 **Safe AI runtime (v4.0.0)**
  - Proposal → Plan → Diff → CLI apply (`--yes`)
  - No AI auto-apply, full auditability

---

## 📦 Requirements

- **PHP:** 8.4+
- **Database:** MySQL 8.0+ or MariaDB 10+
- **Web Server:** Apache / Nginx / IIS
- **Composer:** 2.x
- **Encoding:** UTF-8 (utf8mb4)

---

## 🚀 Quick Start

```bash
git clone https://github.com/SLAED-CMS/LAAS.git
cd LAAS
composer install
```

1. Copy `.env.example` → `.env`
2. Configure database credentials
3. Run migrations:

```bash
php tools/cli.php migrate:up
```

4. Start a local server:

```bash
php -S localhost:8000 -t public/
```

---

## 📄 License

MIT License

© Eduard Laas, 2005–2026  
Website: https://laas-cms.org
