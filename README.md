# installerPhpMyAdmin
## Avec soluce de debuggage 

1. intro: à quoi sert phpMyAdmin ?
Il est toujours intéressant de se référer à [la documentation en ligne officielle de phpMyAdmin](http://localhost/phpmyadmin/doc/html/index.html).

X. débuggages 
Pour ceux qui avaient des problèmes pour installer phpMyAdmin avec une erreur **mbstring**, 
voici la soluce:
    `sudo apt-get install libapache2-mod-php7.0`
    `sudo apt-get install php7.0-mbstring`
    `sudo service apache2 restart`
