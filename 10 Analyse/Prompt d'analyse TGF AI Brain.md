---
type: outil
tags: [ai-brain, prompt, TGF2026]
---
# 🤖 Prompt d'analyse TGF AI Brain

Copie ce prompt dans Claude (ou donne simplement le transcript à Cowork en disant « analyse ce transcript pour le TGF AI Brain ») :

```
Tu analyses le transcript d'un talk du Tunisia Global Forum 2026 (« Bâtir l'avenir à l'ère de l'IA ») pour l'intégrer dans mon vault Obsidian « TGF AI Brain ».

SESSION : <nom de la session>
SPEAKERS : <noms>

Produis en markdown, en français :

## Résumé exécutif
3-5 phrases : le message central du talk.

## Notions
Les 5-12 concepts importants abordés. Pour chacun : **[[Nom de la notion]]** — définition en 1 ligne telle qu'utilisée par le speaker. Réutilise les notions existantes du vault quand le concept est identique (ne crée pas de doublons : vérifie 10 Analyse/Notions/).

## Phrases clés
5-10 verbatims courts à fort signal (position, chiffre, formule marquante), avec le nom du speaker.

## Citations mémorables
2-4 citations exactes dignes d'être conservées/publiées, format : « citation » — [[Speaker]]

## Chiffres & faits
Toutes les données chiffrées et faits vérifiables mentionnés.

## Recommandations & actions
Ce que le speaker propose de FAIRE (pour la Tunisie, l'écosystème, les entreprises).

## Questions ouvertes
Débats non tranchés, tensions, questions soulevées sans réponse.

## Connexions
Thèmes du vault concernés parmi : [[IA & Souveraineté]], [[Talents & Transformations]], [[Écosystème Startups]], [[Recherche & Innovation]], [[Diaspora tunisienne]], [[Gouvernance & Éthique de l'IA]], [[Infrastructures numériques & énergétiques]] + liens éventuels vers le [[Livre Blanc IA Tunisie]].

## Tags (liste FERMÉE - voir [[Taxonomie des tags]])
Chaque élément extrait reçoit :
- 1 tag de nature : #citation #chiffre #annonce #constat #recommandation #action-proposee #controverse #question-ouverte
- le tag de statut #brut (jamais #verifie ni #publie : réservés à l'éditeur)
- si un contenu ne rentre dans aucun thème existant : #theme-propose (ne JAMAIS créer de note de thème)

Règles : ne rien inventer ; rester fidèle au transcript ; wikilinks [[...]] pour toute notion, personne, session et thème (jamais de tags pour les entités) ; aucun tag hors liste fermée ; en cas de doute sur qui a dit quoi, rester en #brut et le signaler.
```

💡 Astuce Cowork : donne-moi directement le fichier audio/texte du talk et dis « intègre-le au TGF AI Brain » — je crée le transcript, l'analyse, les notions et les citations, et je relie tout.
