### Installing WordPress on Ubuntu

[Ubuntu WordPress Install](https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-with-lamp-on-ubuntu-18-04){:target="_blank"}

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
