# Git

## Commit
* Commiter et stage files (fichiers modifiés et supprimés uniquement) : `git commit -a -m "mon texte"`

## Tag
* Créer un tag : `git tag -a v1.0.0 -m "lorem"`
* Pusher le tag : `git push origin v1.0.0`
* Connaître le tag en cours : `git describe --tags`

## Branch
* Créer une branche : `git checkout -b maBranche && git push origin maBranche`
* Changer de branche : `git checkout maBranche`
* Merge de branche : `git merge maBrancheAMergerDansCelleCi`
* Supprimer une branche localement : `git branch -d maBranche`
* Supprimer une branche distante : `git push origin --delete maBranche`

## Clone
* Cloner un repo : `git clone https://monrepo nomDuDossierACreer`
* Cloner une branch d'une repo : `git clone -b branch https://monrepo nomDuDossierACreer`
* Cloner le contenu uniquement : `git clone https://monrepo .`

## Pull
* récupérer un tag en particulier : `git pull origin branch:tag`
* forcer un pull : `git fetch --all` et `git reset --hard origin/master`

## Changing a remote's URL
* From SSH to HTTPS : `git remote set-url origin https://github.com/USERNAME/REPOSITORY.git`
* From HTTPS to SSH : `git remote set-url origin git@github.com:USERNAME/REPOSITORY.git`

## Pull a Branch from Another User's Fork
```bash
git remote add some_user git@github.com:some_user/repo_name.git
git fetch some_user
git checkout -b my_name_for_their_branch some_user/their_branch
```

**Modifying an inactive pull request locally**[ **:**https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/checking-out-pull-requests-locally](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/checking-out-pull-requests-locally)

## Change a commit message in git after push
```
git commit --amend -m "New message"
```

**Help my case-sensitive filename changes don't commit :** [https://daily-dev-tips.com/posts/git-basics-help-my-case-sensitive-filename-changes-dont-commit/](https://daily-dev-tips.com/posts/git-basics-help-my-case-sensitive-filename-changes-dont-commit/)

## Error
* LF will be replaced by CLRF" warning in Git on Windows : `git config --global core.safecrlf false`

## Articles
* Comment déployer sur un serveur distant en une commande GIT, pas à pas: [https://medium.com/@stadja/comment-d%C3%A9ployer-sur-un-serveur-distant-en-une-commande-git-pas-%C3%A0-pas-bdcf5aaf172d](https://medium.com/@stadja/comment-d%C3%A9ployer-sur-un-serveur-distant-en-une-commande-git-pas-%C3%A0-pas-bdcf5aaf172d)
* [https://sethrobertson.github.io/GitPostProduction/gpp.html](https://sethrobertson.github.io/GitPostProduction/gpp.html)



## Ressources
* [https://ohshitgit.com/](https://ohshitgit.com/)
* [https://learngitbranching.js.org/](https://learngitbranching.js.org/)
* [https://www.conventionalcommits.org/en/v1.0.0/](https://www.conventionalcommits.org/en/v1.0.0/)
* [https://github.com/girliemac/a-picture-is-worth-a-1000-words/tree/main/git-purr](https://github.com/girliemac/a-picture-is-worth-a-1000-words/tree/main/git-purr)
* [https://ndpsoftware.com/git-cheatsheet.html#loc=index;](https://ndpsoftware.com/git-cheatsheet.html#loc=index;)
