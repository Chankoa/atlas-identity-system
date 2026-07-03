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
- `prompts/` encadre les usages IA sans remplacer la base de connaissances.
- `jobs/` contient les notes et stratégies propres à une candidature.

## Usage prévu

1. Maintenir les informations factuelles dans `content/`.
2. Choisir un angle dans `profiles/`.
3. Utiliser un template adapté au livrable.
4. Adapter la candidature dans `jobs/` à partir d'une offre réelle.
5. Générer ou rédiger une version finale en respectant les règles du système.

## Règle centrale

Le système peut reformuler, sélectionner et structurer. Il ne doit pas inventer d'informations personnelles, de dates, de résultats, d'employeurs, de diplômes ou de compétences absentes de la base.

## État du projet

Cette version pose l'architecture initiale du Personal Editorial System. Elle ne génère pas encore de PDF, HTML ou mise en page graphique.
