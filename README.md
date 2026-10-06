# Flashcards Soutenance AIS

Site statique de révision : 71 cartes (déroulé de l'oral, chiffres clés, questions du jury).
Aucune dépendance, aucun build : tout est dans `index.html`.

## Mettre en ligne avec GitHub Pages

1. Crée un dépôt (par exemple `flashcards-ais`) et mets tous les fichiers de ce dossier à la racine.
2. Dans le dépôt : **Settings → Pages → Build and deployment**.
3. Source : **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
4. Après une minute, le site est en ligne sur `https://<ton-pseudo>.github.io/flashcards-ais/`.

## Sur le téléphone

- Ouvre le lien, puis **Ajouter à l'écran d'accueil** (Safari : bouton Partager ; Chrome : menu ⋮).
- Après la première ouverture, le site marche aussi hors ligne.
- Tes cartes « Je sais » / « À revoir » sont gardées sur le téléphone.
- Glisse la carte à gauche ou à droite pour changer de carte.

## Modifier les cartes

Les cartes sont dans `index.html`, dans le tableau `CARDS`. Après une modification,
change `flashcards-ais-v1` en `v2` dans `sw.js` pour que les téléphones récupèrent la nouvelle version.
