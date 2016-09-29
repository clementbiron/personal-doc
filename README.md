# Personal Doc

###Ressources

####SVG
- [Sprite](https://css-tricks.com/svg-sprites-use-better-icon-fonts/)
- [Safari 8 (iOS & Mac OS) doesn't render injected SVG sprites when defined later, after the actual svg > use tags](https://gist.github.com/rhawbert/05c7a758cb22d2a1ed24)

---

####MARKDOWN
- [Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

---

####INTELLIJ IDEA
- [Use IntelliJ IDEA efficiently](https://vimeo.com/98922030)
- [Using Cygwin's bash terminal in a JetBrains IDE](http://engineroom.teamwork.com/using-cygwins-bash-terminal-in-a-jetbrains-ide/)
- Raccourcis  Windows : 
  - Séléctionner toutes les occurences : ALT + J

---

####BABUN
- Update : babun update
- Instal package : pact packagename

**Ajouter un alias**
- vim ~/.babunrc
- appuyer sur i, éditer le fichier avec l'alias à rajouter, par exemple 
- alias gem='C:/Program\ Files/Ruby/bin/gem'
- appuyer sur echap et taper :wq (enregistrer et quitter l'édition du fichier)
- rafraichir : source ~/.babunrc

---

####SASS
**Pour installer Sass**
- installer ruby [http://rubyinstaller.org/](http://rubyinstaller.org/) 
- ajouter C:\Ruby23-x64\bin aux variables d'environnement
- vérifier ruby : ruby -v
- vérifier gem : gem -v
- installer sass via gem : gem install sass
- vérifier sass : sass -v
- pour Babun ajouter les alias 
  - ruby='C:/Ruby23-x64/bin/ruby'
  - gem='C:/Ruby23-x64/bin/gem'
  - sass='C:/Ruby23-x64/bin/sass'

---

####WORDMOVE
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

---

####WP CLI
**Installation**
  - cd c:
  - composer create-project wp-cli/wp-cli --no-dev
  - ajout de C:\wp-cli\bin au variables d'environnement windows
  - pour Babun ajouter l'alias wp='C:/wp-cli/bin/wp'

**BDD**
- Exporter la base de données et chercher remplacer oldValue / newValue : wp search-replace http://localhost/exemple http://preprod.exemple.com --export=export.sql
- Copier l'export sql sur un serveur distant via ssh : scp /cygdrive/h/www/exemple/export.sql posykrat@posykrat.odns.fr:/home/posykrat/tmp
- Importer l'export sql sur serveur distant:
  - ssh posykrat@posykrat.odns.fr
  - cd ~/public_html/exemple
  - wp db import /home/posykrat/tmp/export.sql
  







