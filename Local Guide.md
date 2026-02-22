# Indaba Website

**WordPress + XAMPP + VS Code**

This repository contains the custom WordPress theme for the **IndabaX** website. The project is developed locally using **XAMPP**, **WordPress**, and **VS Code**, and version-controlled with **GitHub**.

---

## 📦 Requirements

Make sure you have the following installed:

* XAMPP (Apache + MySQL)
* VS Code
* Git
* A modern web browser (Chrome / Firefox)

---

## 🚀 Local Environment Setup

### 1. Start XAMPP

1. Open **XAMPP Control Panel**
2. Start:

   * Apache
   * MySQL

Both services must be running.

---

### 2. Create the Database (first-time only)

1. In XAMPP, click **Admin** next to MySQL (opens phpMyAdmin)
2. Go to **Databases**
3. Create a database named:

   ```
   indaba_wp
   ```

---

### 3. WordPress Installation Location

Place WordPress inside XAMPP’s `htdocs` folder.

**Windows**

```
C:\xampp\htdocs\indaba
```

**macOS**

```
/Applications/XAMPP/htdocs/indaba
```

Folder structure:

```
indaba/
 ├── wp-admin/
 ├── wp-content/
 └── wp-includes/
```

---

## 🧩 Theme Setup (This Repository)

### 4. Clone the Repository

Navigate to:

```
indaba/wp-content/themes/
```

Clone the repo:

```bash
git clone https://github.com/your-org/indaba-theme.git
```

Resulting structure:

```
wp-content/
 └── themes/
     └── indaba-theme/
```

---

### 5. Open Project in VS Code

Open VS Code and select:

```
indaba/wp-content/themes/indaba-theme
```

This folder is the project root.

---

## ⚙️ VS Code Configuration

### 6. Project Settings

Create the following inside the theme root:

```
indaba-theme/
 └── .vscode/
     └── settings.json
```

Add this to `settings.json`:

```json
{
  "editor.formatOnSave": true,
  "files.autoSave": "afterDelay"
}
```

---

### 7. Recommended VS Code Extensions

* PHP Intelephense
* WordPress Snippets
* Prettier
* GitLens

---

## ▶️ Running the Project

### 8. Open the Website

* Site: `http://localhost/indaba`
* Admin: `http://localhost/indaba/wp-admin`

### 9. Activate the Theme

1. Go to **Appearance → Themes**
2. Activate **IndabaX**

---

## 🔁 Daily Development Workflow

1. Start Apache & MySQL in XAMPP
2. Open VS Code
3. Open the `indaba-theme` folder
4. Make changes
5. Refresh the browser

---

## 🧪 Debugging & Common Issues

### White Screen / Errors

Enable debugging in `wp-config.php`:

```php
define('WP_DEBUG', true);
define('WP_DEBUG_DISPLAY', true);
define('WP_DEBUG_LOG', true);
```

### Changes Not Showing

* Hard refresh: `Ctrl + Shift + R` / `Cmd + Shift + R`

### Apache Won’t Start

* Likely a port 80 conflict
* Change Apache to port **8080** in XAMPP settings

---

## 🌿 Git Workflow

Before starting work:

```bash
git pull
```

After making changes:

```bash
git add .
git commit -m "Describe your change"
git push
```

---

## 📝 Notes

* This repository contains **only the theme**, not WordPress core files
* Do not commit `wp-config.php` or database files

---

## 🤝 Team Onboarding Checklist

* [ ] Install XAMPP
* [ ] Clone the repository
* [ ] Create the database
* [ ] Activate the Indaba theme
* [ ] Confirm the site loads locally


