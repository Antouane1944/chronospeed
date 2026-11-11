# Delivery Points

PWA statique pour préparer une tournée sur Android.

## Fonctionnalités
- Autocomplétion d'adresses via l'API Géoplateforme IGN.
- Référentiel local d'entreprises récurrentes.
- Sélection des entreprises à ajouter à la tournée du jour.
- Modification des coordonnées GPS et consignes.
- Export CSV de la tournée.
- Export/import JSON du référentiel.
- Sauvegarde locale dans le navigateur et cache de l'application.

## Publication GitHub Pages
1. Crée un dépôt GitHub (par exemple `delivery-points`).
2. Dépose les quatre fichiers (`index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`) à la racine.
3. Dans Settings > Pages, choisis `Deploy from a branch`, branche `main`, dossier `/ (root)`.
4. Ouvre l'URL GitHub Pages sur ton Android avec Chrome.
5. Menu ⋮ > Ajouter à l'écran d'accueil / Installer l'application.

## Important
- Les données restent dans le stockage local du navigateur de ce téléphone.
- Exporte régulièrement `delivery-points-backup.json` pour sauvegarder le référentiel.
- L'autocomplétion nécessite Internet. L'application et les données déjà enregistrées restent consultables hors ligne après un premier chargement.
- L'API d'autocomplétion IGN nécessite une connexion et peut évoluer. Vérifier le format des suggestions sur l'environnement réel lors du premier test.
- Ce prototype n'envoie aucune donnée de livraison vers un serveur.
