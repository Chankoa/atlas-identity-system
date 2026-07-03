# Renderer - InDesign

## Rôle

InDesign sert à produire une version éditoriale avancée : meilleure maîtrise de la grille, des styles, des marges, de la typographie et de l'export PDF.

Il intervient après la validation du contenu Markdown.

## Entrées Markdown

- `jobs/[candidature]/cv-[profil].md`
- `jobs/[candidature]/lettre-motivation.md`
- `jobs/[candidature]/indesign-spec.md`
- `jobs/[candidature]/firefly-brief.md`
- `design-system/colors.md`
- `design-system/typography.md`
- `design-system/grid.md`

## Usage recommandé

1. Créer un fichier InDesign par candidature ou un modèle réutilisable.
2. Créer les styles de paragraphe et de caractère avant d'importer tout le contenu.
3. Copier ou importer les textes depuis Markdown.
4. Conserver les blocs de texte éditables.
5. Exporter un PDF final après contrôle typographique et relecture.

## Sorties attendues

- Fichier InDesign éditable.
- PDF final exporté manuellement.
- Éventuellement un package InDesign si des polices ou images sont utilisées.

## Limites

- Ne pas générer un fichier InDesign depuis Codex.
- Ne pas figer les textes en contours ou en image.
- Ne pas utiliser de polices, images ou assets non disponibles.
