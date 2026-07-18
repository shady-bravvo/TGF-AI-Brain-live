---
type: moc
tags: [moc, ai-brain, TGF2026]
---
# 🧠 TGF AI Brain

> Objectif : transformer les talks du [[TGF 2026 - Tunisia Global Forum]] en **base de connaissances vivante** — transcripts liés aux sessions et speakers, puis distillés en notions, citations et insights actionnables (au service du [[Livre Blanc IA Tunisie]] et de la stratégie IA Tunisie).

## 🔄 Le pipeline en 4 étapes

### 1️⃣ Ingestion — un transcript par talk
Crée une note dans `09 Transcripts/` avec le template [[Template - Transcript]].
Nommage : `Transcript - <Session courte> - <Speaker principal>`.
Remplis le frontmatter : `session`, `speakers`, `statut: brut`.

### 2️⃣ Liaison — connecter au graphe
Le frontmatter + les wikilinks relient automatiquement le transcript à sa session ([[Cérémonie d'ouverture TGF 2026]], plénières, talks…) et à ses speakers. Ajoute le lien retour « Transcript » dans la note de session.

### 3️⃣ Extraction — analyse structurée
Passe le transcript au crible avec le [[Prompt d'analyse TGF AI Brain]] (via Claude/Cowork). L'analyse produit dans la note du transcript :
- **Notions** → chaque concept important devient une note atomique dans `10 Analyse/Notions/` ([[Template - Notion]])
- **Phrases clés** → verbatims courts à fort signal
- **Citations** → les meilleures deviennent des notes dans `10 Analyse/Citations/` ([[Template - Citation]])
- **Chiffres & faits** · **Recommandations & actions** · **Questions ouvertes**
Passe alors `statut: analysé`.

### 4️⃣ Distillation — synthèses transverses
Dans `10 Analyse/Synthèses/` ([[Template - Synthèse]]) : croiser les transcripts par thème ([[IA & Souveraineté]], [[Talents & Transformations]]…), faire émerger consensus, désaccords et priorités → nourrir le [[Livre Blanc IA Tunisie]].

## 📊 Tableaux de bord (plugin Dataview requis)

### Transcripts à analyser
```dataview
TABLE session, speakers, date FROM "09 Transcripts" WHERE statut = "brut" SORT date
```
### Transcripts analysés
```dataview
TABLE session, speakers FROM "09 Transcripts" WHERE statut = "analysé"
```
### Notions par fréquence de mention
```dataview
TABLE length(file.inlinks) AS "Mentions" FROM "10 Analyse/Notions" SORT length(file.inlinks) DESC
```
### Citations par speaker
```dataview
TABLE speaker, session FROM "10 Analyse/Citations" SORT speaker
```

## ⚙️ Configuration recommandée (une fois)
1. **Plugins communautaires** à installer : `Dataview` (tableaux de bord ci-dessus), `Templater` (optionnel, templates dynamiques).
2. **Templates** : Réglages → Modèles → dossier = `99 Templates` (déjà préconfiguré).
3. **Graphe** : groupes de couleurs préconfigurés (speakers, sessions, notions, citations, transcripts…). Filtre utile : `tag:#notion OR tag:#transcript` pour voir uniquement le cerveau analytique.

## 🚀 Démarrage rapide
Exemple complet à copier : [[Transcript - EXEMPLE - Plénière Stratégique]] et la notion [[Souveraineté des données]] qui en découle.

Retour à la carte : [[00 Accueil]]
