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
