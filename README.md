# WordPress mirrors without uploads directory

Sometimes duplicating a site over to a development mirror just to test a few changes, run some updates, or debug a plugin conflict etc can be quite cumbersome, especially on older more established sites with huge uploads directories.

Sometimes its just simply not practical to copy a clients entire uploads directory to a mirror location.

This is simple .htaccess snippet to help set up your mirror without the uploads directory.
All requests to the mirrors wp-content/uploads directory will be redirected to the live version IF the file doesn't already exist on the mirrored site.
