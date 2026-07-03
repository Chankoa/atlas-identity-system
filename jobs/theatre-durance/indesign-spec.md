# Spécification InDesign - Théâtre Durance

## Objectif

Préparer une version éditoriale avancée de la candidature dans InDesign, à partir des contenus Markdown déjà rédigés.

Cette spécification ne crée pas de fichier `.indd`. Elle décrit les styles, la grille et les règles de production.

## Sources

- `jobs/theatre-durance/cv-culture.md`
- `jobs/theatre-durance/lettre-motivation.md`
- `jobs/theatre-durance/firefly-brief.md`
- `jobs/theatre-durance/adobe-express-brief.md`
- `design-system/colors.md`
- `design-system/typography.md`
- `design-system/grid.md`
- `design-system/editorial-principles.md`

## Format

- CV : A4 vertical, une page.
- Lettre : A4 vertical, une à deux pages selon le contenu final.
- Marges généreuses pour renforcer l'approche éditoriale.
- Grille simple : une colonne principale, avec possibilité d'une colonne courte pour les coordonnées ou repères.

## Couleurs

- Texte principal : `#202020`
- Fond : `#FAF8F4` ou blanc si l'export doit rester très sobre.
- Accent secondaire : `#667A8A`
- Accent discret : `#73806C`

## Typographies

- Titres : Cormorant Garamond ou serif éditoriale équivalente.
- Texte courant : Source Sans 3 ou sans-serif lisible équivalente.

Si les polices ne sont pas installées, utiliser des alternatives disponibles sans modifier l'esprit : serif éditoriale pour les titres, sans-serif sobre pour le texte.

## Styles de paragraphe à créer

- `Nom` : grand, serif, noir doux.
- `Titre de candidature` : serif ou sans-serif forte, accent discret possible.
- `Coordonnées` : sans-serif, petit corps, interligne confortable.
- `Accroche` : corps légèrement supérieur au texte courant.
- `Rubrique` : titre court, hiérarchie nette, espace avant.
- `Texte courant` : sans-serif lisible.
- `Liste compétences` : puces sobres, interligne régulier.
- `Expérience` : intitulé en semi-bold, période en style secondaire.
- `Note à compléter` : style discret pour repérer les `[à compléter]` avant export.

## Styles de caractère

- `Accent` : `#667A8A` ou `#73806C`.
- `Information manquante` : couleur d'alerte discrète à retirer avant export final.
- `Lien` : accent secondaire, sans soulignement si la lisibilité reste bonne.

## Règles de composition

- Préserver les blancs.
- Limiter les effets graphiques.
- Ne pas multiplier les encadrés.
- Maintenir une hiérarchie immédiate entre identité, compétences et parcours.
- Garder les textes en blocs éditables.
- Ne pas vectoriser les textes.

## Export PDF

- Exporter après relecture complète.
- Vérifier les liens et coordonnées.
- Vérifier que toutes les mentions `[à compléter]` ont été traitées ou volontairement conservées.
- Exporter en PDF standard pour envoi numérique.
- Conserver le fichier InDesign éditable séparément du PDF final.
