# Assistant IA d'orientation face à l'AVC : dépôt de travail

Projet individuel de 8 semaines. Auteure : Yasmine Gorrab. Dépôt : https://github.com/MiiN1136/AVC_MR2. Domaine : accident vasculaire cérébral (AVC), contexte tunisien. Données publiques.

## Structure

| Dossier | Contenu |
|---|---|
| `00-cadrage/` | Fiche de cadrage, trois cadrages comparés, note « PRISMA avec mes mots » |
| `01-revue/` | Protocole PRISMA-P, correspondance avec la checklist, équations versionnées, exports, criblage, extraction |
| `02-code/` | Code de l'assistant et des évaluations |
| `03-base-de-connaissances/` | Sources officielles retenues, avec date de consultation |
| `04-assistant/` | Instructions, règles de sécurité, scénarios de test |
| `05-journal-usage-ia/` | Annexe B, une ligne par usage significatif |
| `06-comptes-rendus/` | Un compte rendu par semaine (annexe A) |

## État au 14/11/2026

Protocole v1.2 ; équation PubMed finale `eq4` figée (**82 résultats** avec limites `2010:2026[dp]` et `en/fr` ; **4/5 sentinelles** retrouvées) ; texte exact des équations (`01-revue/equations/equations_testees.md`), captures et journal des recherches (`01-revue/equations/journal_recherches.csv`) à jour. Prochaine étape : export PubMed vers Zotero, exécution des autres bases (Scopus, CENTRAL, IEEE Xplore, IMEMR/AIM) et début du criblage.

## Règles

- Tout changement du protocole après le 14/11/2026 est inscrit dans `01-revue/CHANGELOG_protocole.md` (date, justification).
- Chaque équation de recherche est versionnée et son nombre de résultats noté dans `01-revue/equations/journal_recherches.csv`.
- Tout élément produit par l'IA est vérifié avant conservation et tracé dans le journal.
