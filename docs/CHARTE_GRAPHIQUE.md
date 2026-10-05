# Charte graphique Diadroma — « itinéraire »

Idée : une preuve est un **trajet**. Chaque étape (votre poste, le dépôt, le lot, Bitcoin) est une **station** reliée par une ligne.
Le nom évoque aussi les poissons diadromes, qui migrent entre deux milieux, comme la donnée voyage entre chez vous et la chaîne publique.

## Symbole

`assets/logo-mark.svg` (aussi `favicon.svg`) : un trait qui monte à 45°, deux stations creuses et une station pleine verte (l'ancrage).
Fond marine arrondi. Ne pas déformer, ne pas changer les couleurs, ne pas ajouter d'effets. Espace libre autour : au moins la moitié de la hauteur du symbole.
Le nom s'écrit « Diadroma », en titre gras (police des titres), à droite du symbole.

## Couleurs (variables dans `style/tokens.css`)

| Rôle | Valeur | Usage |
|---|---|---|
| Marine | `#0F1E3C` | bandeaux, texte principal en clair |
| Papier | `#F5F7FA` | fond de page en clair |
| Menthe | `#1FB58F` | signal « vérifié », stations d'arrivée, boutons principaux |
| Ambre | `#F5A524` | signal « en attente » |
| Texte doux | `#4A5A78` | texte secondaire |
| Lien | `#0B5CAD` | liens sur fond clair |

Règles : un seul accent fort (menthe) ; l'ambre uniquement pour « en attente » ; **la menthe vive ne sert pas de texte sur fond clair**
(utiliser `--menthe-texte` `#0B7A5E`). Contrastes mesurés ≥ 4,5:1 pour tout texte, en clair comme en sombre (thème sombre automatique).

## Typographie

Polices du système uniquement (aucune police externe, pour la vitesse, la confidentialité et la politique de sécurité du site) :
titres gras en `Avenir Next` / `Segoe UI`, texte en police système, **empreintes et identifiants en monospace**.

## Motifs

- Lignes épaisses, angles à 45° et 90°, extrémités arrondies ; stations en cercles (creux = étape, plein vert = arrivée).
- Un composant central : `.route` (itinéraire horizontal sur grand écran, vertical sur téléphone).
- Les niveaux d'une preuve se montrent comme des stations : creux gris = étape, ambre = en attente, plein vert = vérifié.

## Ton

Précis, calme, sans promesse excessive. Dire ce qu'une preuve établit **et ce qu'elle n'établit pas**. Toujours rappeler l'absence de clé de récupération.

## Contraintes techniques

HTML et CSS seulement, aucun script ; politique de sécurité de contenu stricte (`default-src 'none'`, pas d'attribut `style` en ligne).
