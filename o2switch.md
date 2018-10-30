**YARN**

L'hébergeur ne permet pas d'utiliser ou d'installer Yarn, passer par `npm` pour installer des paquets.

**NPM**

Pour rendre la commande disponible : 

1. Dans CPanel, configurer une nouvelle application node
```
Application Root : public_html/../build
Application URL : exemple.com/build
Application startup file : app.js
```

2. Se connecter en SSH et lancer la commande
```
cloudlinux-selector install-modules --json --interpreter nodejs --user username --app-root public_html/../build
```
