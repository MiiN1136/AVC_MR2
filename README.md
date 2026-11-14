# Assistant IA d'orientation face à l'AVC : dépôt de travail

Projet individuel de 8 semaines. Auteure : Yasmine Gorrab. Dépôt : https://github.com/MiiN1136/AVC_MR2. Domaine : accident vasculaire cérébral (AVC), contexte tunisien. Données publiques ou synthétiques uniquement.

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

Protocole v1.1 ; équation PubMed eq4 retenue provisoirement ; à compléter : texte exact des équations (`01-revue/equations/equations_testees.md`), vérification des sentinelles, dates des recherches (`journal_recherches.csv`).

## Règles

- Tout changement du protocole après le 14/11/2026 est inscrit dans `01-revue/CHANGELOG_protocole.md` (date, justification).
- Chaque équation de recherche est versionnée et son nombre de résultats noté dans `01-revue/equations/journal_recherches.csv`.
- Tout élément produit par l'IA est vérifié avant conservation et tracé dans le journal.

## Mise en place Git

```
git init
git add .
git commit -m "Semaine 1 : cadrage et protocole v1.0"
git remote add origin https://github.com/MiiN1136/AVC_MR2
git push -u origin main
```
Puis donner l'accès en lecture à l'encadrant.
