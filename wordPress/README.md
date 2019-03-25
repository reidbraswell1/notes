### Installing WordPress on Ubuntu

* Move the wordpress folder to /var/www after installing apache2

[Ubuntu WordPress Install](https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-with-lamp-on-ubuntu-18-04)

[Ubuntu WordPress Install](https://www.tecmint.com/install-wordpress-on-ubuntu-16-04-with-lamp)

[WordPress Directory Structure](https://www.wpbeginner.com/beginners-guide/beginners-guide-to-wordpress-file-and-directory-structure/)

##### Restarting Apache 2
```bash
sudo service apache2 restart
# or 
sudo systemctl restart apache2
```

#### To display php scripts from a user directory
* Edit your current version of php config file example: 
```bash
# php7.2 is installed but your version might be different
sudo nano /etc/apache2/mods-available/php7.2.conf
```
#### Display from public_html in user directory
* Default Apache Root Directory
```bash
/var/www
```
* Create a public_html directory inside of the user's home directory and give it 755 permissions.
```bash
chmod 755 $HOME/public_html
```
* Point the browser to localhost/~username/
* Copy the wordpress config file wp-config-sample.php to wp-config.php
```bash
  cp wp-config-sample.php wp-config.php
```  
* .htaccess file - used  by Apache Server
* WordPress setup url 
```url
  http://localhost/wp-admin/setup-config.php
```  
* Error message
```code
  Your PHP installation appears to be missing the MySQL extension which is required by WordPress.
```  
