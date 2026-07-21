---
type: livre-blanc-axe
tags: [livre-blanc, axe, TGF2026]
axe: 2
theme: "[[Infrastructures numériques & énergétiques]]"
---
# ⚡ Axe 2 — Construire les capacités en infrastructures critiques nécessaires et frugales

Partie du [[Livre Blanc IA Tunisie]] · Thème : [[Infrastructures numériques & énergétiques]]

## Réalité de la Tunisie
**Énergie** : 5 944 MW installés (25 centrales, 19 395 GWh en 2024), mais **93,7 % de combustibles fossiles importés**. STEG : 92,1 % de la capacité, demande +5 %/an, risques de coupures estivales. Renouvelable : 787 MW en juin 2025 (240 éolien, 485 solaire, 62 hydraulique) soit **4,03 % du mix** ; appels d'offres pour 1 700 MW additionnels. MOU SoleCrypt–Schneider Electric (2025) : connectivité sous-marine vers l'Europe (latence <10 ms) ; potentiel théorique de **320 GW** solaire/éolien pour une pointe de 5 GW.

**Compute** : goulot d'étranglement mondial (Tony Blair Institute, State of Compute Access 2024). Décret-loi n°2023-17 : l'ANCS labellise les hébergeurs — pionnière africaine, 2ᵉ pays arabe (labels G-Cloud/N-Cloud, 7 acteurs N-Cloud, **aucun G-Cloud à ce jour**). Hubs émergents : Centre de Calcul Khawarezmi (1,3 pétaflops, 3ᵉ supercalculateur africain), Hub IA de Novation City (DGX NVIDIA, premier nœud GPU public d'Afrique du Nord), DGX à ESPRIT. Privé : Dataxion (seul Tier IV certifié), EO Datacenter (Tier III). Capacité souveraine totale très limitée et peu accessible.

**Connectivité** : >10 câbles sous-marins (IMEWE, SeaMeWe-4, Hannibal, Medusa…), latence <10 ms vers l'Europe ; 5G lancée en février 2025. Hydrogène vert : projet SoutH2 Corridor (gazoduc 3 500–4 000 km, jusqu'à 163 TWh/an) ; ELMED, première interconnexion électrique en courant continu Europe–Afrique du Nord (Sicile–Cap Bon, ~220 km, 600 MW).

## Benchmark
**Maroc** : leader nord-africain du renouvelable, 5,46 GW installés (2025 ; éolien 2,39 GW, solaire 0,95 GW), Noor Ouarzazate (510 MW), cible 52 % en 2030 ; Digital Maroc 2030, data centers Maroc Telecom/OCP, Huawei Cloud et Oracle. **Égypte** : 11,8 GW renouvelable (Benban 1,8 GW), principal hub de connectivité MENA, Equinix, nœuds AWS et Azure, masse critique de talents pour attirer les hyperscalers.

## Opportunités
- Potentiel solaire/éolien parmi les plus élevés d'Afrique du Nord (320 GW) ; infrastructure électrique couvrant quasi 100 % de la population
- Connexion au réseau européen (câble ELMED, $304,5M) ; SoutH2 ; connectivité sous-marine exceptionnelle
- Partenariat SoleCrypt–Schneider Electric pour data centers IA durables
- Supercalculateur HPC au CCK et Hub NVIDIA DGX opérationnel à Novation City
- Cadre réglementaire cloud pionnier

## Défis
- Dépendance critique au gaz importé (93,7 % fossile) ; objectif 35 % renouvelable en 2030 très ambitieux
- STEG en tension sur la pointe, risque de brownouts estivaux ; investissements énergie insuffisants ($3 Md vs $36 Md Égypte, 2021-2025)
- Absence de cadre PPA vert pour data centers IA ; pas de data center hyperscale certifié
- Capacité GPU souveraine fragmentée et non accessible à tous ; G-Cloud lent à se déployer ; pas de politique de compute souverain

## Recommandations (A2.1 → A2.11)
| # | Recommandation | Nature | Délai |
|---|---|---|---|
| A2.1 | **Green PPA data centers IA** — décret introduisant des contrats d'achat d'énergie renouvelable (PPA) dédiés aux opérateurs de data centers IA | réglementaire | 6 mois |
| A2.2 | **Classification infrastructure numérique prioritaire** — data centers IA = infrastructures critiques ; accès encadré à une alimentation fiable, conditionné à l'efficacité énergétique, la soutenabilité du réseau et la contribution aux renouvelables | réglementaire | 3 mois |
| A2.3 | **Régime fiscal data centers IA** — étudier un régime fiscal et douanier incitatif conditionné à l'investissement, l'emploi, l'efficacité énergétique et la valeur locale (ex. : exonération TVA + IS 7 ans pour investissements >10 MW ; 5 ans opérateurs certifiés) | réglementaire | 3 mois |
| A2.4 | **Étude de cadrage Compute National Souverain** — analyser les besoins réels (recherche, PME/startups, administrations) ; livrable : schéma directeur du compute souverain validé par la gouvernance de l'IA | organisationnelle | 6 mois |
| A2.5 | **Développement Cloud Souverain** — accompagner l'émergence d'acteurs labellisés G-Cloud pour les données publiques sensibles | organisationnelle | 6–12 mois |
| A2.6 | **Fonds Énergie-IA** — fonds souverain de co-investissement dédié à l'énergie renouvelable pour les infrastructures IA (data centers, HPC) | organisationnelle | 12 mois |
| A2.7 | **Comité National Infrastructure IA** — groupe de travail permanent au sein du CSIA ou d'une instance existante ; coordination STEG, INTT, ANCS, AFI + investisseurs privés ; mandat : appels d'offres data centers, politique GPU souverain, attractivité hyperscalers | organisationnelle | 3 mois |
| A2.8 | **Compute cluster national mutualisé, par paliers** — fédérer et étendre Novation City, CCK, ESPRIT en service national ouvert public/privé ; montée en charge selon les besoins ; ouverture négociée à tarifs préférentiels vers les plateformes internationales et/ou régionales maghrébines | opérationnelle | 18–36 mois |
| A2.9 | **Accélération des tenders solaires** — finaliser et raccorder les 1 700 MW en appel d'offres (2023-2025), en priorisant la proximité des futurs parcs de data centers | opérationnelle | 18 mois |
| A2.10 | **Data center pilote 100 % renouvelable** — projet PPP, emplacement à étudier | opérationnelle | 24 mois |
| A2.11 | **Appel d'offres international data centers** — data centers IA certifiés Tier III+, nombre et localisation à définir par une étude dédiée | opérationnelle | 12 mois |

## Liens
- Mesure phare associée : n°1 (Capacités d'énergie et de calcul par paliers) — voir [[Livre Blanc IA Tunisie]]
- [[LB Axe 3 - Données et modèles sectoriels]] (le compute au service des modèles)
