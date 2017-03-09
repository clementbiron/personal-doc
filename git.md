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
- Cloner une branch d'une repo : git clone -b branch https://monrepo nomDuDossierACreer

**Error**
- LF will be replaced by CLRF" warning in Git on Windows : git config --global core.safecrlf false
