# db-backup-ci

Sauvegarde planifiée d'une base Postgres vers un stockage objet privé, chiffrée.

⚠️ Ce dépôt ne contient **que** le workflow d'automatisation (la « recette »).
**Aucune donnée, aucun secret** :

- les sauvegardes chiffrées sont déposées dans un **bucket privé** (jamais ici) ;
- tous les identifiants vivent dans les **GitHub Secrets** du dépôt, jamais dans le code ;
- les sauvegardes sont **chiffrées** : illisibles sans la clé privée, détenue hors ligne.

Le dépôt est public uniquement pour bénéficier des minutes GitHub Actions gratuites
et illimitées ; cela n'expose rien de sensible.
