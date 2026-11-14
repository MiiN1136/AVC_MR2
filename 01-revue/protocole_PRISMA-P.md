# Annexe C. Protocole de revue (PRISMA-P)

**Version :** v1.2 du 14/11/2026 (v1.0 : première rédaction ; amendements v1.1 et v1.2 listés dans `CHANGELOG_protocole.md`). Après cette date, toute modification est inscrite dans `CHANGELOG_protocole.md` avec date et justification.

| Rubrique | Contenu |
|--|----------|
| Titre et domaine | *Protocole d'une revue systématique : interventions numériques d'éducation (applications, SMS, agents conversationnels, IA) pour améliorer la reconnaissance de l'AVC et réduire le délai pré-hospitalier chez les adultes.* Domaine : accident vasculaire cérébral. Auteure : Yasmine Gorrab (yasminegorrab1@gmail.com). Date : 14/11/2026. Protocole non enregistré (projet académique d'un semestre, sans enjeu de publication) ; sa version est horodatée par l'historique Git du dépôt. |
| Question de recherche (PICO) | Chez les **adultes** du grand public, patients à risque d'AVC ou aidants (P), les **interventions numériques d'éducation** (applications, SMS, web, vidéo, agents conversationnels, IA) (I), comparées à l'absence d'intervention ou à l'éducation usuelle (campagne classique, support papier) (C), améliorent-elles la **reconnaissance des signes d'AVC, l'intention ou le comportement d'appel d'urgence et le délai avant l'arrivée à l'hôpital** (O) ? |
| Objectifs | (1) Décider quels formats, canaux et contenus l'assistant doit retenir ; (2) choisir les indicateurs d'évaluation de l'assistant (semaines suivantes) ; (3) relever les risques de sécurité déjà rapportés pour les agents conversationnels ; (4) repérer les lacunes de preuves pour la Tunisie et la région MENA. |
| Critères d'inclusion | **Types d'études :** principal = essais randomisés, quasi-expérimentaux, avant-après avec comparateur, cohortes comparatives, et (amendement v1.1) études avant-après à groupe unique, classées comme quasi-expérimentales et analysées dans une strate à part ; secondaire = études non comparatives de développement ou d'évaluation d'utilisabilité d'agents conversationnels ou d'IA pour l'AVC (analysées à part). **Période :** 01/01/2010 jusqu'à la date de chaque recherche (généralisation des smartphones ; les modèles de langage ne datent que de 2022). **Langues :** français, anglais. **Population :** adultes ≥ 18 ans, tous pays ; le contexte tunisien et MENA est extrait comme critère de transposabilité, pas comme filtre, car les études locales sont rares. **Qualité minimale :** article revu par les pairs ; résultat chiffré rapporté sur au moins un critère de jugement. |
| Critères d'exclusion | Éditoriaux, lettres, avis, protocoles sans résultats (raison : pas de données ; leurs registres sont notés pour suivi) ; résumés de congrès (raison : information insuffisante pour apprécier la qualité) ; études sur professionnels de santé ou secouristes seulement (raison : population hors cible) ; interventions sans composante numérique (raison : hors intervention) ; AVC de l'enfant (raison : signes et parcours différents) ; études sans critère sur la reconnaissance, l'appel ou le délai (raison : hors résultat) ; doublons ; texte intégral introuvable après deux tentatives (raison : non évaluable, signalé comme limite). Langues autres que français et anglais, dont l'arabe (raison : capacité de relecture ; signalé comme limite). |
| Sources | PubMed/MEDLINE (exécutée le 14/11/2026) ; Scopus ; Cochrane CENTRAL ; IEEE Xplore (volet technique, agents conversationnels) ; IMEMR/WHO EMRO et African Index Medicus (contexte régional) ; ClinicalTrials.gov et ICTRP (essais en cours) ; Google Scholar, 200 premiers résultats (complément) ; littérature grise ciblée (OMS, World Stroke Organization, sociétés savantes, ministère de la Santé tunisien), utilisée pour le contexte et exclue des comptages principaux ; listes de références des revues pertinentes. **Date des autres recherches : à inscrire au moment de l'exécution (jj/mm/aaaa)** dans `equations/journal_recherches.csv`. |
| Équations de recherche | Voir `equations/equations_testees.md` et `equations/equations_v1.md`. Équation PubMed finale (`eq4`) : voir ci-dessous. Résultats obtenus : **PubMed : 82 (14/11/2026)** ; Scopus : [n] ; CENTRAL : [n] ; IEEE : [n] ; IMEMR : [n] (à renseigner après exécution des autres bases au cours des prochains livrables). Chaque modification crée une version (v2, v3…) avec son nombre de résultats. |
| Sélection | Deux étapes : (1) titres et résumés ; (2) textes complets. Gestion dans Zotero (dédoublonnage) et tableau de criblage versionné dans le dépôt. Relecteurs : moi (Yasmine Gorrab) comme relectrice principale ; un outil d'IA comme second relecteur indépendant sur **20 % des références tirées au hasard** à chaque étape. L'IA ne décide jamais seule : toute exclusion qu'elle propose est vérifiée par moi. L'encadrant peut relire le journal de criblage, mais aucune décision n'attend sa validation. Essai pilote sur 50 références pour clarifier les critères. Accord humain-IA mesuré par le kappa de Cohen ; seuil ≥ 0,60, sinon reformulation des critères et nouveau pilote. Désaccords tranchés par moi, avec la raison notée par écrit. |
| Extraction | Formulaire testé sur 3 études puis ajusté. Extraction par moi, vérifiée en double sur 20 % des études. Variables : référence, pays, année, devis, effectif, âge, niveau d'éducation, type d'intervention, langue, durée, contenu, comparateur, outils de mesure, résultats (connaissance, intention d'appel, délai en minutes, part arrivant avant 4,5 h), suivi, financement, effets indésirables ou erreurs de sécurité, limites, éléments de transposabilité (langue, accès au smartphone, organisation du SAMU) ; pour les outils d'IA : modèle, base de connaissances, évaluation de sécurité. |
| Qualité des études | **RoB 2** pour les essais randomisés ; **ROBINS-I** pour les études comparatives non randomisées ; **JBI (liste pour études quasi-expérimentales)** pour les études avant-après à groupe unique ; **MMAT 2018** pour les études non comparatives de développement ou à méthodes mixtes. Raison : ces outils couvrent les trois familles de devis attendues, avec une grille adaptée à chacune. Les études avant-après sans groupe de comparaison sont attendues à haut risque de biais et ne soutiennent pas de conclusion causale. Appréciation faite au niveau de l'étude et par critère de jugement principal. |
| Synthèse prévue | **Narrative structurée** (démarche SWiM), avec tableaux comparatifs par type d'intervention et par critère de jugement. Méta-analyse seulement si ≥ 3 études sont comparables sur le même critère et le même type d'intervention (modèle à effets aléatoires, hétérogénéité par I²) ; sinon pas de regroupement chiffré. Confiance dans les preuves appréciée par **GRADE** pour les critères principaux. |
| Décisions de conception | Voir la section dédiée ci-dessous. |
| Risques et limites | Biais de publication (les outils efficaces sont plus publiés) ; peu d'études tunisiennes et arabophones ; exclusion de l'arabe ; littérature IA/LLM très récente et en partie hors revue par les pairs ; critères de jugement hétérogènes (connaissance déclarée ≠ comportement réel) ; accès aux textes complets ; revue existante proche (Tan et al. 2022, campagnes publiques d'éducation à l'AVC), dont ma revue se distingue par le canal numérique et dont je contrôlerai la liste de références ; nombre d'études éligibles possiblement faible (voir plan de repli ci-dessous) ; relectrice principale unique, atténuée par le second criblage (IA) de 20 %. |

## Équation PubMed finale (eq4, figée le 14/11/2026 — 82 résultats)

```text
(
  "Stroke"[Mesh] OR stroke[tiab]
  OR "cerebrovascular accident"[tiab]
)
AND
(
  "online video"[tiab]
  OR "educational video"[tiab]
  OR "social media"[tiab]
  OR "digital campaign"[tiab]
  OR "web-based"[tiab]
  OR "mobile application"[tiab]
  OR "text message"[tiab]
  OR SMS[tiab]
  OR "e-learning"[tiab]
)
AND
(
  educat*[ti]
  OR awareness[ti]
  OR campaign*[ti]
  OR "stroke knowledge"[tiab]
  OR "symptom recognition"[tiab]
)
AND (2010:2026[dp])
AND (english[la] OR french[la])
```
