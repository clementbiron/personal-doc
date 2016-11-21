# Personal Doc

* [SVG](svg.md)
* [Markdown](markdown.md)


---

####Composer
- Générer l'autoloader :  composer dump-autoload

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
  
---

####DOCKER
**Installation**
- Pour Windaube suivre : [https://docs.docker.com/docker-for-windows/](https://docs.docker.com/docker-for-windows/)
- Tester 
  - docker --version
  - docker run hello-world
- Installer kitematic (gui pour les containers)

**Commandes**
- docker ps :  liste les containers qui tourne
- docker ps -a : liste tous les containers
- stopper tous les containers : docker kill $(docker ps -q)
- Lancer un container lamp :  docker run -t -i -p 80:80 tutum/lamp /bin/bash
- Lancer un container en mappant un repertoire local : docker run -t -i -v h:/monDossier/sur/maMachine:/dossier/dans/leContainer -p 80:80  tutum/lamp /bin/bash
- Commiter des modifs sur un container :  docker commit -m "added composer" 3a9b9953c4e7 dfwp/lamp:v0.1.1
- Construire une image à partir d'un Dockerfile : docker build /path (si dans le dossier mettre .)

**Ressources**
- doc en fr (non officiel) : [https://github.com/xataz/Tutoriels/blob/master/Docker/0.%20Introduction.md](https://github.com/xataz/Tutoriels/blob/master/Docker/0.%20Introduction.md)

---

####GIT
**Commit**
- Commiter et stage files (fichiers modifiés et supprimés uniquement) : commit -a -m "mon texte"

**Tag**
- Créer un tag : git tag -a v1.0.0 -m "lorem"
- Pusher le tag : git push origin v1.0.0

**Branch**
- Créer une branche : git checkout -b maBranche && git push origin maBranche
- Changer de branche : git checkout maBranche
- Merge de branche : git merge maBrancheAMergerDansCelleCi

**Clone**
- Cloner un repo : git clone https://monrepo nomDuDossierACreer

---

####BASH

**Manipulation de fichiers / dossiers**
- Créer un dossier : mkdir
- Créer un fichier : touch
- Supprimer un dossier et fichiers (récursif) : rm -r monDossier

**SSH**
- Génération de clés : ssh-keygen -t rsa
- Envoyer la clé publique sur le serveur : cat ~/.ssh/id_rsa.pub | ssh user@domain "cat >> ~/.ssh/authorized_keys"
- Si erreur WARNING: UNPROTECTED PRIVATE KEY FILE!  
  - sudo chmod 600 ~/.ssh/id_rs
  - sudo chmod 600 ~/.ssh/id_rs.pub
  - sudo chmod 755 ~/.ssh







