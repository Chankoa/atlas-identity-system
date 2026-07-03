# Workflow

Le workflow part de la base de connaissances et va jusqu'au PDF final, sans créer de second repo ni déplacer la source de vérité hors du Markdown.

Pipeline général :

Identity System  
-> Codex : analyse, sélection, structuration, rédaction  
-> Firefly : direction artistique, moodboard, intentions visuelles  
-> Adobe Express : mise en page rapide éditable  
-> InDesign : production éditoriale avancée  
-> PDF final

## 1. Ajouter ou corriger la matière source

Toute information personnelle ou professionnelle doit d'abord être ajoutée dans `content/`.

Exemples :

- une expérience dans `content/experiences/` ;
- une compétence dans `content/skills/` ;
- une formulation d'identité dans `content/identity/`.

## 2. Qualifier l'information

Chaque bloc doit distinguer :

- les faits établis ;
- les formulations éditoriales ;
- les éléments à vérifier ;
- les preuves ou exemples à rattacher.

## 3. Choisir un profil

Le profil sert à orienter la sélection. Il ne doit pas créer de contenu nouveau.

Exemples :

- `profiles/culture-communication.md` pour une structure culturelle ;
- `profiles/web-front-end.md` pour un poste web ;
- `profiles/formation.md` pour un rôle de transmission.

## 4. Choisir un template

Le template définit le livrable :

- CV ;
- lettre de motivation ;
- portfolio ;
- email de candidature.

## 5. Choisir une commande de génération

Les commandes de `commands/` indiquent à Codex quoi produire et quelles limites respecter.

Exemples :

- `commands/generate-application-package.md` pour un dossier complet ;
- `commands/generate-cv.md` pour un CV ciblé ;
- `commands/generate-cover-letter.md` pour une lettre ;
- `commands/generate-firefly-brief.md` pour une direction artistique ;
- `commands/generate-adobe-express-brief.md` pour une mise en page rapide ;
- `commands/generate-indesign-spec.md` pour une production éditoriale avancée.

## 6. Créer un dossier de candidature

Chaque candidature doit avoir son espace dans `jobs/`.

Le dossier rassemble les notes sur l'offre, la stratégie de réponse et les choix éditoriaux.

## 7. Produire les fichiers Markdown

La production doit rester traçable :

- aucun fait non présent dans `content/` ;
- aucune promesse non vérifiée ;
- une adaptation réelle au destinataire ;
- une écriture sobre, claire et professionnelle.

## 8. Préparer la direction artistique avec Firefly

Utiliser `jobs/[candidature]/firefly-brief.md` et `renderers/firefly.md`.

Firefly sert à explorer une ambiance, une matière visuelle et une direction graphique. Il ne doit pas devenir la source du texte final.

## 9. Mettre en page dans Adobe Express

Utiliser `jobs/[candidature]/adobe-express-brief.md` et `renderers/adobe-express.md`.

Adobe Express sert à produire rapidement une version éditable. Les textes doivent rester modifiables, pas être figés dans une image.

## 10. Produire une version avancée dans InDesign

Utiliser `jobs/[candidature]/indesign-spec.md` et `renderers/indesign.md`.

InDesign sert à contrôler finement la grille, les styles, la typographie et l'export PDF.

## 11. Exporter le PDF final

Le PDF final est exporté manuellement depuis Adobe Express ou InDesign après relecture.

Le PDF n'est pas généré par le repo et ne remplace pas les fichiers Markdown sources.
