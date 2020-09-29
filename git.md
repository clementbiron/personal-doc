#### GIT
**Commit**
- Commiter et stage files (fichiers modifiés et supprimés uniquement) : `git commit -a -m "mon texte"`

**Tag**
- Créer un tag : `git tag -a v1.0.0 -m "lorem"`
- Pusher le tag : `git push origin v1.0.0`
- Connaître le tag en cours : `git describe --tags`

**Branch**
- Créer une branche : `git checkout -b maBranche && git push origin maBranche`
- Changer de branche : `git checkout maBranche`
- Merge de branche : `git merge maBrancheAMergerDansCelleCi`

**Clone**
- Cloner un repo : `git clone https://monrepo nomDuDossierACreer`
- Cloner une branch d'une repo : `git clone -b branch https://monrepo nomDuDossierACreer`
- Cloner le contenu uniquement : `git clone https://monrepo .`

**Pull**
- récupérer un tag en particulier : `git pull origin branch:tag`
- forcer un pull : `git fetch --all` et `git reset --hard origin/master`

**Changing a remote's URL**
- From SSH to HTTPS : `git remote set-url origin https://github.com/USERNAME/REPOSITORY.git`
- From HTTPS to SSH : `git remote set-url origin git@github.com:USERNAME/REPOSITORY.git`

**Error**
- LF will be replaced by CLRF" warning in Git on Windows : `git config --global core.safecrlf false`

**Articles**
- Comment déployer sur un serveur distant en une commande GIT, pas à pas : https://medium.com/@stadja/comment-d%C3%A9ployer-sur-un-serveur-distant-en-une-commande-git-pas-%C3%A0-pas-bdcf5aaf172d
