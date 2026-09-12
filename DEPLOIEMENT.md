# MASTERPLAN — Installation sur iPhone

L'app est un site web statique. Pour l'avoir sur ton écran d'accueil, il faut qu'elle soit servie depuis une adresse https. Deux options, les deux gratuites. Compte 3 minutes.

## Option A — Netlify Drop (le plus simple)

1. Va sur **app.netlify.com/drop** depuis ton Mac
2. Crée un compte si nécessaire (gratuit, email suffit)
3. Glisse-dépose **le dossier entier** (`index.html`, `manifest.json`, `sw.js`, les 3 icônes)
4. Netlify te donne une URL du type `https://xxx-yyy.netlify.app` — copie-la
5. Optionnel : renomme le site dans *Site settings → Change site name* pour avoir `https://masterplan-arthur.netlify.app`

## Option B — GitHub Pages

1. Crée un dépôt `masterplan` (public ou privé, les deux marchent)
2. Uploade les 6 fichiers à la racine
3. *Settings → Pages → Source : Deploy from branch → main → / (root)* → Save
4. URL : `https://<ton-user>.github.io/masterplan/`

## Ajouter à l'écran d'accueil (iPhone)

1. Ouvre l'URL dans **Safari** (pas Chrome — seul Safari sait installer)
2. Bouton **Partager** (carré avec flèche) → **Sur l'écran d'accueil**
3. Nomme-la MASTERPLAN → **Ajouter**

L'icône apparaît comme une app native, plein écran, sans barre Safari. Elle fonctionne hors ligne après la première ouverture.

## Où sont les données

Tout est stocké **sur ton iPhone** (localStorage du navigateur). Rien ne part sur un serveur.

Conséquence : si tu supprimes l'app de l'écran d'accueil ou vides les données Safari, tout est perdu. **Exporte un JSON une fois par semaine** — bouton ⚙️ → Exporter. Le fichier atterrit dans Fichiers, tu peux le mettre sur iCloud.

Pour restaurer : ⚙️ → Importer → choisir le JSON.

## Mettre à jour l'app

Quand je te livre une nouvelle version : remplace les fichiers sur Netlify (re-drop du dossier) ou GitHub. Tes données ne sont pas touchées — elles vivent dans le navigateur, pas dans les fichiers.

Si l'app semble ne pas se mettre à jour : fermer complètement l'app (swipe up), rouvrir. Le service worker recharge en arrière-plan.

## Whoop

Il n'y a pas d'API Whoop grand public accessible depuis une page statique. La saisie est manuelle — 4 chiffres le matin, 20 secondes. Le jour où Whoop ouvre un accès, on branchera.
