---
description: >-
  Betriver maintains a strict standard Laravel  folder structure. This makes it
  easy for any laravel developer to customize, update or modify the software.
---

# Cpanel/Plesk installation

### Directory Structure

* **Pre Built CSS Files:** `/../public/assets/css`
* **Source code CSS Files:** `/../resources/css`
* **Source code Js Files**`/../resources/js`
* **Pre Built JavaScript Files:** `/../public/assets/js`
* **Pre Built Fonts, images, components:** `/../public/assets/`

&#x20;All Dependencies and  assets have been installed  built and exported, unless you need to make changes to the source code, you don’t have to install or update anything.\
[**Learn more about Laravel**](https://laravel.com/docs/)

### 1. Create a Database

Create a fresh database, choose `utf8mb4_general_ci` character encoding and add a user to the database, then grant this user all permissions to that database. Note the **database name**, **username**, and **password**.  It will be needed during installation

### 2. Unzip and upload server files

Extract the file you downloaded. In the extracted directory find **betriver-server.zip,** upload this to the root folder of your domain. Extract the contents of **betriver-server.zip** here.

### 3. **Change Your Document Root**

* Go back to cPanel main page
* Look for "Domain" or "Domains" section
* Click on "Domains" or "Domain Manager"
* Find your domain and click "Manage" or the gear/settings icon
* Look for "Document Root" or "Directory"
* Add `/public` to the end of your current path
* Example: If current path is `/home/username/public_html`, change it to `/home/username/public_html/public`
* Save changes

**Alternative Method** (if above option isn't available):

* Contact your hosting provider
* Ask them to change the document root to point to the `/public` folder inside the uploaded files.

**Important Notes:**

* This change may take a few minutes to take effect
* Make sure all your Betriver files are properly uploaded before making this change
* If your site shows errors, double-check the path is correct

### 3. Run the installer.

Visit your site in the browser. The installer should load. &#x20;

Follow the instructions on the screen.

<figure><img src="../../.gitbook/assets/Screenshot 2024-11-06 at 10.19.08 PM.png" alt="Betn installerr welcome screen" width="563"><figcaption><p>Installer Step 1</p></figcaption></figure>

#### The installer will check if your system meets some minimum requirements 

<figure><img src="../../.gitbook/assets/Screenshot 2024-11-06 at 10.19.26 PM.png" alt="Betn System Requirements" width="563"><figcaption><p>System Requirements</p></figcaption></figure>

#### If all is fine, the installer will verify if your folder permissions are fine. Ensure that storage  and cache are writeable before proceeding.

<figure><img src="../../.gitbook/assets/Screenshot 2024-11-06 at 10.19.36 PM.png" alt="Betn folder permissions setup" width="563"><figcaption><p>Folder permissions</p></figcaption></figure>

#### Next the installer will require your Database settings. 

<figure><img src="../../.gitbook/assets/Screenshot 2024-11-06 at 10.20.24 PM.png" alt="" width="563"><figcaption></figcaption></figure>

Here are some common settings for MySQL.\


```properties
MySQL
Database_HOST=localhost
Database_PORT=3306
```



#### Once You configure database. The site should be ready to go.

<figure><img src="../../.gitbook/assets/Screenshot 2024-11-07 at 3.31.55 AM.png" alt="" width="563"><figcaption></figcaption></figure>

Start and wait for migrations. (there are no SQL files)\


<figure><img src="../../.gitbook/assets/Screenshot 2024-11-07 at 3.31.16 AM.png" alt="" width="563"><figcaption></figcaption></figure>

#### Finally Click Complete installation, to update final configurations.

<figure><img src="../../.gitbook/assets/Screenshot 2024-11-07 at 3.31.43 AM.png" alt="" width="563"><figcaption></figcaption></figure>
