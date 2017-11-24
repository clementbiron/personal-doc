#### WordPress

**Rest API**
- Client JavaScript : https://www.npmjs.com/package/wpapi

**Template hierarchy**
- https://developer.wordpress.org/files/2014/10/wp-hierarchy.png

**ACF**
- Extensions : http://awesomeacf.com/
- Image responsive : http://aaronrutley.com/responsive-images-in-wordpress-with-acf/
- Add Sortable ACF Admin Column : https://support.advancedcustomfields.com/forums/topic/add-sortable-acf-admin-column/
- Understanding where your ACF field group settings are coming from : https://awesomeacf.com/understanding-where-your-acf-field-group-settings-are-coming-from/
- Recovery Tool from PHP Export : https://github.com/BeAPI/ACF-PHP-Recovery
- A tester : 
  - Medium Editor Field (champs TinyMCE configurable) : https://github.com/Hube2/acf-medium-editor
  - Afficher les champs ACF dans la post table : https://github.com/mcguffin/acf-quick-edit-fields
  - Extensions pour créer des formulaires avec des champs ACF : https://advancedforms.github.io/

**Divers**
- WP Backdoor user (devenir admin via upload d'un fichier sur le ftp) : http://boiteaweb.fr/plugin-backdoor-user-3311.html
- Sortable taxonomu columns : http://scribu.net/wordpress/sortable-taxonomy-columns.html

---

#### WP CLI
**Installation**
  - cd c:
  - composer create-project wp-cli/wp-cli --no-dev
  - ajout de C:\wp-cli\bin au variables d'environnement windows
  - pour Babun ajouter l'alias wp='C:/wp-cli/bin/wp'

**BDD**
- Exporter la base de données et chercher remplacer oldValue / newValue : wp search-replace http://localhost/exemple http://preprod.exemple.com --export=export.sql
- Copier l'export sql sur un serveur distant via ssh : scp /cygdrive/h/www/exemple/export.sql posykrat@posykrat.odns.fr:/home/posykrat/tmp
- Importer l'export sql sur serveur distant:
  - ssh user@serveur.fr
  - cd ~/public_html/exemple
  - wp db import /home/posykrat/tmp/export.sql
  
  ---
  
 #### WORDMOVE
**Installation pour Babun**
- gem install wordmove 
- pour Babun ajouter les alias 
  - wordmove='C:/Ruby23-x64/bin/wordmove'
  - mysqldump='C:/wamp/bin/mysql/mysql5.6.17/bin/mysqldump'
  - mysql='C:/wamp/bin/mysql/mysql5.6.17/bin/mysql'
- Installer lftp : pact install lftp
- Si erreur suivante: find: Fatal error: Certificate verification: subjectAltName does not match :
- mkdir ~/.lftp
- vim ~/.lftp
- appuyer sur i, éditer le fichier
- set ssl:verify-certificate no
- appuyer sur echap et taper :wq

**Installation pour Powershell**
- Installer choco (besoin d'un gestionnaire de paquet) : iwr https://chocolatey.org/install.ps1 -UseBasicParsing | iex
(voir [https://chocolatey.org/install](https://chocolatey.org/install))
- Installer lftp : choco install lftp
- Ajouter mysql aux variables d'environnement windows : C:\wamp\bin\mysql\mysql5.6.17\bin

