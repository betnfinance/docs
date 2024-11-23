---
description: If you plan to use a machine from Digital Ocean / Vultr ETC.
---

# VPS Installation.

***

#### Step-by-Step Installation Instructions for Betn on a VPS

**Prerequisites:**

1. **LAMP Stack**: Make sure you have a LAMP (Linux, Apache, MySQL, PHP) server setup. This setup includes: ([Server Requirement](server-requirements.md)s for full list)
   * **Linux** (Ubuntu or CentOS, for instance)
   * **Apache** web server
   * **MySQL 8.0** database server (or MariaDB, depending on your preference)
   * **PHP 8.2 or later** (preferably the latest version compatible with Betriver)
2.  **Composer** and **Node.js/NPM** installed on your server:

    * **Composer**: A dependency manager for PHP, required to install PHP packages.
    * **Node.js and NPM**: Node Package Manager, required for frontend assets.\\





**Detailed  Steps:**

1. **Set Up Your Web Root**:
   * Point your Apache web server’s DocumentRoot to the `public` directory inside your site directory.
   *   Example for Apache configuration (`/etc/apache2/sites-available/betriver.io.conf`):

       ```apache
       <VirtualHost *:80>
           ServerName betriver.io
           DocumentRoot /var/www/betriver.io/public
           
           <Directory /var/www/betriver.io/public>
               AllowOverride All
               Require all granted
           </Directory>

           ErrorLog ${APACHE_LOG_DIR}/betriver.io-error.log
           CustomLog ${APACHE_LOG_DIR}/betriver.io-access.log combined
       </VirtualHost>
       ```
   *   After updating this file, enable the site and restart Apache:

       <pre class="language-bash"><code class="lang-bash"><strong>sudo a2ensite betriver.io.conf
       </strong>sudo systemctl reload apache2
       </code></pre>
2. **Extract the Application Files**:
   * Upload `Betriver``-vps.zip` to your `/var/www/` directory.
   *   Extract the zip file:

       ```bash
       sudo unzip Betriver-vps.zip -d /var/www/
       ```
   *   Rename the extracted folder to your site name, for example:

       ```bash
       sudo mv /var/www/Betriver /var/www/betriver.io
       ```
3. **Navigate to the Site Directory**:
   *   Change directory to your newly created site folder:

       ```bash
       cd /var/www/betriver.io
       ```
4. **Install PHP Dependencies**:
   *   Run Composer to install the necessary PHP packages:

       ```bash
       composer install
       ```
   * This will create a `vendor` directory containing all the required PHP packages.
5.  **Set Up Frontend Assets**:

    *   Run NPM to build frontend assets:

        ```bash
        npm install
        npm run production
        ```


6. **Configure Environment Variables**:
   *   rename the `env.file` file to `.env`:

       ```bash
       cp .env.file .env
       ```
   *   Update `.env` with your database and other configuration details:

       ```env
       DB_CONNECTION=mysql
       DB_HOST=127.0.0.1
       DB_PORT=3306
       DB_DATABASE=your_database_name
       DB_USERNAME=your_database_user
       DB_PASSWORD=your_database_password
       ```
7. **Generate Application Key**:
   *   Run the following command to generate a unique application key:

       <pre class="language-bash"><code class="lang-bash"><strong>php artisan key:generate
       </strong></code></pre>
8. **Run Database Migrations and Seeders**:
   *   Migrate the database tables and seed initial data:

       ```bash
       php artisan migrate --seed
       ```
9. **Set Folder Permissions**:
   *   Ensure the necessary permissions for the `storage` and `bootstrap/cache` directories:

       ```bash
       sudo chmod -R 775 storage bootstrap/cache
       sudo chown -R www-data:www-data storage bootstrap/cache
       ```
10. **Restart Apache**:
    *   Finally, restart Apache to ensure all configurations are correctly applied:

        ```bash
        sudo systemctl restart apache2
        ```
11. **Access the Site**:
    * Open your browser and navigate to your site’s URL (e.g., `http://betriver.io`). Your site should now be live!

***

These instructions should set up Betriver.io properly on your VPS, ensuring both the server and application are ready for production. Let me know if any steps need further clarification!
