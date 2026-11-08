# Fiche de cadrage : assistant IA d'orientation face aux signes d'un AVC

**Auteur :** [Prénom NOM] · **Date :** 08/11/2026 · **Domaine attribué :** accident vasculaire cérébral (AVC)

## 1. Périmètre

L'assistant couvre **la phase pré-hospitalière de l'AVC de l'adulte** : reconnaître les signes d'alerte (repères de type FAST / VITE), comprendre qu'il s'agit d'une urgence, appeler le SAMU (190, à vérifier dans une source officielle tunisienne avant intégration) et savoir quoi dire et quoi éviter en attendant les secours. Il fournit aussi une information de base sur les facteurs de risque (hypertension, diabète, tabac, fibrillation atriale). La langue de la première version est le français ; l'arabe est prévu plus tard.

## 2. Utilisateurs visés

Adultes du grand public en Tunisie, et surtout les **proches et aidants de personnes à risque** (âgées, hypertendues, diabétiques), qui sont souvent les premiers témoins. Les professionnels de santé ne sont pas la cible.

## 3. Problème à résoudre

Les traitements de reperfusion de l'AVC ischémique ne sont possibles que dans une fenêtre de temps limitée : tout retard d'appel réduit les chances de traitement. Or une enquête multicentrique menée aux urgences du centre et du sud de la Tunisie conclut à un besoin urgent d'améliorer les connaissances de la population sur l'AVC (Rekik et al., *Stroke knowledge among emergency centre visitors*, PMC7724164), et les auteurs notent que le délai entre le début des signes et l'admission reste long. Le projet cherche si un assistant conversationnel peut raccourcir l'étape « reconnaître et appeler ».

## 4. Trois cas d'usage

1. **Reconnaissance en situation :** un proche a le visage qui tombe et la parole confuse. L'assistant pose 3 ou 4 questions fermées, affiche « appelez le 190 maintenant », demande et rappelle l'heure de début des signes.
2. **Préparer l'appel :** l'utilisateur demande quoi dire au SAMU. L'assistant fournit une liste courte (adresse, heure de début, traitements en cours, état de conscience).
3. **Prévention et culture du risque :** une personne hypertendue demande quels signes surveiller. L'assistant répond à partir d'une base de connaissances fermée, avec la source citée.

## 5. Exclusions volontaires (et raison de chacune)

| Exclu | Raison |
|---|---|
| Diagnostic ou tri médical individuel | Risque de faux négatif, responsabilité médicale, logiciel assimilable à un dispositif médical |
| Aide à la décision pour cliniciens (thrombolyse) | Exige des données de patients, une validation clinique et un accord éthique, hors de portée en 8 semaines |
| Rééducation et suivi post-AVC | Domaine distinct, trop vaste pour une revue et un assistant de qualité |
| Analyse d'imagerie (scanner, IRM) | Autre compétence (vision), données non publiques |
| AVC de l'enfant, hémorragie sous-arachnoïdienne | Parcours et signes différents, base documentaire séparée |
| Arabe dialectal en v1 | Ressources et jeux d'évaluation insuffisants ; reporté, documenté comme limite |
| Toute donnée de patient | Contrainte du projet : données publiques ou synthétiques uniquement |

## 6. Risques et limites de l'assistant

- **Fausse réassurance** : l'assistant ne dit jamais « vous n'avez pas d'AVC » ; au moindre doute, il oriente vers le 190. On accepte volontairement une sur-alerte (hypoglycémie ou migraine peuvent imiter un AVC).
- **Hallucination** : réponses limitées à une base de connaissances fermée (sources officielles), avec refus quand l'information manque.
- **Numéros et procédures erronés** : tout numéro d'urgence et toute consigne sont vérifiés à la source avant publication.
- **Équité d'accès** : fracture numérique, littératie, langue ; l'assistant complète les campagnes de sensibilisation sans les remplacer.
- **Confidentialité** : aucune conservation de données personnelles ; aucun test avec de vraies personnes en situation d'urgence.
- **Preuves incertaines** : la littérature sur les agents conversationnels pour l'AVC peut être mince, d'où une revue élargie aux outils numériques d'éducation (voir protocole).
