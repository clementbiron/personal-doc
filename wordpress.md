#### WordPress

**Rest API**
- Client JavaScript : https://www.npmjs.com/package/wpapi

**Template hierarchy**
- https://developer.wordpress.org/files/2014/10/wp-hierarchy.png

**ACF**
- Extensions : http://awesomeacf.com/
- Image responsive : http://aaronrutley.com/responsive-images-in-wordpress-with-acf/
- A tester : 
  - Medium Editor Field (champs TinyMCE configurable) : https://github.com/Hube2/acf-medium-editor
  - Afficher les champs ACF dans la post table : https://github.com/mcguffin/acf-quick-edit-fields

**Divers**
- WP Backdoor user (devenir admin via upload d'un fichier sur le ftp) : http://boiteaweb.fr/plugin-backdoor-user-3311.html
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
