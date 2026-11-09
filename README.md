# Astra Console

Site de lancement pour Astra Console. Ouvrir `index.html` après publication avec GitHub Pages.

`index.html` et `Astra-Console.html` sont la même console : `index.html` est la page du site,
`Astra-Console.html` est le fichier que les consoles installées téléchargent.

## Mettre à jour la console soi-même

1. Ouvre `Astra-Console.html` (ou `index.html`, ce sont les mêmes fichiers) et fais les modifications voulues.
2. Enregistre le fichier, puis dépose-le sur le dépôt sous **les deux noms** : `Astra-Console.html` et `index.html`.
3. Ouvre `updates/manifest.json` et augmente `version` (ex. `1.13.0` → `1.14.0`) en ajoutant une ligne dans `releaseNotes`.
4. Les consoles déjà installées voient alors « Nouvelle mise à jour Astra Console X.Y.Z disponible » et téléchargent `Astra-Console.html` depuis le dépôt.

## Le dossier `updates/` (pour mettre à jour les autres appareils)

- `updates/manifest.json` — version courante, notes de version et liens de téléchargement lus par l'application « Mise à jour ».
- `updates/astra-console-v1.13.0.zip` — la console complète en paquet : `index.html`, `Astra-Console.html`, `betrock.html`, `game.html`, `three.min.js`, `manifest.json`, `updates/manifest.json`, `LISEZ-MOI.txt`, `Lancer-Astra-Console.bat`.
- `astra-console-v1.1.0.zip` — ancien paquet, conservé.
- Version actuelle de la console : **1.13.0**.

Pour un autre appareil : télécharge le ZIP, décompresse-le dans un dossier « Astra Console », double-clique sur `Lancer-Astra-Console.bat` (ou ouvre `index.html`). Aucune installation, aucune connexion nécessaire.

Pour publier une nouvelle version : modifie `Astra-Console.html` et `index.html`, refais un ZIP nommé `astra-console-vX.Y.Z.zip` dans `updates/`, mets à jour `updates/manifest.json` (`version`, `package`, `packageUrl`, `releaseNotes`) et le `manifest.json` de la racine.

## Jeux disponibles

- **Grand Fast Horizon** — le jeu de conduite intégré à la console.
- **Betrock** — monde de blocs à explorer, casser et construire. Fichier source : `betrock.html`, intégré dans la console comme application, comme tuile de l'accueil et dans le dossier « Jeux ».

Commandes Betrock : souris pour viser, ZQSD pour marcher, clic gauche pour casser, clic droit pour poser, 1-5 pour choisir un bloc, Échap pour la pause.
