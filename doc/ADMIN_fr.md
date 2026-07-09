# Instructions post-installation

Calagopus est désormais disponible à l'adresse `https://__DOMAIN____PATH__`.

## Première configuration

Ouvrez l'URL ci-dessus dans votre navigateur. L'assistant **OOBE** (Out-Of-Box Experience) vous guide pour :

1. Créer le premier compte administrateur.
2. Configurer les paramètres globaux (SMTP, apparence, etc.).
3. Ajouter votre premier nœud Wings pour héberger des serveurs de jeux.

## Ajouter un nœud Wings

Calagopus nécessite au moins un démon **Wings** sur un hôte Linux pour lancer effectivement des serveurs de jeux. Le panneau gère uniquement la configuration — c'est Wings qui exécute les conteneurs.

Installez Wings en suivant la [documentation officielle de Wings](https://calagopus.com/docs/wings/installation).

## Fichier d'environnement

La configuration du panneau se trouve dans `/etc/calagopus/.env`.  
**Ne l'éditez pas manuellement** — YunoHost l'écrasera lors de la prochaine mise à jour.

## Journaux

Les journaux applicatifs sont écrits dans `/var/log/__APP__/__APP__.log` et sont automatiquement archivés par logrotate.
