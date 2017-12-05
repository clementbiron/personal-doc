#### WordPress

**Template hierarchy**
- https://developer.wordpress.org/files/2014/10/wp-hierarchy.png

**Rest API**
- Client JavaScript : https://www.npmjs.com/package/wpapi

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
  
**Internationalization**
- Blank WordPress Pot : https://github.com/fxbenard/Blank-WordPress-Pot

**Divers**
- WP Backdoor user (devenir admin via upload d'un fichier sur le ftp) : http://boiteaweb.fr/plugin-backdoor-user-3311.html
- Sortable taxonomy columns : http://scribu.net/wordpress/sortable-taxonomy-columns.html
- Liste des emails envoyés par WordPress : https://gist.github.com/johnbillion/0a48021de5510c41d517
- Useful developer tools for working with WordPress : http://wpgear.org/

---

#### WP CLI
**Installation**
  - cd c:
  - composer create-project wp-cli/wp-cli --no-dev
  - ajout de C:\wp-cli\bin au variables d'environnement windows
  - pour Babun ajouter l'alias wp='C:/wp-cli/bin/wp'

**BDD export / import**
- Exporter la base de données et chercher remplacer oldValue / newValue : wp search-replace http://localhost/exemple http://preprod.exemple.com --export=export.sql
- Copier l'export sql sur un serveur distant via ssh : scp /cygdrive/h/www/exemple/export.sql posykrat@posykrat.odns.fr:/home/posykrat/tmp
- Importer l'export sql sur serveur distant:
  - ssh user@serveur.fr
  - cd ~/public_html/exemple
  - wp db import /home/posykrat/tmp/export.sql

