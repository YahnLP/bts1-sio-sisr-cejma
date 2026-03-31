---
author: YLP
title: 📄 ANNEXE 1
---

# 📚 FICHE DE COURS ÉLÈVE
## RGPD (4) : Contrôle & Sanctions — Pouvoirs de la CNIL et Risques Financiers

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 10 — CEJMA*

---

## 📖 PARTIE III — Les Sanctions RGPD

### III.A. Les 2 Types de Sanctions

Le RGPD prévoit **2 types de sanctions** :

#### 1. Sanctions Administratives (Article 83)

Prononcées par la **CNIL** (autorité administrative).

**Types de sanctions administratives :**

| **Sanction** | **Description** | **Exemple** |
|---|---|---|
| **Avertissement** | Rappel à l'ordre sans amende | "Vous devez corriger sous 3 mois" |
| **Mise en demeure** | Injonction de se conformer | "Désignez un DPO sous 2 mois" |
| **Limitation temporaire** | Suspension d'un traitement | "Arrêtez le profilage publicitaire" |
| **Suspension des flux** | Interdiction de transférer des données | "Arrêtez les transferts vers les USA" |
| **Amende administrative** | **Sanction pécuniaire** | De 10 000 € à 20 millions € |
| **Injonction de cesser** | Arrêt définitif d'un traitement | "Fermez ce fichier illégal" |

#### 2. Sanctions Pénales (Code Pénal)

Prononcées par un **tribunal pénal**.

**Infractions pénales liées au RGPD :**

| **Infraction** | **Article Code Pénal** | **Peine** |
|---|:---:|---|
| **Collecte de données par moyens frauduleux** | 226-18 | 5 ans + 300 000 € |
| **Conservation excessive de données** | 226-20 | 5 ans + 300 000 € |
| **Violation du secret professionnel** | 226-13 | 1 an + 15 000 € |
| **Détournement de finalité** | 226-21 | 5 ans + 300 000 € |
| **Atteinte à un système informatique** (en lien RGPD) | 323-1 | 2 ans + 60 000 € |

> ⚠️ **Attention :** Les sanctions pénales peuvent être **cumulées** avec les amendes administratives.

---

### III.B. Calcul de l'Amende Administrative

Le RGPD prévoit **2 niveaux d'amendes maximales** :

#### Niveau 1 : Maximum 10 millions € OU 2% du CA mondial

**Violations concernées :**
- Absence de registre des traitements (art. 30)
- DPO non désigné alors qu'obligatoire (art. 37)
- Absence d'AIPD pour traitement à risque (art. 35)
- Sous-traitant qui ne respecte pas les instructions du RT (art. 28)

#### Niveau 2 : Maximum 20 millions € OU 4% du CA mondial

**Violations concernées :**
- Violation des principes fondamentaux (art. 5-6)
- Non-respect des droits des personnes (art. 15-22)
- Absence de consentement (art. 7)
- Défaut de sécurité (art. 32)
- Non-notification de violation (art. 33-34)
- Transfert illicite de données hors UE (art. 44-49)

**Règle de calcul :**

```
Amende maximale = LE PLUS ÉLEVÉ DE :
- 20 millions € (montant fixe)
- 4 % du chiffre d'affaires annuel mondial de l'exercice précédent
```

**Exemples de calculs :**

| **Entreprise** | **CA Mondial** | **4% du CA** | **Maximum applicable** |
|---|---|---|---|
| PME (CA 5M€) | 5 000 000 € | 200 000 € | **20 millions €** (montant fixe) |
| ETI (CA 100M€) | 100 000 000 € | 4 000 000 € | **20 millions €** (montant fixe) |
| Google (CA 300Mds$) | 300 000 000 000 $ | 12 000 000 000 $ | **12 milliards $** (4% CA > 20M€) |

> 💡 **En pratique :** La CNIL ne prononce **jamais le maximum**. Elle applique des critères de modulation (voir ci-dessous).

---

### III.C. Critères de Modulation de l'Amende (Article 83-2)

La CNIL évalue **11 critères** pour déterminer le montant de l'amende :

| **Critère** | **Question Posée** | **Impact sur l'Amende** |
|---|---|---|
| **1. Nature, gravité, durée** | Violation grave ? Combien de temps ? | ↑ Plus c'est grave/long, plus l'amende augmente |
| **2. Caractère intentionnel** | Négligence ou mauvaise foi ? | ↑ Mauvaise foi → amende élevée |
| **3. Mesures prises** | L'organisme a-t-il corrigé rapidement ? | ↓ Corrections rapides → amende réduite |
| **4. Coopération avec CNIL** | L'organisme a-t-il collaboré ? | ↓ Bonne coopération → amende réduite |
| **5. Catégories de données** | Données sensibles ? Enfants ? | ↑ Santé, enfants → amende élevée |
| **6. Nombre de personnes concernées** | 100 ou 10 millions ? | ↑ Plus il y a de victimes, plus l'amende augmente |
| **7. Préjudice subi** | Dommages réels (financiers, moraux) ? | ↑ Préjudice important → amende élevée |
| **8. Notification à la CNIL** | Violation notifiée dans les 72h ? | ↓ Notification rapide → amende réduite |
| **9. Antécédents** | Déjà sanctionné ? | ↑ Récidive → amende multipliée |
| **10. Situation financière** | PME ou grande entreprise ? | ↓ PME en difficulté → amende adaptée |
| **11. Autres circonstances** | Contexte particulier ? | Variable |

**Exemple de modulation :**

```
Entreprise : Google Ireland
Violation : Cookies sans consentement
CA mondial : ~75 milliards €
Amende maximale théorique : 75 Mds × 4% = 3 milliards €

Mais la CNIL a prononcé 90 millions € car :
- Gravité : Élevée mais pas maximale (pas de fuite de données)
- Coopération : Moyenne (corrections partielles)
- Antécédents : Déjà sanctionné en 2020 (aggravant)
- Mesures : Prises tardivement

Résultat : 90M€ = 0,12% du CA (bien en dessous du maximum)
```

---

### III.D. Publication des Sanctions

**Principe :** Toutes les sanctions CNIL sont **publiques** (art. 83-4-h).

**Modalités :**
- Publication sur le site [cnil.fr](https://www.cnil.fr/fr/les-sanctions)
- Nom de l'organisme sanctionné (sauf exception)
- Montant de l'amende
- Résumé des manquements

**Impact :**
- ❌ **Réputationnel** : atteinte à l'image de marque
- ❌ **Commercial** : perte de confiance des clients
- ❌ **Juridique** : risque de class action (recours collectif)

---

![Schéma des critères de modulation : balance avec d'un côté "Critères aggravants" (gravité, mauvaise foi, antécédents, nombre de victimes) et de l'autre "Critères atténuants" (coopération, mesures prises, notification rapide). Au centre : montant de l'amende.]

*Légende : Les critères de modulation de l'amende CNIL*

---