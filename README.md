# Atlas Identity System

Construire une identité professionnelle une fois. Générer des candidatures adaptées ensuite.

Atlas Identity System est un système éditorial personnel destiné à produire des CV, lettres de motivation, portfolios, biographies, prompts IA et dossiers de candidature à partir d'une base de connaissances unique.

Le projet ne vise pas à générer un document isolé. Il organise les informations professionnelles sous forme de modules réutilisables : identité, expériences, compétences, formation, culture, profils cibles, templates, règles éditoriales, direction visuelle et stratégies de candidature.

## Principe

Chaque information doit exister une seule fois, dans le fichier le plus proche de sa nature :

- `content/` contient la matière source : identité, expériences, compétences, formation et regards culturels.
- `profiles/` sélectionne et hiérarchise cette matière selon un angle professionnel.
- `templates/` décrit la structure des livrables sans figer un poste ou une organisation.
- `design-system/` rassemble les choix visuels et éditoriaux.
- `commands/` contient les prompts de génération pour Codex.
- `renderers/` documente le passage vers Firefly, Adobe Express et InDesign.
- `prompts/` encadre les usages IA sans remplacer la base de connaissances.
- `jobs/` contient les notes et stratégies propres à une candidature.

## Workflow

Le repo reste unique, mais chaque dossier a un rôle clair :

- `content/` = connaissances : identité, expériences, compétences, formation, culture.
- `profiles/` = angles de candidature : culture, web, formation, tourisme, relation client.
- `templates/` = structures éditoriales : CV, lettre, portfolio, email.
- `design-system/` = direction visuelle et principes éditoriaux.
- `commands/` = prompts de génération utilisés par Codex.
- `jobs/` = candidatures produites, dossier par dossier.
- `renderers/` = modes d'emploi pour Firefly, Adobe Express et InDesign.

Pipeline :

Identity System  
-> Codex : analyse, sélection, structuration, rédaction  
-> Firefly : direction artistique, moodboard, intentions visuelles  
-> Adobe Express : mise en page rapide éditable  
-> InDesign : production éditoriale avancée  
-> PDF final

## Usage prévu

1. Maintenir les informations factuelles dans `content/`.
2. Choisir un angle dans `profiles/`.
3. Utiliser une commande dans `commands/`.
4. Utiliser un template adapté au livrable.
5. Produire la candidature dans `jobs/`.
6. Préparer le rendu avec `renderers/` sans déplacer la source de vérité.

## Règle centrale

Le système peut reformuler, sélectionner et structurer. Il ne doit pas inventer d'informations personnelles, de dates, de résultats, d'employeurs, de diplômes ou de compétences absentes de la base.

## État du projet

Cette version pose l'architecture initiale du Personal Editorial System et un pipeline simple de génération de candidatures. Elle ne génère pas encore de PDF, HTML ou fichier graphique.
