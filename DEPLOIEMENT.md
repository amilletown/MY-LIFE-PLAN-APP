# MASTERPLAN v3 — Installation

## 1. Mettre en ligne (3 min, une seule fois)

**Depuis l'app GitHub iOS :** ＋ → Create repository → nom `masterplan` → Public → Create.

**Depuis Safari** (l'app ne sait pas uploader de fichiers ni activer Pages) :
1. `github.com/<toi>/masterplan` → *uploading an existing file* → sélectionner les 7 fichiers (index.html, sw.js, manifest.json, 3 icônes, ce guide) du dossier → *Commit changes*
2. *Settings → Pages → Source : Deploy from a branch → main → / (root) → Save*
3. Attendre 1 min, rafraîchir, copier l'URL `https://<toi>.github.io/masterplan/`

## 2. Installer sur l'iPhone

Ouvrir l'URL dans **Safari** → bouton Partager → **Sur l'écran d'accueil**.

## 3. Activer le coach IA

1. console.anthropic.com → API keys → Create key → copier
2. Dans l'app : Plus → Coach IA → coller la clé → OK

La clé reste sur ton téléphone. Coût : moins d'un centime par question avec Sonnet.

## Mise à jour

Si tu avais la v1 : tes données sont reprises automatiquement au premier lancement.
Pour une nouvelle version : remplacer les fichiers sur GitHub. Tes données ne bougent pas — elles vivent dans le navigateur.

## Sauvegarde

Plus → Exporter les données, une fois par semaine. Le JSON va dans Fichiers.

## Vérifier que la mise à jour est bien chargée

Plus → tout en bas : la ligne « Forcer la mise à jour » affiche la version (v3.4 ou plus récente).
Si elle affiche « Version — » ou n'existe pas, l'ancien index.html est encore servi : vérifie que le fichier a bien été remplacé sur GitHub (Commit changes), attends 1–2 min, puis ferme l'app complètement (balayer vers le haut) et rouvre-la.
Sinon, touche « Forcer la mise à jour » : ça vide le cache de l'app et recharge. Tes données ne sont pas touchées.
