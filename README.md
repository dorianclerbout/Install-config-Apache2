# Install config Apache2 server

- [1 - Install Apache2  ](#1---Install-Apache2) 
- [2 - Create file php.info ](#2---Create-file-php.info)
- [3 - Launch, Reload, and Stop apache2 ](#3---Launch-Reload-and-Stop-apache2)




## 1.  Install Apache2 server

- Inside terminal :

        sudo apt-get install apache2

- Let's check the install version :

        sudo apache2ctl -v

- to test the configuration

        sudo apache2ctl -t



- delete index.html :
>   go to /var/www/html/

        rm index.html

## 2. Create file php.info

>in the html folder var/www/html/ create file php.info

    touch php.info

- Inside php.info paste : 

        <?php
        phpinfo();
        ?>

> to see the result, go to the browser and search in the url

    localhost or 127.0.0.1

> you can now deposit your projects in var/www/html/

## 3. Launch, Reload, and Stop apache2

- For launch apache2 :

        sudo systemctl start apache2

- For reload :

        sudo systemctl reload apache2

- For close : 

        sudo systemctl stop apache2