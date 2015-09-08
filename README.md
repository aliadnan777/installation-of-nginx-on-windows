# installation-on-windows

### new theme on wordpress
* download theme or plugin which you want to use
* move on appearence then on theme
* click on add new 
* select your theme
* last thing activate it

* thats all your theme is ready to use

### nginx installation

* download stable version of nginx

* open the console of window and run following commands
* `unzip nginx-1.8.0.zip`
* `start nginx`

* thats all
* if you want to stop reload reopen or quit nginx
* then follow these commands

* `nginx -s stop`
* `nginx -s reopen`
* `nginx -s reload`
* `nginx -s quit`



### wordpress installation
* for installing wordpress on windows 
* first you need to install wamp or xampp on your windows
* just download the stable version of wamp or xampp and install

* after the installation of xampp open its control panel
* and star apachi server and mysql
* if apachi give error of ports
* then signout from skype , free the port 80 and tryagain

* write in your browser localhost/phpmyadmin
* it will move you to the mysql main page for making database
now

* download the stable version of wordpress for windows
* for working with xampp you need to unzip word press in xampp folder

* C:/Program Files/XAMPP/htdocs.
* unzip the folder and name it what ever you like but same name which you write in database
* Open your WordPress folder, find the wp-config-sample.php file and rename it wp-config.php.
now open this file and edit database name, user name and password field blank and saved it

* Open your browser and go to http://localhost/name of folder/

* you will see the welcome screen of wordpress
* Enter your details and click “Install WordPress.”

* Your WordPress installation is now complete!

### setting multisite on wordpress

* Having Multisite setup on a local machine provides a great way to test themes and plugins in a Multisite environment, 
* but also makes it a quick and easy to have multiple sites running at once.

* Open your wp-config.php file again and 
* add/edit the following lines to activate Multisite’s installation mode

* define('WP_DEBUG',TRUE);

* define('WP_ALLOW_MULTISITE',TRUE);
* Open XAMPP and ensure your Apache and MySQL servers are running.

* Login to your localhost site in your browser and under “Tools” you will now have a new option, “Network Setup.”
* Enter a name for your network and your email address, then click “Install.”

* WordPress will prompt you to edit your wp-config.php and .htaccess files.
* edit WP-config.php file as under
* define('WP_DEBUG',true);
* define('WP_ALLOW_MULTISITE',true);
* define('MULTISITE',true);
* define('SUBDOMAIN_INSTALL',false);
* define('WP_ALLOW_MULTISITE',true);
* define('DOMAIN_CURRENT_SITE','localhost');
* define('PATH_CURRENT_SITE','/');
* define('SITE_ID,CURRENT_SITE',1);
* define('BLOG_ID, CURRENT_SITE',1);

* EDIT .htaccess file
* http://premium.wpmudev.org/blog/wp-content/uploads/2014/06/htaccess-edit.jpg

* Multisite should now be enabled and working on your WordPress site!
