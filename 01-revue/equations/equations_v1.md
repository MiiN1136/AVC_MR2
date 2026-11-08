# Équations de recherche, version v1 (non encore exécutées)

**Statut : brouillon.** Rien ici n'a encore été lancé dans une base. Les nombres de résultats sont à renseigner par l'auteur après exécution.

## Procédure de test (à faire avant de figer le protocole)

1. Constituer 5 à 10 **articles sentinelles** trouvés à la main (hors équation) sur l'éducation à l'AVC par outil numérique.
2. Lancer l'équation ; vérifier que **tous les sentinelles** sont retrouvés. Sinon, ajouter les termes manquants (v2).
3. Lire les titres des 50 premiers résultats ; estimer la proportion hors sujet et en identifier la cause (ex. `stroke` au sens de « stroke volume », `app[tiab]`).
4. Valider chaque descripteur MeSH dans le MeSH Browser (existence, orthographe, arborescence).
5. Adapter la syntaxe aux autres bases et noter dans `journal_recherches.csv`.

## Journal à remplir (`journal_recherches.csv`)

```
base,date,version,equation_fichier,limites,nb_resultats,sentinelles_retrouves,remarques
PubMed,,v1,pubmed_v1.txt,2010:2026 ; en/fr,,/,
Scopus,,v1,scopus_v1.txt,2010-2026 ; en/fr,,/,
CENTRAL,,v1,central_v1.txt,2010-2026,,/,
IEEE Xplore,,v1,ieee_v1.txt,2010-2026,,/,
IMEMR / AIM,,v1,regional_v1.txt,,,/,
```

## Adaptations prévues

- **Scopus** : `TITLE-ABS-KEY(...)` avec les mêmes blocs de mots libres ; pas de MeSH, donc ajouter des synonymes (`"brain attack"`, `"cerebrovascular"`).
- **CENTRAL** : blocs 1, 2 et 3 en mots libres, filtre « essais ».
- **IEEE Xplore** : bloc 1 AND bloc 3 (volet technique), sans bloc éducation.
- **IMEMR / African Index Medicus** : équation courte (`stroke AND (education OR awareness)`), interface limitée.

## Risques connus de l'équation v1

- Bloc 4 trop large (`knowledge[tiab]`) : bruit probable, à resserrer en v2 si le tri est trop lourd.
- `educat*` et `awareness` : forte sensibilité, faible précision.
- Les agents conversationnels récents peuvent être indexés sous des termes non prévus (« generative AI », « ChatGPT ») : à ajouter si les sentinelles manquent.
