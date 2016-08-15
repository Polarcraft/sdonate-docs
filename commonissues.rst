Common Errors
==================

My package doesn't show up in my store even though it's enabled!
-----------------------------------------------------------------------
Make sure your package has at least one command added, then make sure that command has your server enabled. A package won't show up for a server if it has no commands enabled for that server.

PayPal Error 10002 - Security header is not valid
---------------------------------------------------------------
Your PayPal API credentials are incorrect, follow the instructions in :doc:`configuration/paypal` again.

I've enabled Maintenance mode and now I can't disable it!
--------------------------------------------------------------------
Go to http://yourdomain.com/folder/login.php, or if you are using the one-click hosting and setup this will be at https://sdonate.com/stores/<yourdomain>/login.php. When you have logged in, go to http://yourdomain.com/folder/dashboard.php (https://sdonate.com/stores/<yourdomain>/login.php if using free SDonate hosting).

https:// wrapper is disabled in the server configuration by allow_url_fopen=0
--------------------------------------------------------------------
This issue is caused by the php configuration setting "allow_url_fopen" being set to zero. To fix this simply go into the nginx sites configuration file and put "fastcgi_param PHP_VALUE allow_url_fopen=1" underneath the php location.
