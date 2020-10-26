# o2switch

**YARN**

L'hébergeur ne permet pas d'utiliser ou d'installer Yarn, passer par `npm` pour installer des paquets.

**NPM**

Pour rendre la commande disponible il faut créer une application node dans cPanel

```text
Application Root : public_html/../build
Application URL : exemple.com/build
Application startup file : app.js
```

Se connecter en SSH et lancer la commande

```text
cloudlinux-selector install-modules --json --interpreter nodejs --user username --app-root public_html/../build
```

