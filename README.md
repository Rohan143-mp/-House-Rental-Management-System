# 🏠 House Rental Management System

This is a PHP-MySQL-based web application for managing houses, tenants, payments, invoices, and reports for a rental agency or landlord.

---

## 📁 Features

- 🧑 Tenant Management (Add, Edit, Remove)
- 🏘️ Property Listing and Category Management
- 💳 Payment Tracking and Invoice Generation
- 📊 Report Generation (Balance, Payments, etc.)
- 👤 Admin/User Roles and Authentication

---
### ✅ Prerequisites

- [XAMPP](https://www.apachefriends.org/) or any LAMP/WAMP stack
- PHP >= 7.0
- MySQL Server

### 🛠️ Steps

1. **Clone or Extract**
   ```bash
   git clone <this-repo-url>
   # OR extract the `house_rental.zip` contents into your server directory
   ```

2. **Move Folder**
   Move the `house_rental` folder to your local server directory:  
   - For XAMPP: `htdocs/house_rental`
   - For WAMP: `www/house_rental`

3. **Import Database**
   - Open phpMyAdmin
   - Create a new database (e.g., `rental_db`)
   - Import the SQL file: `house_rental/db_rental.sql` *(if available)*

4. **Configure DB Connection**
   - Open `house_rental/db_connect.php`
   - Set your DB credentials:
     ```php
     $conn = new mysqli('localhost', 'root', '', 'rental_db');
     ```

5. **Run App**
   - Open browser and go to:
     ```
     http://localhost/house_rental
     ```

6. **Login Credentials**
   - Admin Panel: `http://localhost/house_rental/login.php`
   - Default Admin:
     - **Username**: `admin`
     - **Password**: `admin123` *(or as set in DB)*

---

## 📂 Project Structure

```
house_rental/
├── admin_class.php
├── ajax.php
├── db_connect.php
├── login.php
├── manage_user.php
├── houses.php
├── tenants.php
├── payments.php
├── reports.php
└── ...
```

---

## 📌 Notes

- Ensure your MySQL and Apache servers are running via XAMPP/WAMP.
- All core files are inside the `house_rental/` directory.
- You can customize styles, templates, and logic as needed.

---

## 📄 License

This project is for educational/demo purposes. Contact the original developer or modify freely under MIT-like terms.
