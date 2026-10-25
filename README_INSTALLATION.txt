# BPU Explorer — installation PWA et GitHub Pages

## Contenu
- `index.html` : application et données du BPU intégrées.
- `manifest.webmanifest` : nom, icônes et paramètres d'installation.
- `sw.js` : mise en cache pour pouvoir rouvrir l'application hors connexion après le premier chargement.
- `icons/` : icônes de l'application.

## Publier sur GitHub Pages
1. Connecte-toi à GitHub et crée un dépôt, par exemple `bpu-explorer`.
2. Dans le dépôt, choisis **Add file > Upload files**.
3. Décompresse ce ZIP sur ton ordinateur puis téléverse **le contenu** du dossier `BPU_Explorer_PWA` (il faut que `index.html`, `manifest.webmanifest`, `sw.js` et `icons/` soient à la racine du dépôt, pas dans un sous-dossier).
4. Clique sur **Commit changes**.
5. Ouvre **Settings > Pages**. Sous **Build and deployment**, choisis **Deploy from a branch**, puis `main` et `/ (root)`, puis **Save**.
6. Attends la publication, puis ouvre l'adresse GitHub Pages indiquée dans cette page. Elle sera généralement de la forme `https://TON-COMPTE.github.io/bpu-explorer/`.

## Installer sur téléphone ou ordinateur
- **Android / Chrome** : ouvre l'adresse HTTPS publiée, puis le menu ⋮ et `Installer l'application` ou `Ajouter à l'écran d'accueil`.
- **iPhone / Safari** : ouvre l'adresse, touche `Partager`, puis `Sur l'écran d'accueil`.
- **Ordinateur / Chrome ou Edge** : ouvre l'adresse et utilise l'icône d'installation dans la barre d'adresse si elle apparaît, ou le menu du navigateur.

L'installation PWA nécessite une adresse HTTPS (GitHub Pages convient). L'ouverture directe du fichier HTML local permet de tester l'application, mais pas d'activer toutes les fonctions d'installation et de mise en cache. Après la première ouverture en ligne, l'application peut être disponible hors connexion.

## Mettre à jour plus tard
Remplace `index.html` par la nouvelle version et valide les changements sur GitHub. Si tu modifies aussi le cache, incrémente `bpu-explorer-v1` dans `sw.js` (par exemple `bpu-explorer-v2`) pour forcer la mise à jour.
