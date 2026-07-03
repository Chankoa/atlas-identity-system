# Architecture

L'architecture sépare strictement la matière source, les profils d'adaptation, les templates, les directions graphiques, les commandes de génération, les candidatures produites et les modes de rendu.

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

## `commands/`

Contient les commandes de génération utilisées par Codex.

Chaque fichier `commands/*.md` définit :

- l'objectif de la commande ;
- les sources à lire ;
- les sorties attendues ;
- les règles à respecter ;
- ce que Codex peut reformuler ;
- ce que Codex ne doit jamais inventer.

## `prompts/`

Contient les consignes destinées aux outils IA. Les prompts doivent rappeler la règle de non-invention et utiliser les fichiers sources comme seule base.

## `jobs/`

Contient les dossiers de candidature. Chaque sous-dossier correspond à une opportunité, une structure ou une offre.

Un dossier de candidature peut contenir :

- une analyse ;
- un CV ciblé ;
- une lettre ;
- un email ;
- des briefs de rendu ;
- une spécification InDesign ;
- un workflow d'export.

## `renderers/`

Documente le passage des fichiers Markdown vers les outils de rendu.

- Firefly : direction artistique, moodboard, intentions visuelles.
- Adobe Express : mise en page rapide éditable.
- InDesign : production éditoriale avancée.
- PDF final : export manuel depuis l'outil de rendu retenu.

## Flux de dépendance

Les dépendances doivent rester descendantes :

`content/` -> `profiles/` -> `commands/` -> `templates/` -> `jobs/`

`design-system/` et `renderers/` encadrent le rendu, mais ne remplacent pas la matière source.

## Pipeline de génération

Identity System  
-> Codex : analyse, sélection, structuration, rédaction  
-> Firefly : direction artistique, moodboard, intentions visuelles  
-> Adobe Express : mise en page rapide éditable  
-> InDesign : production éditoriale avancée  
-> PDF final

## Règle de source unique

Le Markdown reste la source de vérité. Les fichiers produits dans Adobe Express, InDesign ou en PDF sont des sorties éditables ou finales, pas des sources à réinjecter sans contrôle.
