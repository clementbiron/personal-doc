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
####POWERSHELL
**Pour installer Wp-cli**
- suivre les infos ici : [Installing on Windows](https://wp-cli.org/docs/installing/#installing-on-windows)

**Pour installer WordMove**
- Installer choco (besoin d'un gestionnaire de paquet) : iwr https://chocolatey.org/install.ps1 -UseBasicParsing | iex
(voir [https://chocolatey.org/install](https://chocolatey.org/install))
- Installer lftp : choco install lftp
- Ajouter mysql aux variables d'environnement windows : C:\wamp\bin\mysql\mysql5.6.17\bin
---
####BABUN
- Update : babun update
- Instal package : pact packagename
---
####CYGWIN
**Ajouter un alias**
- vim ~/.babunrc
- appuyer sur i, éditer le fichier avec l'alias à rajouter, par exemple 
- alias gem='C:/Program\ Files/Ruby/bin/gem'
- appuyer sur echap et taper :wq (enregistrer et quitter l'édition du fichier)
- rafraichir : source ~/.babunrc

**Pour installer Wp-cli**
- télécharger dans C:/wp-cli le wp-cli.phar sur le site officiel
- ajouter l'alias suivant : alias wp='php C:/wp-cli/wp-cli.phar'

**Pour installer Sass**
- installer ruby [http://rubyinstaller.org/](http://rubyinstaller.org/) en l'ajoutant au PATH
- vérifier ruby : ruby -v
- vérifier gem : gem -v
- installer sass via gem : gem install sass
- vérifier sass : sass -v
- Si erreur suivante : C:\Ruby22-x64\bin\ruby.exe: No such file or directory -- /cygdrive/c/Ruby22-x64/bin/gem (LoadError) : rajouter l'alias.

**Pour installer Wordmove**
Installer WordMove (nécessite ruby + gem) : 
- gem install wordmove 
- Si erreur suivante  C:\Ruby22-x64\bin\ruby.exe: No such file or directory : rajouter l'alias
- Installer lftp : pact install lftp
- Ajouter un alias mysqldump à Babun : alias mysqldump='C:/wamp/bin/mysql/mysql5.6.17/bin/mysqldump'
- Si erreur suivante: find: Fatal error: Certificate verification: subjectAltName does not match :
- mkdir ~/.lftp
- vim ~/.lftp
- appuyer sur i, éditer le fichier
- set ssl:verify-certificate no
- appuyer sur echap et taper :wq







