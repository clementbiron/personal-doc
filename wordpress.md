#### WordPress

**Articles**
- How not to be depressed when working with WordPress : https://devops-life.com/blog/2019/04/10/state-of-wordpress-in-2019/

**Template hierarchy**
- https://developer.wordpress.org/files/2014/10/wp-hierarchy.png

**Rest API**
- Client JavaScript : https://www.npmjs.com/package/wpapi

**Wp Query**
- WordPress Query Comprehensive Reference : https://github.com/luetkemj/wp-query-ref

**ACF**
- Extensions : http://awesomeacf.com/
- Image responsive : http://aaronrutley.com/responsive-images-in-wordpress-with-acf/
- Add Sortable ACF Admin Column : https://support.advancedcustomfields.com/forums/topic/add-sortable-acf-admin-column/
- Understanding where your ACF field group settings are coming from : https://awesomeacf.com/understanding-where-your-acf-field-group-settings-are-coming-from/
- Recovery Tool from PHP Export : https://github.com/BeAPI/ACF-PHP-Recovery
- Font Awesome field: https://wordpress.org/plugins/advanced-custom-fields-font-awesome/
 Medium Editor Field (champs TinyMCE configurable) : https://github.com/Hube2/acf-medium-editor
- 8 snippets pour modifier le comportement d’ACF : https://mosaika.fr/astuces-developpement-acf/
- ACF with Timber : https://medium.com/@robertguss/how-to-make-a-custom-wordpress-page-builder-using-advanced-custom-fields-pro-timber-4ef822098dc3
- Créer un Formulaire de Connexion & Inscription en AJAX grâce à ACF Form : https://hwk.fr/blog/acf-creer-un-formulaire-de-connexion-inscription-en-ajax-grace-acf-form
- A tester : 
  - Afficher les champs ACF dans la post table : https://github.com/mcguffin/acf-quick-edit-fields
  - Extensions pour créer des formulaires avec des champs ACF : https://advancedforms.github.io/
  - ACF Columns : https://fr.wordpress.org/plugins/acf-columns/
  - https://github.com/MarieComet/MC-ACF-Flexible-Template/
 - https://github.com/7studio/acf-svg-icon
 - https://github.com/BeAPI/acf-svg-icon
  
**Polylang**
- Auto translate existing media : https://github.com/aucor/polylang-translate-existing-media
- Disable language selector : https://github.com/aucor/polylang-smart-language-select-disabler
  
**RGPD**
- https://wordpress.org/plugins/gdpr/
  
**Internationalization**
- Blank WordPress Pot : https://github.com/fxbenard/Blank-WordPress-Pot
- Poedit translation secrets : https://www.cssigniter.com/wordpress-poedit-translation-secrets/

**Divers**
- WP Backdoor user (devenir admin via upload d'un fichier sur le ftp) : http://boiteaweb.fr/plugin-backdoor-user-3311.html
- Sortable taxonomy columns : http://scribu.net/wordpress/sortable-taxonomy-columns.html
- Liste des emails envoyés par WordPress : https://gist.github.com/johnbillion/0a48021de5510c41d517
- Useful developer tools for working with WordPress : http://wpgear.org/
- Rewrite Rules Inspector https://wordpress.org/plugins/rewrite-rules-inspector/
- Snippets : https://hwk.fr/codes
- A Deep Dive Into WordPress Automatic Updates : https://kinsta.com/blog/wordpress-automatic-updates/
- We strive to make the world's best Premium WordPress Themes & Plugins and WooCommerce Extensions & Themes available for free : https://gpldl.com/search-the-repository/

**Confs**
- WPTech 2018 : https://github.com/yannkozon/wptech-2018

**Gut**
- https://imathi.eu/2018/08/12/tuttogut-01/

**Elementor**
- https://trello.com/b/52NXAeg2/elementor-resources-for-and-by-the-community


---

#### WP CLI
**Installation**
  - cd c:
  - composer create-project wp-cli/wp-cli --no-dev
  - ajout de C:\wp-cli\bin au variables d'environnement windows
  - pour Babun ajouter l'alias wp='C:/wp-cli/bin/wp'

**BDD export / import**
- Exporter la base de données et chercher remplacer oldValue / newValue : wp search-replace http://localhost/exemple http://preprod.exemple.com --export=export.sql
- Copier l'export sql sur un serveur distant via ssh : scp /cygdrive/h/www/exemple/export.sql user@domain.com:/home/posykrat/tmp
- Importer l'export sql sur serveur distant:
  - ssh user@serveur.fr
  - cd ~/public_html/exemple
  - wp db import /home/posykrat/tmp/export.sql

