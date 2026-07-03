# Commande - Générer un CV

## Objectif

Produire un CV ciblé en Markdown pour une candidature donnée.

Le CV doit être une sélection structurée du système, pas une réécriture complète du parcours.

## Fichiers sources à utiliser

- `content/identity/`
- `content/experiences/`
- `content/skills/`
- `content/education/`
- `profiles/[profil].md`
- `templates/cv.md`
- `jobs/[candidature]/offer-notes.md`
- `jobs/[candidature]/strategy.md`

## Fichier de sortie attendu

- `jobs/[candidature]/cv-[profil].md`

## Règles à respecter

- Adapter le titre, l'accroche et l'ordre des rubriques au poste visé.
- Garder une forme concise, compatible avec une page.
- Relier chaque compétence à une source existante.
- Utiliser `[à compléter]` pour les dates, coordonnées, formations ou détails absents.
- Éviter les formulations trop générales.

## Ce que Codex peut reformuler

- L'accroche professionnelle.
- Les intitulés de rubriques.
- Les descriptions d'expériences déjà documentées.
- Les compétences transversales, si elles sont présentes dans `content/`.

## Ce que Codex ne doit jamais inventer

- Périodes d'emploi.
- Employeurs ou clients.
- Diplômes.
- Résultats mesurables.
- Logiciels ou technologies non documentés.
