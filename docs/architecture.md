# Architecture

L'architecture sépare strictement la matière source, les règles, les templates, le design et les candidatures.

## `content/`

Contient les informations de fond. Ces fichiers ne doivent pas être écrits pour une candidature précise.

- `identity/` : positionnement, taglines, valeurs, biographies.
- `experiences/` : expériences professionnelles ou activités identifiées.
- `skills/` : compétences mobilisables.
- `education/` : formations et apprentissages.
- `culture/` : regards, références, angles d'analyse.

## `profiles/`

Contient des angles éditoriaux. Un profil n'ajoute pas de faits : il sélectionne, ordonne et pondère les modules de `content/`.

## `templates/`

Contient les structures de livrables. Un template définit une forme, pas un contenu final.

## `design-system/`

Contient les règles visuelles et éditoriales : couleurs, typographies, grille, direction d'image et principes de composition.

## `prompts/`

Contient les consignes destinées aux outils IA. Les prompts doivent rappeler la règle de non-invention et utiliser les fichiers sources comme seule base.

## `jobs/`

Contient les dossiers de candidature. Chaque sous-dossier correspond à une opportunité, une structure ou une offre.

## Flux de dépendance

Les dépendances doivent rester descendantes :

`content/` -> `profiles/` -> `templates/` -> livrables

`design-system/` et `prompts/` encadrent la production, mais ne remplacent pas la matière source.
