## Avant d'installer Calagopus

**Ce package installe uniquement le panneau Calagopus.**

Pour héberger des serveurs de jeux, vous devrez également installer **Wings** sur au moins un hôte Linux après la configuration du panneau. Wings est le démon qui exécute et gère les conteneurs de serveurs de jeux. Les instructions d'installation sont disponibles dans la [documentation Calagopus](https://calagopus.com/docs/wings/installation).

**Prérequis :**
- Un domaine ou sous-domaine dédié est recommandé (ex. `panel.votredomaine.tld`)
- Au moins **512 Mo de RAM** disponibles à l'exécution (1 Go recommandé)
- Au moins **1 Go d'espace disque libre**
- Architecture : **amd64** ou **arm64** uniquement

**Important :** La clé `APP_ENCRYPTION_KEY` générée lors de l'installation est utilisée pour protéger les données sensibles stockées en base de données. **Ne perdez pas cette clé** — elle ne peut pas être récupérée et la faire tourner nécessite de re-chiffrer tous les secrets stockés.
