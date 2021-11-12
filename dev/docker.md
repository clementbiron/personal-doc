#### DOCKER
**Installation**
- Pour Windaube suivre : [https://docs.docker.com/docker-for-windows/](https://docs.docker.com/docker-for-windows/)
- Tester 
  - `docker --version`
  - `docker run hello-world`
- Installer kitematic (gui pour les containers)

**Commandes**
- `docker ps` liste les containers qui tourne
- `docker ps -a` liste tous les containers
- stopper tous les containers : docker kill $(docker ps -q)
- Lancer un container lamp :  docker run -t -i -p 80:80 tutum/lamp /bin/bash
- Lancer un container en mappant un repertoire local : docker run -t -i -v h:/monDossier/sur/maMachine:/dossier/dans/leContainer -p 80:80  tutum/lamp /bin/bash
- Commiter des modifs sur un container :  docker commit -m "added composer" 3a9b9953c4e7 dfwp/lamp:v0.1.1
- Construire une image à partir d'un Dockerfile : docker build /path (si dans le dossier mettre .)

**Ressources**
- doc en fr (non officiel) : [https://github.com/xataz/Tutoriels/blob/master/Docker/0.%20Introduction.md](https://github.com/xataz/Tutoriels/blob/master/Docker/0.%20Introduction.md)
