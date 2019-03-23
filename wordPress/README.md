### Installing WordPress on Ubuntu

##### Restarting Apache 2
```bash
sudo service apache2 restart
# or 
sudo systemctl restart apache2
```

chmod 755 $HOME/public_html
<br>
default Apache uses /var/www as document root
<br>
#### Display from public_html in user directory
* Point the browser to localhost/~username/
