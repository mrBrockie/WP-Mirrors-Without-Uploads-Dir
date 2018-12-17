# WordPress mirrors without uploads directory

A simple .htaccess snippet for setting up a wordpress mirror without having to duplicate the entire uploads directory


RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule ^wp-content/uploads/(.*)$ https://livedomain.com/wp-content/uploads/$1 [L,R=301]
