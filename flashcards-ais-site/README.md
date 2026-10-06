# Flashcards Soutenance AIS

Site statique de révision : 71 cartes (déroulé de l'oral, chiffres clés, questions du jury).
Pour chaque carte, tu écris (ou dictes) ta réponse et le site la corrige : chaque point attendu s'affiche en ✓ trouvé ou ✗ manquant, avec un verdict Juste / Partiel / À revoir.
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

## Comment marche la correction

La correction se fait dans le téléphone, sans serveur : elle cherche les mots-clés de chaque point attendu
(chiffres, sigles, mots importants) dans ta réponse, sans tenir compte des accents ni des majuscules.
Elle ne comprend pas le sens : si tu utilises un synonyme, elle peut le rater. Dans ce cas, corrige
le classement avec les boutons « Je sais » / « À revoir ».

## Modifier les cartes

Les cartes sont dans `index.html`, dans le tableau `CARDS`. Après une modification,
incrémente le numéro de version `flashcards-ais-v2` (v3, v4…) dans `sw.js` pour que les téléphones récupèrent la nouvelle version.
