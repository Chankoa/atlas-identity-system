# Renderers

Ce dossier documente comment transformer les contenus Markdown générés en supports visuels éditables.

Il ne contient pas de fichiers graphiques réels pour l'instant. Il décrit seulement le passage entre l'Identity System et les outils de rendu.

## Rôle des renderers

- `firefly.md` : préparer la direction artistique, les intentions visuelles et les prompts d'image.
- `adobe-express.md` : créer rapidement une version éditable et exportable.
- `indesign.md` : produire une version éditoriale avancée, mieux contrôlée pour impression ou PDF final.

## Pipeline général

Identity System  
-> Codex : analyse, sélection, structuration, rédaction  
-> Firefly : direction artistique, moodboard, intentions visuelles  
-> Adobe Express : mise en page rapide éditable  
-> InDesign : production éditoriale avancée  
-> PDF final

## Règle

Le Markdown reste la source éditoriale. Les outils de rendu ne doivent pas devenir la source de vérité du contenu.
