---
type: doc
tags: [interne, rendus, TGF2026]
---
# 📦 00 Rendus — mode d'emploi

> Tous les rendus du jour J vivent ici. **Principe : rien ne se crée le jour J, tout se remplit.** Chaque rendu a été testé sur le contenu actuel du vault (transcript exemple inclus).

## Contenu du dossier

| Fichier | Quoi | Comment il se met à jour |
|---|---|---|
| `dashboard.html` | Dashboard + nuage de tags, charte TGF (bleu nuit / rouge Tunisie) | `python3 generate_dashboard.py` (dans `_INTERNE .../pipeline/`) — à relancer après chaque lot de notes |
| `dashboard-data.json` | Les chiffres bruts (KPIs, tags, sessions, citations) | Généré en même temps — sert aussi à remplir le recap et la slide chiffres |
| `Recap - TGF 2026.md` | Gabarit du recap — zones `[À INSÉRER]` | Rempli à 14h (content freeze), relu par l'éditeur |
| `Feuille de route - TGF 2026.md` | Gabarit roadmap par thème + 5 priorités | v1 à 14h, consolidée en fin de journée |
| `Presentation 15h - TGF AI Brain.pptx` | Deck de la démo 15h (8 slides, notes speaker avec timing) | Zones **JOUR J** en ambre : recap, chiffres, questions chatbot, QR codes. Régénérable via `pipeline/build_deck_15h.js` (`node build_deck_15h.js`) |

## Checklist avant 15h (extrait du runbook)

- [ ] 14h00 — content freeze : `generate_dashboard.py` une dernière fois
- [ ] Copier les chiffres de `dashboard-data.json` dans la slide 4 et le recap
- [ ] Coller les 3 messages clés + verbatims dans le recap et la slide 3
- [ ] Insérer les 3 questions chatbot testées à 14h30 (slide 7)
- [ ] QR codes chatbot + site insérés (à faire dès J-3 quand les URLs sont figées)
- [ ] Onglets navigateur préparés : dashboard plein écran + graphe
- [ ] Répétition éclair : bascules slide 5 → dashboard et slide 6 → graphe

## À décider / faire encore

- URL définitive du site (bloque les QR codes) — question ouverte ATUGE
- Le nuage de tags reflète pour l'instant les liens du programme pré-rempli ; il prendra vie avec les vrais transcripts
- Ce dossier est exclu du parsing du dashboard (pas de boucle) mais **sera publié par Quartz** sauf exclusion explicite — à trancher avant J-3
