# KARTSET – V16 (PWA Android / GitHub Pages)

Application statique KARTSET, basée sur la V15 bleu/jaune et conservant ses fonctions et fiches locales.

## Structure à déposer à la racine du dépôt GitHub

- `index.html` : application
- `manifest.webmanifest` : identité et installation PWA
- `sw.js` : cache hors-ligne versionné
- `icons/icon-192.png` et `icons/icon-512.png` : icônes d'installation
- `icons/favicon.svg` : favicon
- `.nojekyll` : désactive le traitement Jekyll

Ne pas déplacer ces fichiers ni supprimer le dossier `icons`. Les chemins sont relatifs et compatibles avec une publication GitHub Pages dans un sous-dossier, par exemple `/Otk-exentric-setup/`.

## Publication

Déposer tous les éléments de cette archive à la racine du dépôt, en conservant le dossier `icons`, puis publier depuis `main` / root dans Settings → Pages. Attendre la fin du déploiement.

## Android

Ouvrir l'URL GitHub Pages dans Chrome. Si une ancienne version a déjà été visitée, fermer les onglets du site, puis recharger après publication. Le service worker utilise le cache `kartset-v16` et supprime les anciens caches KARTSET à son activation.

Les fiches restent stockées localement dans le navigateur/appareil ; elles ne sont pas synchronisées automatiquement. Exporter régulièrement une sauvegarde JSON.
