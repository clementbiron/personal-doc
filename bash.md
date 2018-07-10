#### BASH

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

**Ressources**
- La bash bible : https://github.com/dylanaraps/pure-bash-bible
