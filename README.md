# ANSET Toolbox — versions publiées

Ce dépôt ne contient que les versions publiées d'ANSET Toolbox, l'application d'entretien des PC Windows (diagnostic, sécurité, sauvegardes, maintenance). Le code de travail est dans un dépôt privé.

## Installer sur un nouveau PC

Télécharger **[ANSET-Toolbox-installation.exe](https://github.com/detremerie-stack/anset-toolbox-versions/releases/latest/download/ANSET-Toolbox-installation.exe)** (toujours la dernière version) et double-cliquer. Installation dans le profil de l'utilisateur, sans droits administrateur ; PowerShell 7 est fourni.

Si Windows affiche « Windows a protégé votre ordinateur » : *Informations complémentaires* > *Exécuter quand même*.

## Mises à jour

Les PC équipés se mettent à jour tout seuls : ANSET Toolbox consulte la [dernière version](https://github.com/detremerie-stack/anset-toolbox-versions/releases/latest) à chaque ouverture et une fois par jour, vérifie l'empreinte SHA-256 du paquet, puis l'installe en gardant les rapports et les réglages du PC.

Chaque version contient :

| Fichier | Rôle |
|---|---|
| `version.json` | numéro de version, nouveautés, empreinte SHA-256 du paquet |
| `MaintenancePC-<version>.zip` | paquet de mise à jour (léger, sans PowerShell) |
| `ANSET-Toolbox-installation.exe` | installateur complet pour un nouveau PC |
| `Migration-PC-portable.exe` | assistant de migration d'un PC, sans installation |
