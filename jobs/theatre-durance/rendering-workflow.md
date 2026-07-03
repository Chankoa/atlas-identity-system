# Workflow de rendu - Théâtre Durance

## Objectif

Transformer les fichiers Markdown de la candidature en supports éditables puis en PDF final, sans perdre la source de vérité.

Le contenu source reste dans `jobs/theatre-durance/`.

## Mode rapide

1. Relire `cv-culture.md` et `lettre-motivation.md`.
2. Supprimer ou compléter la ligne portfolio si nécessaire.
3. Générer une ambiance dans Firefly avec le prompt principal de `firefly-brief.md`.
4. Monter rapidement le CV dans Adobe Express en A4 vertical.
5. Exporter un PDF de relecture.
6. Si le rendu doit être plus éditorial, reconstruire le CV dans InDesign avec les styles de `indesign-spec.md`.
7. Exporter les PDF finaux : CV et lettre.

## 1. Préparer les fichiers Markdown

Relire et compléter en priorité :

- `jobs/theatre-durance/cv-culture.md`
- `jobs/theatre-durance/lettre-motivation.md`
- `jobs/theatre-durance/email-candidature.md`
- `jobs/theatre-durance/firefly-brief.md`
- `jobs/theatre-durance/adobe-express-brief.md`
- `jobs/theatre-durance/indesign-spec.md`

Avant rendu, remplacer les `[à compléter]` quand l'information est vérifiée.

Points à vérifier avant mise en page :

- portfolio ou LinkedIn ;
- disponibilité du 12 octobre 2026 au 12 février 2027 ;
- disponibilité soirs, week-ends et déplacements ;
- permis B, seulement s'il est confirmé.

## 2. Copier dans Firefly

Copier depuis `jobs/theatre-durance/firefly-brief.md` :

- le prompt principal ;
- le prompt négatif ;
- les mots-clés ;
- la palette ;
- les contraintes d'image et de matière.

Ne pas copier toute la lettre ou tout le CV dans Firefly. Firefly sert à produire une ambiance visuelle, pas à mettre en page le texte final.

Coller ce type de demande dans Firefly :

`Direction graphique pour une candidature de chargé de communication culturelle dans une scène nationale de territoire, inspirée du design éditorial culturel français, catalogues d'exposition et programmes de festivals, grands espaces blancs, typographie forte, mise en page sobre et contemporaine, papier mat, communication culture territoire publics, spectacle vivant, musique, création sonore, audio-balade, Verdon, médiation, sans logo existant, sans imitation d'identité réelle.`

Sortie à conserver :

- moodboard ;
- image d'ambiance éventuelle ;
- notes sur les choix retenus.

## 3. Copier dans Adobe Express

Créer un document A4 vertical.

Copier le contenu depuis :

- `jobs/theatre-durance/cv-culture.md` pour le CV ;
- `jobs/theatre-durance/lettre-motivation.md` pour la lettre ;
- `jobs/theatre-durance/firefly-brief.md` pour l'ambiance ;
- `jobs/theatre-durance/adobe-express-brief.md` pour les consignes de mise en page.

Appliquer :

- fond clair `#FAF8F4` ou blanc ;
- texte `#202020` ;
- accents `#667A8A` et `#73806C` ;
- grands espaces blancs ;
- titres forts ;
- textes courts et éditables.

Conserver une version éditable dans Adobe Express avant tout export PDF.

Workflow Express recommandé :

- document 1 : CV ;
- document 2 : lettre ;
- conserver les textes en blocs éditables ;
- exporter uniquement après relecture.

## 4. Appliquer les styles dans InDesign

Créer un document A4 vertical.

Styles de paragraphe à créer :

- `Nom`
- `Titre de candidature`
- `Coordonnées`
- `Accroche`
- `Rubrique`
- `Texte courant`
- `Liste compétences`
- `Expérience`
- `Note à compléter`

Styles de caractère à créer :

- `Accent`
- `Information manquante`
- `Lien`

Appliquer les couleurs et typographies définies dans :

- `design-system/colors.md`
- `design-system/typography.md`
- `jobs/theatre-durance/indesign-spec.md`

Le texte doit rester éditable. Ne pas transformer le texte en image ou en contours.

Workflow InDesign recommandé :

- créer les styles avant de coller le texte ;
- conserver une grille simple ;
- exporter d'abord un PDF de relecture ;
- corriger dans le fichier `.indd` ;
- exporter le PDF final.

## 5. Conserver une version éditable

À conserver :

- fichiers Markdown sources dans le repo ;
- document Adobe Express éditable si utilisé ;
- fichier InDesign `.indd` si utilisé ;
- export PDF final séparé.

Le PDF n'est jamais la source de vérité.

## 6. Exporter en PDF

Exporter manuellement depuis Adobe Express ou InDesign après contrôle :

- coordonnées complètes ;
- poste ciblé ;
- absence de `[à compléter]` non volontaire ;
- cohérence entre CV et lettre ;
- lisibilité du PDF ;
- poids de fichier acceptable pour envoi.

Nom de fichier recommandé :

- `Chandra-Josephus-CV-Theatre-Durance.pdf`
- `Chandra-Josephus-Lettre-Theatre-Durance.pdf`

Email d'envoi :

- destinataire : `administration@theatredurance.fr`
- attention : Élodie Presles, directrice
- objet : `Candidature - Chargé de communication - CDD remplacement congé maternité`

Les PDF ne sont pas générés par Codex dans ce sprint.
