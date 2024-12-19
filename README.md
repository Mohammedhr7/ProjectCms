# ProjectCms
 build a web site with wordpress and woocommerce
# WordPress Project Installation Guide

This guide explains how to set up and run the WordPress project on your local machine.

---

## **Requirements**
Before starting, ensure you have the following installed:
- PHP (version 7.4 or higher)
- MySQL or MariaDB
- Apache or Nginx web server
- phpMyAdmin (optional, for database management)

---

## **Step 1: Clone the Repository**
1. Open a terminal or GitHub Desktop.
2. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/wordpress-project.git

Step 2: Import the Database
Open phpMyAdmin or your preferred database management tool.
Create a new database (e.g., wordpress_db).
Import the database file included in the repository:
Navigate to the database folder and select wordpress_db.sql.
Click Go to complete the import.

Step 3: Configure WordPress
Open the wp-config-sample.php file in the root directory.

Rename it to wp-config.php.

Edit the following lines to match your database settings:
define('DB_NAME', 'wordpress_db'); // Database name
define('DB_USER', 'root');        // Your database username
define('DB_PASSWORD', '');        // Your database password
define('DB_HOST', 'localhost');   // Database host

Step 4: Run the WordPress Site
Start your web server and MySQL service:

For XAMPP, use the XAMPP Control Panel.
http://localhost/wordpress-project

Notes
If the site doesn't load, ensure:

PHP and MySQL services are running.
The database is correctly imported.
File permissions are properly set for the wp-content directory.
You can modify the site content and settings from the WordPress admin panel:
http://localhost/wordpress-project/wp-admin

Default admin credentials:
Username: admin (or the one set during setup)
Password: password (or the one set during setup)
