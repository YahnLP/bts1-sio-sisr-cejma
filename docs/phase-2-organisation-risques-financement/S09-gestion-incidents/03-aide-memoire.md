# Aide-mémoire – Incident, priorité, SLA, MTTR, disponibilité

*BTS SIO SISR 1re année – CEJMA – S09*

> Un mot ou un sigle inconnu ? Passe la souris dessus, ou ouvre le [glossaire](../../ressources/glossaire.md).

## Vocabulaire

| Terme | Sens |
|---|---|
| **Incident** | Interruption ou dégradation non prévue |
| **Problème** | Cause d'un ou plusieurs incidents |
| **Demande** | Besoin prévu et standard |
| **Changement** | Modification du système |

## Processus

**Enregistrer → classer → prioriser → diagnostiquer → (escalader) → rétablir → clôturer → capitaliser.**

## Priorité

| Impact ↓ / Urgence → | Haute | Moyenne | Basse |
|---|---|---|---|
| Élevé | P1 | P2 | P3 |
| Moyen | P2 | P3 | P4 |
| Faible | P3 | P4 | P4 |

## Engagements

**SLA** = accord de niveau de service. **GTI** = délai de prise en charge. **GTR** = délai de rétablissement. Heures **ouvrées** = heures d'ouverture du service.

## Formules

- **Taux de respect du SLA** = tickets dans les délais ÷ tickets × 100.
- **MTTR** = somme des durées de rétablissement ÷ nombre d'incidents.
- **MTBF** = durée de fonctionnement ÷ nombre de pannes.
- **Disponibilité** = (total − arrêt) ÷ total = **MTBF ÷ (MTBF + MTTR)**.
- **Courbe à 80 %** : coût × 0,8 à chaque doublement de la production cumulée.

## Incident majeur

Cellule de crise, responsable, porte-parole, communication ; **retour d'expérience** sans chercher de coupable.

## Pièges

- Prendre une **demande** pour un **incident**.
- Fonder une décision sur le seul **MTTR** : un ticket extrême fausse la moyenne.
- Oublier de **clôturer avec l'utilisateur**.
