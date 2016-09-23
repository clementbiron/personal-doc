# Personal Doc

###Ressources

####SVG
- [Sprite](https://css-tricks.com/svg-sprites-use-better-icon-fonts/)
- [Safari 8 (iOS & Mac OS) doesn't render injected SVG sprites when defined later, after the actual svg > use tags](https://gist.github.com/rhawbert/05c7a758cb22d2a1ed24)

####Markdown
- [Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

####IntelliJ IDEA
- [Use IntelliJ IDEA efficiently](https://vimeo.com/98922030)
- [Using Cygwin's bash terminal in a JetBrains IDE](http://engineroom.teamwork.com/using-cygwins-bash-terminal-in-a-jetbrains-ide/)
- Raccourcis  Windows : 
  - Séléctionner toutes les occurences : ALT + J

####Babun
Update : babun update
Instal package : pact packagename

####Cygwin
**Pour installer Sass**
- installer ruby [http://rubyinstaller.org/](http://rubyinstaller.org/) en l'ajoutant au PATH
- vérifier ruby : ruby -v
- vérifier gem : gem -v
- installer sass via gem : gem install sass
- vérifier sass : sass -v

Si erreur suivante : C:\Ruby22-x64\bin\ruby.exe: No such file or directory -- /cygdrive/c/Ruby22-x64/bin/gem (LoadError)
- vim ~/.babunrc
- appuyer sur i, éditer le fichier avec les alias ci dessous
- alias gem='C:/Program\ Files/Ruby/bin/gem'
- alias sass='C:/Program\ Files/Ruby/bin/sass'
- appuyer sur echap et taper :wq (enregistrer et quitter l'édition du fichier)
- rafraichir : source ~/.babunrc

####WordMove
- Installer WordMove (nécessite ruby + gem) : gem install wordmove (si erreur suivante  C:\Ruby22-x64\bin\ruby.exe: No such file or directory... voir le paragraphe sur Cygwin pour ajouter l'alias)

**Etapes avec PowerShell**
- Installer choco (besoin d'un gestionnaire de paquet) : iwr https://chocolatey.org/install.ps1 -UseBasicParsing | iex  (voir [https://chocolatey.org/install](https://chocolatey.org/install))
- Installer lftp : choco install lftp

**Avec Babun**
On utilise le gestionnaire de paquet pact
- Installer lftp : pact install lftp


Si erreur suivante: find: Fatal error: Certificate verification: subjectAltName does not match 
lftp > set ssl:verify-certificate no






