# Bash

## Manipulation de fichiers / dossiers
* Créer un dossier : `mkdir`
* Créer un fichier : `touch`
* Supprimer un dossier et fichiers (récursif) : `rm -r monDossier`
* Lister le poids des dossiers : `du -sh ./*`

## SSH
* Génération de clés : `dssh-keygen -t rsa`
* Envoyer la clé publique sur le serveur : `dcat ~/.ssh/id_rsa.pub | ssh user@domain "cat >> ~/.ssh/authorized_keys"`
* Si erreur WARNING: UNPROTECTED PRIVATE KEY FILE! &#x20;
  * sudo chmod 600 \~/.ssh/id\_rs
  * sudo chmod 600 \~/.ssh/id\_rs.pub
  * sudo chmod 755 \~/.ssh

## Ressources
* La bash bible: [https://github.com/dylanaraps/pure-bash-bible](https://github.com/dylanaraps/pure-bash-bible)



