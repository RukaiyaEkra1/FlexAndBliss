# Flex & Bliss - E-commerce Website

**Flex & Bliss** is a premium e-commerce platform dedicated to handcrafted home decor, including gypsum masterpieces, scented candles, jewelry, and more. This project is a full-stack web application built with a focus on aesthetics, functionality, and a seamless user experience.

![Flex & Bliss Banner](hero_bg.png)

## 🚀 Features

### Frontend (User Experience)
*   **Stunning UI/UX**: Modern, responsive design with glassmorphism effects, smooth animations, and a rich color palette.
*   **Dynamic Product Catalog**: Browse products by category (Gypsum, Candles, Jewelry, Concrete, Soap, etc.) with real-time search.
*   **Shopping Cart & Wishlist**: Fully functional cart and wishlist with persistent storage.
*   **User Accounts**: Secure registration, login, and profile management with email verification.
*   **Video Hero Slider**: Engaging video backgrounds on the homepage showcasing products.
*   **Micro-interactions**: Interactive hover effects and feedback for all user actions.

### Backend (Admin & Functionality)
*   **Multi-Step Checkout**: A streamlined 4-step checkout process (Cart -> Details -> Payment -> Confirmation).
*   **Payment Integration**: Support for **bKash**, **Nagad**, Credit/Debit Cards, and Cash on Delivery (COD).
*   **Admin Dashboard**:
    *   Monitor detailed statistics (Total Users, Orders, Revenue).
    *   Manage products (Add, Edit, Delete).
    *   View and track customer orders.
    *   Access system logs.
*   **Logging System**: Automated logging of registrations and orders to text files for auditing.
*   **Security**: CSRF protection, secure password hashing, and input validation.

### Technology Stack
*   **Frontend**: HTML5, CSS3 (Vanilla), JavaScript (ES6+)
*   **Backend**: PHP (Native)
*   **Database**: MySQL
*   **Server**: Apache (via XAMPP)

---

## 🛠️ Setup & Installation Guide

This project is designed to run locally using **XAMPP** on Windows.

### Prerequisites
1.  **Download & Install XAMPP**: [https://www.apachefriends.org/](https://www.apachefriends.org/)
2.  **Git**: Ensure Git is installed to clone the repository.

### Step 1: Clone the Repository
Open your terminal/command prompt and run:
```bash
cd C:\xampp\htdocs
git clone https://github.com/RukaiyaEkra1/FlexAndBliss.git
```
*Note: Make sure the folder name is simple, e.g., `flexbliss`.*

### Step 2: Configure the Database
1.  Start **Apache** and **MySQL** in the XAMPP Control Panel.
2.  Open your browser and go to `http://localhost/phpmyadmin`.
3.  Create a new database named **`flexbliss_db`**.
4.  Click **Import** and select the file `flexbliss_deploy_FULL.sql` from the project folder.
5.  Click **Go** to duplicate the database structure.

### Step 3: Verify Configuration
Check `includes/config.php` to ensure the database settings match your environment (default XAMPP settings are usually correct):
```php
define('DB_HOST', 'localhost');
define('DB_NAME', 'flexbliss_db');
define('DB_USER', 'root');
define('DB_PASS', '');
```

### Step 4: Run the Application
*   **Storefront**: Visit `http://localhost/FlexAndBliss/index.html` (or your folder name).
*   **Admin Panel**: Visit `http://localhost/FlexAndBliss/admin/index.php`.

### Default Credentials
*   **Database User**: `root` (No password)
*   **Admin Login**: You may need to register a new account and manually promote it to admin via database or use the registration flow if an admin seeder is not included.

---

## 📂 Project Structure
```
FlexAndBliss/
├── index.html          # Homepage & Main App
├── styles.css          # Global Styles
├── script.js           # Frontend Logic
├── dashboard.php       # User Dashboard
├── admin/              # Admin Panel Files
├── api/                # Backend API Endpoints
├── includes/           # PHP Core Config & Helpers
├── images/             # Product Assets
├── logs/               # System Logs (Orders/Registrations)
└── database.sql        # Database Import File
```

## ✨ License
This project is created by **Rukaiya Binta Hossain Ekra**. All rights reserved.
