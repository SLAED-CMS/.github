# LAAS CMS 🚀
**Modern, secure & framework-less Content Management System (PHP 8.4+)**

LAAS CMS is a **security-first, frontend-agnostic CMS** built with pure PHP.  
No frameworks, no magic — just explicit architecture, strong security, and full developer control.

> Successor of **SLAED CMS**, redesigned for modern PHP, operations, and long-term maintainability.

> [!NOTE]  
> LAAS is intentionally **framework-less**.  
> This is a conscious design decision to ensure transparency, predictability, and long-term stability.

---

## ✨ Why LAAS?

LAAS focuses on **clarity over convenience** and **control over abstraction**.

- 🔒 **Security-first** core architecture
- ⚡ **Fast & lightweight** – no unnecessary complexity
- 🧩 **Modular design** (core, modules, blocks)
- 🧠 **Clean template structure** (no framework lock-in)
- 🌍 **Multilingual support**
- 🛠️ **Developer-friendly** (readable code, predictable behavior)

> [!IMPORTANT]  
> LAAS enforces a strict separation of concerns:  
> **Controllers return data only — templates own all markup and presentation logic.**

---

## 📦 Recommended Project

### 👉 **LAAS CMS**
➡️ https://github.com/SLAED-CMS/LAAS

- PHP **8.4+**
- MySQL / MariaDB
- Actively maintained
- **Recommended for all new projects**

---

## 📚 Other Projects

| Project | Status | Description |
|-------|--------|-------------|
| **LAAS** | ✅ Active | Modern CMS (recommended) |
| **SLAED CMS 6.3** | 🟡 Maintenance | Stable legacy version |
| **SLAED CMS 6.2 Pro** | ⚫ Archived | Historical release |

> [!NOTE]  
> SLAED CMS remains available for legacy installations,  
> but all new development and innovation happens in **LAAS**.

---

## ✨ Key Features

### 🔐 Security
- RBAC, CSRF protection, rate limiting
- Session hardening and timeouts
- 2FA / TOTP authentication
- Secure password reset flows
- Sanitized HTML with trust markers and raw-output guards

> [!WARNING]  
> Disabling or bypassing security mechanisms (CSRF, rate limits, raw-output guards)  
> can introduce **critical vulnerabilities** and is strongly discouraged.

### ⚙️ Architecture
- Pure PHP 8.4+ with strict types
- No Laravel, Symfony, or hidden dependencies
- Predictable request lifecycle
- No global state, no magic methods

### 🧩 Modularity
- Self-contained modules
- Explicit routes, controllers, repositories, migrations
- Enable/disable features without side effects

### 🌍 Frontend-agnostic
- HTML or JSON via content negotiation
- Optional headless mode
- Progressive enhancement friendly

### 🛠️ Operations
- Health checks
- Backup & restore
- Audit log
- Performance budgets and guards

### 🤖 Safe AI Runtime (v4.0.0)
- Proposal → Plan → Diff workflow
- Read-only UI previews
- Explicit CLI apply (`--yes`)
- Full auditability

> [!CAUTION]  
> AI features in LAAS **never apply changes automatically**.  
> All modifications require explicit human approval via CLI using `--yes`.

---

## 📦 Requirements

- **PHP:** 8.4+
- **Database:** MySQL 8.0+ or MariaDB 10+
- **Web Server:** Apache / Nginx / IIS
- **Composer:** 2.x
- **Encoding:** UTF-8 (utf8mb4)

Optional:
- Redis (sessions)
- ClamAV (media scanning)
- S3 / MinIO (object storage)

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

- Frontend: http://localhost:8000  
- Admin: http://localhost:8000/admin  
- Health: http://localhost:8000/health  

> [!TIP]  
> Start with the default configuration and explore the system first.  
> LAAS is designed to be understandable without reading the full source code upfront.

---

## 📄 License

MIT License

© Eduard Laas, 2005–2026  
Website: https://laas-cms.org
