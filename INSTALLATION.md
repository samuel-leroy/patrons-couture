# Patrons — installation (10 minutes)

L'application est hébergée sur GitHub Pages (comme le Carnet d'entretien). Les fiches, photos et PDF sont stockés dans votre Google Drive, dans le dossier « Patrons couture », créé automatiquement.

## 1. Récupérer l'ID client Google
Utilisez le même que celui du Carnet d'entretien. Il se trouve dans le code du Carnet (cherchez `apps.googleusercontent.com`) ou dans Google Cloud Console › API et services › Identifiants.
L'origine `https://samuel-leroy.github.io` est déjà autorisée pour le Carnet, rien à ajouter. Collez l'ID dans `index.html`, à la ligne :

```js
const CLIENT_ID = 'COLLER_ICI_VOTRE_ID_CLIENT.apps.googleusercontent.com';
```

## 2. Publier sur GitHub
1. Créez un dépôt `patrons-couture` sur GitHub.
2. Déposez-y les 5 fichiers : `index.html`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`.
3. Settings › Pages › Branch `main` / dossier `/ (root)` › Save.
4. L'appli sera disponible sur `https://samuel-leroy.github.io/patrons-couture/`.

## 3. Premier lancement
1. Ouvrez l'adresse sur le téléphone, puis « Se connecter » avec le compte Google du foyer, celui qui sert au Carnet.
2. Menu du navigateur › « Ajouter à l'écran d'accueil » / « Installer l'application ».
3. Sur PC, ouvrez simplement l'adresse avec le même compte.

## Confidentialité
- Seul le code de l'appli est public. Aucune donnée n'est dans GitHub.
- Les données sont dans votre Drive et n'apparaissent qu'après connexion avec le compte Google du foyer. L'appli n'a accès qu'aux fichiers qu'elle a elle-même créés (droit `drive.file`).
- Ne partagez pas le dossier « Patrons couture » par lien public.

## Mises à jour sans perte
- Pour mettre à jour, remplacez les fichiers dans GitHub. Les données ne sont jamais touchées, car elles sont dans Drive.
- Les nouveaux champs ou listes sont ajoutés aux fiches existantes sans rien effacer (migration automatique).
- Une copie de travail est gardée sur chaque appareil, et la synchro fusionne les modifications fiche par fiche.
- Une sauvegarde quotidienne est créée dans Drive (Patrons couture › Sauvegardes, 20 conservées).
- La suppression passe d'abord par la corbeille.
