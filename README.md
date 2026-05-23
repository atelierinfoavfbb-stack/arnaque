# AVF Sécurité — Application anti-arnaques

## Déploiement GitHub Pages

### Étapes d'installation

**1. Créer le dépôt GitHub**
- Aller sur github.com → "New repository"
- Nom : `avf-securite` (ou `avf-alerte`)
- Cocher "Public"
- Cliquer "Create repository"

**2. Déposer les fichiers**
- Sur la page du dépôt → "uploading an existing file"
- Glisser tous les fichiers de ce dossier
- "Commit changes"

**3. Activer GitHub Pages**
- Settings du dépôt → Pages (menu gauche)
- Source : "Deploy from a branch" → branch "main" → dossier "/ (root)"
- Save

**4. L'application sera accessible sur :**
`https://[votre-compte].github.io/avf-securite/`

---

## Domaine personnalisé (optionnel)

Pour utiliser `aide.avfboulognebillancourt.fr` :

**Chez votre registrar (OVH, Gandi, etc.) :**
Ajouter un enregistrement DNS de type `CNAME` :
```
aide    CNAME    [votre-compte].github.io.
```

**Dans GitHub Pages Settings :**
Custom domain → `aide.avfboulognebillancourt.fr`
Cocher "Enforce HTTPS"

**Créer le fichier CNAME dans ce dossier :**
```
aide.avfboulognebillancourt.fr
```
(fichier sans extension, une seule ligne)

---

## Mise à jour du contenu

Toute modification d'un fichier sur GitHub est publiée en 1 à 3 minutes.

Pour mettre à jour la liste des référents AVF ou les numéros de contact :
- Modifier `index.html` ligne ~320 (section "Référent numérique AVF")
- Incrémenter la version dans `sw.js` : `avf-securite-v2`, `v3`...

---

## Installation sur les téléphones (à faire en Atelier 3)

**iPhone (Safari uniquement) :**
1. Ouvrir Safari → taper l'adresse du site
2. Bouton "Partager" (carré avec flèche)
3. "Sur l'écran d'accueil"
4. "Ajouter"

**Android (Chrome) :**
1. Ouvrir Chrome → taper l'adresse
2. Menu "⋮" → "Ajouter à l'écran d'accueil"
3. "Installer"

L'icône AVF rouge apparaît sur l'écran d'accueil.
L'application fonctionne ensuite **hors connexion**.
