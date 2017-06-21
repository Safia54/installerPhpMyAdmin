# installerPhpMyAdmin
## Avec soluce de debuggage 

1. A quoi sert phpMyAdmin ?
 
 phpMyAdmin est une interface d'administration pour le SGBD MySQL. Il est écrit en langage PHP et s'appuie sur le serveur HTTP Apache.

Il permet d'administrer les éléments suivants :

    les bases de données
    les tables et leurs champs (ajout, suppression, définition du type)
    les index, les clés primaires et étrangères
    les utilisateurs de la base et leurs permissions
    exporter les données dans divers formats (CSV, XML, PDF, OpenDocument, Word, Excel et LaTeX)


2. débuggages 

Pour ceux qui avaient des problèmes pour installer phpMyAdmin avec une erreur **mbstring**, 

voici la soluce:
    `sudo apt-get install libapache2-mod-php7.0`
    `sudo apt-get install php7.0-mbstring`
    `sudo service apache2 restart`

3. Voir docu officielle

Il est toujours intéressant de se référer à [la documentation en ligne officielle de phpMyAdmin](http://localhost/phpmyadmin/doc/html/index.html).
