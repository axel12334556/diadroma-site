# Charte graphique Diadroma — « itinéraire »

Idée : une preuve est un **trajet**. Chaque étape (votre poste, le dépôt, le lot, Bitcoin) est une **station** reliée par une ligne.
Le nom évoque aussi les poissons diadromes, qui migrent entre deux milieux, comme la donnée voyage entre chez vous et la chaîne publique.

## Symbole

`assets/logo-mark.svg` (aussi `favicon.svg`) : un trait qui monte à 45°, deux stations creuses et une station pleine verte (l'ancrage).
Fond marine arrondi. Ne pas déformer, ne pas changer les couleurs, ne pas ajouter d'effets. Espace libre autour : au moins la moitié de la hauteur du symbole.
Le nom s'écrit « Diadroma », en titre gras (police des titres), à droite du symbole.

## Couleurs (variables dans `style/tokens.css`)

| Rôle | Valeur (clair) | Usage |
|---|---|---|
| Fond | `#FBFBFD` | fond de page |
| Aplat | `#F5F5F7` | sections alternées, tuiles |
| Texte | `#1D1D1F` | texte principal |
| Texte doux | `#6E6E73` | texte secondaire |
| Marine | `#0F1E3C` | boutons, symbole |
| Menthe | `#1FB58F` | signal « vérifié », station d'arrivée |
| Ambre | `#E8920A` | signal « en attente » |
| Nuit | `#1D1D1F` | une seule bande sombre : le message essentiel |
| Lien | `#0066CC` | liens |

Règles : beaucoup d'espace et de blanc ; un seul accent (menthe), jamais en texte sur fond clair (utiliser `--menthe-texte`
`#0B7A5E`) ; l'ambre uniquement pour « en attente » ; pas de dégradés, pas de lueurs, pas d'ombres appuyées ; une seule bande sombre par page.
Le thème sombre suit le réglage du visiteur. Contrastes mesurés ≥ 4,5:1 pour les textes.

## Typographie

Polices du système uniquement (aucune police externe, pour la vitesse, la confidentialité et la politique de sécurité du site) :
très grands titres gras à interlettrage serré (police système : SF Pro sur Apple, Segoe UI ou Roboto ailleurs), texte en police système, **empreintes et identifiants en monospace**.

## Motifs

- Lignes fines et régulières, stations en cercles (creux = étape, plein vert = arrivée). Un titre = une idée = une section.
- Un composant central : `.route` (itinéraire horizontal sur grand écran, vertical sur téléphone).
- Les niveaux d'une preuve se montrent comme des stations : creux gris = étape, ambre = en attente, plein vert = vérifié.

## Ton

Précis, calme, sans promesse excessive. Dire ce qu'une preuve établit **et ce qu'elle n'établit pas**. Toujours rappeler l'absence de clé de récupération.

## Contraintes techniques

HTML et CSS seulement, aucun script ; politique de sécurité de contenu stricte (`default-src 'none'`, pas d'attribut `style` en ligne).
