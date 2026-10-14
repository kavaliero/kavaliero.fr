# kavaliero.fr

La page de liens de Kavaliero, dans la DA « Heure dorée ». Un site statique : une seule page, sans outil de construction. Il suffit de déposer ce dossier chez n'importe quel hébergeur de sites statiques.

## Contenu

| Fichier | Rôle |
| --- | --- |
| `index.html` | la page, avec ses styles |
| `assets/` | bannière (800 et 1536 px de large), avatar, icône du serveur, emoji de L'Écuyer, icônes des liens (`assets/icones/`) |
| `fonts/` | Jersey 10, Jersey 15 et New Rocker en woff2, réduites aux caractères latins et français, avec leurs licences OFL. Hébergées ici : aucun appel à Google Fonts. |
| `favicon.ico`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `site.webmanifest` | l'icône d'onglet et d'écran d'accueil (l'écu au K du serveur) |
| `og-image.jpg` | l'aperçu affiché quand on colle le lien sur Discord, X, etc. (1200 × 630) |

## Modifier un lien

Dans `index.html`, chaque lien est un bloc `<li><a class="lien" href="…">` avec son icône, son titre et son sous-titre. Change l'adresse dans `href` ou le texte entre les balises.

Les polices Jersey ne sont nettes qu'à certaines tailles : Jersey 10 à 18.667px ou 37.333px, Jersey 15 à 27px. Garde ces valeurs si tu touches aux styles.

## Adresses absolues

`og:url`, `og:image` et `canonical` pointent vers `https://kavaliero.fr/`. Si le site part sur une autre adresse, change-les dans le `<head>` de `index.html`.
