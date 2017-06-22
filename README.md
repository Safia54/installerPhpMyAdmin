# Comment installer phpMyAdmin ?
#### Avec soluce de débuggage 



## A quoi sert phpMyAdmin ?
 
phpMyAdmin est un outil en interface qui permet de lire une base de donnée SQL accessible depuis un navigateur en local. 

*ou sinon expliqué plus complètement [ici par la doc Ubuntu](https://doc.ubuntu-fr.org/phpmyadmin)*

## Installation

1. Avant de *vouloir* installer phpMyAdmin, c'est qu'on a déjà installé un serveur de base de données comme MySQL pour le plus connu.
    Si ce n'est pas fait : vous pouvez [suivre les instructions ici](https://github.com/becodeorg/BeCode/wiki/Installer-LAMP-sur-Ubuntu) qui explique comment installer LAMP (**L**inux **A**pache **M**ySQL **P**hp) sur Ubuntu.
    
2. Télécharger le dossier [disponible sur le site officiel de phpMyAdmin](https://www.phpmyadmin.net/)

*OU*

Depuis la ligne de commande du terminal: `sudo wget https://files.phpmyadmin.net/phpMyAdmin/4.7.1/phpMyAdmin-4.7.1-all-languages.zip` 

3. S'assurer que le dossier phpMyAdmin téléchargé se retrouve dans le dossier où sont entreposés vos fichiers de serveur de base de données, et le renommer avec un mom plus court 
> ex : phpmyadmin. 

4. Taper **dans sa ligne de commande du terminal** `mysql -u root -p` afin de configurer l'utilisation de l'interface phpMyAdmin comme utilisateur.

5. Ton terminal te demande le mot de passe de l'utilisateur root. Indique ton mot de passe et retiens-le.

6. Puisque tu as déjà installé un serveur comme dit au point 1., rends-toi **depuis ton navigateur** sur ton localhost, et indique le chemin vers ton dossier phpmyadmin que tu as placé et renommé comme indiqué au point 3. 
> par exemple : localhost/phpmyadmin 

(Attention, lorsque tu as nommé ton dossier avec des majuscules, recopie le nom tel quel dans le chemin du localhost car c'est sensible à la case.)

7. Il te demande ton nom d'utilisateur qui est root et ton mot de passe tel que retenu au point 5.

8. Te voilà sur phpMyAdmin ! Tu peux créer des bases de données, des tableaux et des colonnes plus facilement grâce à cet outil !


## Débuggage d'installation

Pour ceux qui ont des problèmes pour installer phpMyAdmin avec une erreur **mbstring**, voici la soluce depuis le terminal :

`sudo apt-get install libapache2-mod-php7.0`

`sudo apt-get install php7.0-mbstring`

`sudo service apache2 restart`


## Docu officielle

Il est toujours intéressant de se référer à [la documentation en ligne officielle de phpMyAdmin](http://localhost/phpmyadmin/doc/html/index.html).
