# Commande - Générer un dossier de candidature complet

## Objectif

Produire un dossier de candidature complet dans `jobs/[candidature]/` à partir de l'Identity System.

Cette commande orchestre les autres commandes : analyse, CV, lettre, email, brief Firefly, brief Adobe Express et spécification InDesign.

## Fichiers sources à utiliser

- `content/` pour les faits, expériences, compétences et éléments d'identité.
- `profiles/[profil].md` pour l'angle de candidature.
- `templates/` pour la structure des livrables.
- `design-system/` pour les règles éditoriales et graphiques.
- `jobs/[candidature]/offer-notes.md` pour le contexte de l'offre.
- `jobs/[candidature]/strategy.md` pour la stratégie retenue.

## Fichiers de sortie attendus

- `jobs/[candidature]/analysis.md`
- `jobs/[candidature]/cv-[profil].md`
- `jobs/[candidature]/lettre-motivation.md`
- `jobs/[candidature]/email-candidature.md`
- `jobs/[candidature]/firefly-brief.md`
- `jobs/[candidature]/adobe-express-brief.md`
- `jobs/[candidature]/indesign-spec.md`
- `jobs/[candidature]/rendering-workflow.md`

## Règles à respecter

- Conserver une séparation stricte entre sources, adaptation, rédaction et rendu.
- Écrire en Markdown uniquement.
- Produire des fichiers directement exploitables.
- Marquer les informations manquantes avec `[à compléter]`.
- Ne pas générer de PDF, HTML ou fichier graphique.

## Ce que Codex peut reformuler

- Une accroche de CV à partir du positionnement existant.
- Une lettre à partir du profil, de la stratégie et des notes d'offre.
- Un email court à partir du CV et de la lettre.
- Des briefs de rendu à partir du design system.
- Une structure de mise en page éditoriale.

## Ce que Codex ne doit jamais inventer

- Diplômes, dates, employeurs, clients, missions, résultats chiffrés.
- Connaissance précise d'une structure si elle n'est pas documentée.
- Niveau de maîtrise d'un outil non confirmé.
- Pièces jointes effectivement produites si elles ne le sont pas.
- Identité graphique officielle d'une organisation.
