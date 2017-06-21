# Installer PhpMyAdmin
## Avec soluce de debuggage 



### A quoi sert phpMyAdmin ?
 
 phpMyAdmin est une interface d'administration pour le SGBD MySQL. Il est écrit en langage PHP et s'appuie sur le serveur HTTP Apache.

Il permet d'administrer les éléments suivants :
*les bases de données
*les tables et leurs champs (ajout, suppression, définition du type)
*les index, les clés primaires et étrangères
*les utilisateurs de la base et leurs permissions
*exporter les données dans divers formats (CSV, XML, PDF, OpenDocument, Word, Excel et LaTeX)

### Installation

1. Avant de *vouloir* installer phpMyAdmin, c'est qu'on a déjà installé un serveur de base de données comme MySQL pour le plus connu.
    Si ce n'est pas fait : vous pouvez [suivre les instructions ici](https://github.com/becodeorg/BeCode/wiki/Installer-LAMP-sur-Ubuntu) qui explique comment installer LAMP (**L**inux **A**pache **M**ySQL **P**hp) sur Ubuntu.
    
2. Télécharger le dossier [disponible sur le site officiel de phpMyAdmin](https://www.phpmyadmin.net/)
*OU*
Depuis la ligne de commande : `sudo apt-get install https://files.phpmyadmin.net/phpMyAdmin/4.7.1/phpMyAdmin-4.7.1-all-languages.zip` 

3. S'assurer que le dossier phpMyAdmin téléchargé se retrouve dans le dossier où sont entreposés vos fichiers de serveur de base de données.

4. 

### Débuggages d'installation

Pour ceux qui ont des problèmes pour installer phpMyAdmin avec une erreur **mbstring**, 

voici la soluce:
    `sudo apt-get install libapache2-mod-php7.0`
    `sudo apt-get install php7.0-mbstring`
    `sudo service apache2 restart`


### Toujours se référer à la docu officielle

Il est toujours intéressant de se référer à [la documentation en ligne officielle de phpMyAdmin](http://localhost/phpmyadmin/doc/html/index.html).
