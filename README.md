# FileGrab

FileGrab is a sophisticated file-sharing platform that enables the user to upload and disseminate their downloads, thereby providing global accessibility to their valuable resources.

## Installation

>1. Unzip filegrab_1.0.zip
>2. Upload everything in the folder "UPLOAD"
>3. Make /uploads/ writable by PHP (e.g., chmod 755 or 775 depending on server).
>4. Edit /inc/config.php (Example show below) Make sure to have your database information and your Recaptcha V2 Keys.

```php
/INC/CONFIG.PHP Example

// ---- BASIC SITE SETTINGS ----
define('SITE_NAME', 'Your SocialDL'); // Changeable site name
define('COUNTDOWN_SECONDS', 7);       // Modal countdown before like
define('ADMIN_PASSWORD_HASH', password_hash('changeme', PASSWORD_DEFAULT)); // change with password_hash

// ---- DATABASE ----
define('DB_HOST', 'localhost');
define('DB_NAME', 'your_db_name');
define('DB_USER', 'your_db_user');
define('DB_PASS', 'your_db_pass');
define('DB_CHARSET', 'utf8mb4');

// ---- PAGINATION / LAYOUT ----
define('BOXES_PER_ROW', 4);
define('ROWS_PER_PAGE', 10); // 10 rows per batch
define('ITEMS_PER_PAGE', BOXES_PER_ROW * ROWS_PER_PAGE); <-- DO NOT RECOMMEND EDITING THIS PART UNLESS YOU KNOW HOW.

// ---- PATHS ----
define('UPLOAD_DIR', __DIR__ . '/../uploads');    // filesystem path
define('UPLOAD_URL', '/uploads');                  // public URL base


// ---- reCAPTCHA (v2 checkbox) ----
define('RECAPTCHA_SITE_KEY', 'YOUR_RECAPTCHA_SITE_KEY');
define('RECAPTCHA_SECRET_KEY', 'YOUR_RECAPTCHA_SECRET_KEY');
// Theme is set to dark in the contact form

```

## Usage

```python
Visit site: Yoursite.com
Admin area: Yoursite.com/admin/
```

## Admin Dashboard (index.php)

We are aware this page just says "This page is intentionally blank (for now)." and we promise we have plans to give it some really good benefits in the next version for you.

## License

[Attribution-NonCommercial-ShareAlike 4.0 International ](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.en)
