# Portfolio — Froshe

Portfolio personnel d'Axel Kramer (Froshe), étudiant en Master Informatique (parcours IMAGINE) à l'Université de Montpellier.

Site en un seul fichier `index.html` (HTML/CSS/JS inline), avec vidéo de fond, musique, modèles 3D interactifs (`model-viewer`) et CV téléchargeable.

## Déploiement (GitHub Pages)

1. Settings → Pages → Source: `Deploy from a branch`, branche `main`, dossier `/ (root)`.
2. Le site est ensuite disponible à `https://<ton-pseudo>.github.io/<nom-du-repo>/`.

## Fichiers
- `index.html` — le site
- `menu.mp4` — vidéo de fond en boucle (raccourcie et compressée depuis l'original 390 Mo/30 min)
- `music.mp3` — musique de fond
- `model1.glb`, `model2.glb`, `model3.glb` — modèles 3D (Givrali, Moustillon, Manny Calavera)
- `cv.pdf` — CV téléchargeable
- `menu-poster.jpg` — première image de la vidéo, affichée si la lecture auto est bloquée (Safari en mode économie d'énergie…)
- `fonts/anton.woff2` — police Anton hébergée avec le site (rendu identique Mac / Windows / mobile)
- `lib/model-viewer.min.js` — model-viewer 4.2.0 hébergé localement (build classique)

## Tester en local
Ouvrir `index.html` en double-cliquant fonctionne, **sauf les modèles 3D** : les navigateurs bloquent le chargement des `.glb` depuis `file://`.
Pour tout tester : `python3 -m http.server` dans ce dossier puis http://localhost:8000 (ou l'extension Live Server de VS Code).
