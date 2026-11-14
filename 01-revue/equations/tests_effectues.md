# Tests de recherche PubMed (captures dans `captures/`)

Les nombres ci-dessous ont été lus sur les captures d'écran. **Aucune limite de date ni de langue n'était appliquée** (les histogrammes remontent avant 2010) : les nombres avec les limites du protocole (2010:2026, anglais ou français) restent à relever. Le texte exact de chaque équation est tronqué sur les captures : il est à coller dans `equations_testees.md` depuis l'historique PubMed (Advanced > History and Search Details).

## 1. Équations testées

| Essai | Nb | Ce que montrent les 10 premiers titres | Verdict |
|---|---|---|---|
| v0 et v1 avec filtre « Associated data » | 18 031 et 10 | Filtre non prévu au protocole | Invalides |
| eq1_1 (v1 sans filtre) | 2 025 | Rééducation, télé-AVC, adhésion médicamenteuse, TikTok, soins de transition ; très peu d'éducation à la reconnaissance | Trop bruyante |
| eq2 | 1 466 | Presque uniquement rééducation et cliniques post-AVC (orthèses, aphasie, déficience visuelle) | Rejetée : hors périmètre |
| eq3 | 69 | Revues et recommandations sur la prise en charge pré-hospitalière, campagnes publiques (revue de Tan 2022), application pour enfants, éducation aux urgences ; bruit : unités mobiles AVC, traumatologie | Précise mais dominée par des revues et des textes d'organisation |
| **eq4** | **87** | Surtout des travaux sur la connaissance de l'AVC : enquêtes (Thaïlande, Soudan, Arabie saoudite), application pour enfants, éducation numérique, vidéo en téléconférence ; peu de bruit | **Retenue provisoirement** : thème juste, volume lisible |
| eq5 | 306 | Rétinopathie hypertensive, prédiction par apprentissage automatique, rééducation : cause probable `knowledge[tiab]` | Rejetée : bruit |

**Choix provisoire : eq4.** Pourquoi : meilleur compromis entre pertinence thématique et volume (87 références se criblent en une séance). Réserve : beaucoup de résultats sont des enquêtes transversales **sans intervention**, qui seront exclues au criblage par le critère « intervention numérique » ; c'est normal, l'équation capte le thème.

## 2. Recherches ciblées de contrôle

| Recherche | Nb | Constat |
|---|---|---|
| « stroke awareness » AND vidéo en ligne… (r1) | 1 | Cherfane 2025 (EAU) : avant-après sur 407 adultes, connaissance de l'AVC passée de 20,80 à 23,53 (p < 0,001) |
| « stroke symptom recognition » AND application… (r2) | 1 | Seulement une revue narrative non éligible : la combinaison est très rare |
| stroke AND agents conversationnels, ChatGPT… (r3) | 62 | Seulement 2 titres proches sur 10 : Vora 2023 (ChatGPT et sensibilisation à l'AVC ischémique), Qiang 2025 (grands modèles de langage et éducation en rééducation). **Preuves sur les agents conversationnels très minces**, ce qui confirme le choix d'élargir l'intervention |
| stroke AND délai pré-hospitalier, SAMU… (r4) | 113 | Enquêtes, revues ; l'étude d'Oostema 2019 vise les équipes de secours (exclue : professionnels) |
| stroke AND Tunisie, Maghreb, MENA… (r5) | 50 | Bruit : rapports mondiaux de morbidité. Termes régionaux inutiles dans l'équation |
| stroke symptom recognition app (r6) | 10 | Surtout hors sujet (encéphalite, Alzheimer) ; outils de tri (FAST-ED) et applications de dépistage, pas d'éducation |
| stroke awareness tunisia (r7) | 8 | Deux sources de contexte : Roushdy 2025 (17 pays africains) et l'étude CAP de Tunis (Aounallah Skhiri, Tunis Med 2005, avant 2010 : hors période) |

## 3. Vérification des sentinelles

Requête de contrôle exécutée le 14/11/2026 sur `eq4` avec les 5 PMID sentinelles (`AND (40771970[pmid] OR 38841682[pmid] OR 39482602[pmid] OR 35334251[pmid] OR 20434048[pmid])`) :
- **Score : 4/5 sentinelles retrouvées** : Iskandar 2024 (`38841682`), Safwan 2024 (`39482602`), Cherfane 2025 (`40771970`) et Chan 2010 (`20434048`).
- **Sentinelle manquante (1/5) :** Shufflebarger et al., 2022 (`35334251`), car le résumé utilise « CDC video » / « video » et non les expressions exactes `"online video"` ou `"educational video"` du bloc 2. Elle sera repérée par le contrôle des listes de références et les autres bases (Scopus, CENTRAL (recherches a effectuer dans le futur)).

## 4. Enseignements et figement de l'équation PubMed

- Peu de vraies études d'intervention : plusieurs avant-après à groupe unique, des enquêtes transversales et des protocoles. D'où l'amendement v1.1 du protocole (acceptation des avant-après à groupe unique, plan de repli vers une revue exploratoire si < 5 études éligibles).
- Existence d'une revue proche (Tan 2022, PMID 34844126) : à positionner, et ses références à contrôler.
- **Exécution finale avec limites du protocole :** `eq4` relancée le 14/11/2026 avec `2010:2026[dp]` et `english[la] OR french[la]` donne **82 résultats**, soit 5 références écartées par rapport aux 87 résultats sans filtre. L'équation `eq4` est figée comme équation PubMed finale (amendement v1.2).
