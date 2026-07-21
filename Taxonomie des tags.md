---
type: officiel
tags: [officiel, ai-brain, TGF2026]
---
# Taxonomie des tags - TGF AI Brain

> **Liste FERMÉE.** Les agents (Obelyx, Claude, Cowork) n'utilisent que ces tags. Tout nouveau thème passe par `#theme-propose`, validé par l'éditeur. Aucun tag inventé, aucun synonyme, aucun pluriel alternatif.

## 1. Tags de structure (qui est quoi)

*Un par note, ils colorent le graphe.*

| Tag | Usage |
|---|---|
| `#personne` | Tout être humain mentionné dans le vault |
| `#speaker` | En PLUS de `#personne`, si la personne intervient au TGF |
| `#organisation` | Entreprise, institution, association, université |
| `#partenaire` | En PLUS de `#organisation`, si partenaire/sponsor du TGF |
| `#evenement` | TGF (éditions) et side events (hackathon, awards, networking) |
| `#session` | Un créneau de prise de parole du programme |
| `#lieu` | Salle ou espace physique |
| `#theme` | Note thématique de référence (dossier `07 Thèmes`) |
| `#livre-blanc` | Notes du Livre Blanc IA Tunisie |
| `#livrable` | Documents produits par le projet (`00 Rendus`) |
| `#officiel` | Documents de référence validés (programme, taxonomie, règles) |

## 2. Tags de nature du propos (fabriquent les livrables)

*Posés sur les notes d'extraction (`10 Analyse`) : 1 tag de nature + wikilinks session/speaker/thème.*

| Tag | Usage | Alimente |
|---|---|---|
| `#citation` | Verbatim exact, attribué | Recap, com, site |
| `#chiffre` | Donnée chiffrée citée | Dashboard, recap |
| `#annonce` | Annonce concrète faite sur scène | Recap, moments forts |
| `#constat` | État des lieux, diagnostic | Recap, thèmes |
| `#recommandation` | Ce qu'il FAUDRAIT faire selon un intervenant | **Feuille de route** |
| `#action-proposee` | Action concrète avec porteur identifiable | **Feuille de route** |
| `#controverse` | Désaccord entre intervenants | Recap (débats) |
| `#question-ouverte` | Question restée sans réponse | Feuille de route (à creuser) |

**Règle feuille de route** : `#recommandation` + `#action-proposee` au statut `#verifie`, groupées par axe du [[Livre Blanc IA Tunisie]], sinon par thème.

## 3. Tags de statut éditorial (workflow interne, jamais publiés)

| Tag | Signification | Qui le pose |
|---|---|---|
| `#brut` | Sorti du transcript, non relu | Agent |
| `#traite` | Structuré et lié (session, speaker, thème) | Agent |
| `#verifie` | Relu : noms, chiffres, citations exacts | Éditeur |
| `#publie` | Autorisé sur le site et en démo | Éditeur |
| `#exclu` | Hors publication (demande speaker, Chatham House) | Éditeur |

**Content freeze 14h** : seul `#verifie` peut passer `#publie`. Une citation nominative n'est jamais `#publie` sans vérification humaine.

## 4. Tag de proposition

| Tag | Usage |
|---|---|
| `#theme-propose` | Contenu qui ne rentre dans aucun thème existant. L'éditeur tranche à 14h : création ou fusion. |

## Règles pour les agents

1. Tags autorisés : uniquement ceux de ce document. Liste fermée.
2. Une note d'extraction = 1 tag de nature + 1 tag de statut + wikilinks `[[Session]]`, `[[Speaker]]`, `[[Thème]]`.
3. Personnes, organisations, sessions et thèmes = **wikilinks vers leurs notes**, jamais des tags.
4. Ne jamais créer une note de thème : utiliser `#theme-propose` sur la note d'extraction.
5. Ne jamais poser `#verifie`, `#publie` ou `#exclu` : réservés à l'éditeur.
6. Doute sur une attribution → rester en `#brut` et le signaler.

## Graphe : le système de couleurs est configuré

Les 22 groupes sont dans les réglages du graphe (ordre = priorité, premier match gagne). Logique :

- **Gris** = pas encore montrable (`#brut`, `#exclu`). `#traite`/`#verifie`/`#publie` ne sont pas colorés : dès qu'une note sort de `#brut`, sa couleur de nature s'affiche.
- **Violet** (`#recommandation`, `#action-proposee`) = la feuille de route qui se construit.
- **Or** (`#annonce`) = les annonces du jour.
- **Entités** = la palette existante (speakers cyan, thèmes rouge, sessions vert, partenaires magenta, livre blanc jaune...).

**Vue scène (projetée à 15h)** - filtre à coller dans la barre de recherche du graphe :
```
-tag:#brut -tag:#traite -tag:#exclu -tag:#livrable -tag:#officiel -path:"99 Templates" -file:Untitled
```
