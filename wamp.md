# Wamp

## Configuration
Lire: [http://ordi-genie.com/developpement-php/35-wamp-serveur/81-configuration-de-wamp](http://ordi-genie.com/developpement-php/35-wamp-serveur/81-configuration-de-wamp)

## Erreur MySql
Erreurs lors de l'import MySql incorrect datetime value '0000-00-00 00:00:00'

Dans les configuration de base de MySql la valeur zéro est maintenant interdite dans les dates.Si vous avez des champs date avec des valeurs à zéro, il faut enlever ce contrôle. Dans le fichier de configuration de MySql (C:\wamp64\bin\mysql\mysql.y.z\my.ini pour Wamp 64 bits) Rechercher la variable d'environnement sql-mode et supprimer NO\_ZERO\_DATE et NO\_ZERO\_IN\_DATE

Par exemple (cas standard) , remplacer : sql-mode="STRICT\_ALL\_TABLES,ERROR\_FOR\_DIVISION\_BY\_ZERO,NO\_ZERO\_DATE,NO\_ZERO\_IN\_DATE,NO\_AUTO\_CREATE\_USER" par sql-mode="STRICT\_ALL\_TABLES,ERROR\_FOR\_DIVISION\_BY\_ZERO,NO\_AUTO\_CREATE\_USER"

## Erreur SSL
`Fatal error: Uncaught Exception: SSL certificate problem: unable to get local issuer certificate in...` A lire: [https://stackoverflow.com/questions/28858351/php-ssl-certificate-error-unable-to-get-local-issuer-certificate](https://stackoverflow.com/questions/28858351/php-ssl-certificate-error-unable-to-get-local-issuer-certificate)
