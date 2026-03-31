---
author: YLP
title: 📚 FICHE DE COURS
---

# 📚 FICHE DE COURS ÉLÈVE
## "RGPD (1) : Fondamentaux, Définitions et Droits"

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 6*

---

## 🎯 Objectifs

À la fin de cette séance, je serai capable de :

✅ Définir **donnée personnelle**, **traitement**, **consentement**  
✅ Expliquer les **6 principes fondamentaux** du RGPD  
✅ Connaître les **8 droits des personnes**  
✅ Identifier les **bases légales** d'un traitement  
✅ Traiter une **demande d'exercice de droits**  
✅ Appliquer le RGPD dans mon métier de technicien SISR

## 📚 Vocabulaire Juridique Clé

| **Terme** | **Définition** |
|-----------|----------------|
| **RGPD** | Règlement Général sur la Protection des Données (UE 2016/679) |
| **Donnée personnelle** | Information relative à une personne physique identifiée ou identifiable |
| **Traitement** | Toute opération sur des données personnelles (collecte, stockage, consultation...) |
| **Responsable de traitement** | Entité qui détermine les finalités et moyens du traitement |
| **Sous-traitant** | Entité qui traite des données pour le compte du responsable |
| **DPO** | Délégué à la Protection des Données (Data Protection Officer) |
| **CNIL** | Commission Nationale de l'Informatique et des Libertés (autorité française) |
| **Consentement** | Accord libre, spécifique, éclairé et univoque de la personne |

---

### 1️⃣ QU'EST-CE QU'UNE DONNÉE PERSONNELLE ?

### Définition Juridique (RGPD Art. 4.1)

> *"Toute information se rapportant à une personne physique **identifiée ou identifiable**."*

**Personne identifiable** = Personne qui peut être identifiée, directement ou indirectement.

---

### Les 2 Types d'Identification

```
┌────────────────────────────────────────────────┐
│ IDENTIFICATION DIRECTE                         │
│ (Permet d'identifier immédiatement)            │
├────────────────────────────────────────────────┤
│ • Nom et prénom                                │
│ • Email                                        │
│ • Photo / Vidéo du visage                      │
│ • Numéro de Sécurité Sociale                   │
│ • Empreinte digitale                           │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ IDENTIFICATION INDIRECTE                       │
│ (Croisement d'infos permet identification)    │
├────────────────────────────────────────────────┤
│ • Adresse IP                                   │
│ • Cookie / Identifiant unique                  │
│ • Login (ex: jdupont)                          │
│ • Plaque d'immatriculation                     │
│ • Coordonnées GPS                              │
│ • N° de téléphone                              │
└────────────────────────────────────────────────┘
```

**[ILLUSTRATION À INSÉRER]**
**Légende :** Schéma circulaire avec au centre une silhouette de personne. Autour, deux cercles concentriques : le cercle intérieur contient les identifiants directs (nom, email, photo), le cercle extérieur les identifiants indirects (IP, cookie, login). Flèches convergentes vers la personne centrale.

---

### Cas Particuliers

**⚠️ Adresse IP = Donnée Personnelle**
- Arrêt CJUE (Breyer, 2016) : IP = identifiant indirect
- Même IP dynamique = donnée perso (FAI peut relier à abonné)
- **Conséquence** : Logs serveur = traitement de données perso

**⚠️ Données Sensibles (Art. 9)**

Catégories **interdites par défaut** (sauf exceptions) :
- Origine raciale ou ethnique
- Opinions politiques
- Convictions religieuses
- Appartenance syndicale
- **Données de santé**
- **Données biométriques** (empreintes, reconnaissance faciale)
- Orientation sexuelle

---

## 2️⃣ QU'EST-CE QU'UN TRAITEMENT ?

### Définition (RGPD Art. 4.2)

> *"Toute opération ou ensemble d'opérations effectuées sur des données personnelles."*

---

### Les Types de Traitements

```
┌───────────────────────────────────────────────┐
│ COLLECTE                                      │
│ • Création compte utilisateur                 │
│ • Formulaire web                              │
│ • Scanner carte d'identité                    │
├───────────────────────────────────────────────┤
│ ENREGISTREMENT / STOCKAGE                     │
│ • Base de données                             │
│ • Sauvegarde                                  │
│ • Archivage                                   │
├───────────────────────────────────────────────┤
│ CONSULTATION / EXTRACTION                     │
│ • Recherche dans annuaire                     │
│ • Affichage profil utilisateur                │
│ • Export CSV                                  │
├───────────────────────────────────────────────┤
│ MODIFICATION                                  │
│ • Mise à jour adresse email                   │
│ • Changement mot de passe                     │
│ • Correction erreur                           │
├───────────────────────────────────────────────┤
│ COMMUNICATION / DIFFUSION                     │
│ • Envoi email                                 │
│ • Publication annuaire                        │
│ • Transmission sous-traitant                  │
├───────────────────────────────────────────────┤
│ EFFACEMENT / DESTRUCTION                      │
│ • Suppression compte                          │
│ • Anonymisation                               │
│ • Destruction sécurisée                       │
└───────────────────────────────────────────────┘
```

**Important :** Même la simple **consultation** d'une donnée personnelle = traitement !

---

## 3️⃣ LES 6 PRINCIPES FONDAMENTAUX (Art. 5)

### Principe 1 : Licéité, Loyauté, Transparence

**Licéité** : Traitement **légal** (base légale valide)  
**Loyauté** : Traitement **honnête** (pas de collecte cachée)  
**Transparence** : Information **claire** des personnes

**Exemple concret :**
- ✅ Collecte email avec case à cocher + explication = OK
- ❌ Collecte email sans information = NON conforme

---

### Principe 2 : Limitation des Finalités

**Règle :** Données collectées pour des **finalités déterminées, explicites et légitimes**.

**Interdiction** : Utiliser les données pour autre chose que la finalité annoncée.

**Exemple :**
- ✅ Email collecté pour "envoi newsletter" → OK pour newsletter
- ❌ Email collecté pour "newsletter" → utilisé pour démarchage commercial = NON conforme

---

### Principe 3 : Minimisation des Données

**Règle :** Collecter **uniquement** les données **strictement nécessaires**.

**Exemple :**
- ✅ Compte utilisateur : nom, prénom, email = OK
- ❌ Compte utilisateur : + date naissance + situation familiale + revenus = Trop (sauf si justifié)

---

### Principe 4 : Exactitude

**Règle :** Données doivent être **exactes et à jour**.

**Obligation :** Rectifier ou effacer données inexactes.

**Exemple :**
- Salarié change d'adresse → MAJ obligatoire dans Active Directory

---

### Principe 5 : Conservation Limitée

**Règle :** Conserver les données **uniquement le temps nécessaire**.

**Durées courantes :**
- Logs sécurité : 6 mois à 1 an
- Données RH (après départ) : 5 ans
- Données comptables : 10 ans

**Obligation :** Définir durée de conservation ET effacer après.

---

### Principe 6 : Sécurité et Confidentialité

**Règle :** Protéger les données contre :
- Accès non autorisé
- Perte accidentelle
- Destruction illicite

**Mesures techniques :**
- Chiffrement
- Contrôle d'accès (RBAC)
- Sauvegarde
- Pare-feu, antivirus

**Mesures organisationnelles :**
- Charte informatique
- Formation utilisateurs
- Procédures sécurisées

---

**[ILLUSTRATION À INSÉRER]**
**Légende :** Schéma des 6 principes RGPD représentés comme 6 piliers soutenant un toit "Protection des Données". Chaque pilier annoté : 1-Licéité, 2-Finalité, 3-Minimisation, 4-Exactitude, 5-Conservation, 6-Sécurité.

---

## 4️⃣ LES BASES LÉGALES (Art. 6)

### Pourquoi Une Base Légale ?

**Principe :** Un traitement de données personnelles est **INTERDIT** par défaut.

**Exception :** AUTORISÉ si repose sur une des **6 bases légales**.

---

### Les 6 Bases Légales

| Base légale | Définition | Exemple |
|-------------|------------|---------|
| **1. Consentement** | Accord libre, spécifique, éclairé | Newsletter marketing |
| **2. Contrat** | Nécessaire à l'exécution du contrat | Livraison commande |
| **3. Obligation légale** | Imposé par la loi | Conservation données comptables (10 ans) |
| **4. Sauvegarde intérêts vitaux** | Protection vie de la personne | Transmission dossier médical en urgence |
| **5. Mission d'intérêt public** | Service public | Inscription école publique |
| **6. Intérêt légitime** | Intérêt du responsable, proportionné | Vidéosurveillance magasin (vol) |

---

### Focus : Le Consentement

**Définition (Art. 4.11) :**

> *"Manifestation de volonté, **libre, spécifique, éclairée et univoque**."*

**Les 4 Critères :**

```
┌────────────────────────────────────────────────┐
│ LIBRE                                          │
│ • Pas de contrainte                            │
│ • Refus possible sans conséquence              │
│ • ❌ Case pré-cochée = NON libre              │
├────────────────────────────────────────────────┤
│ SPÉCIFIQUE                                     │
│ • Un consentement par finalité                 │
│ • ❌ Consentement groupé = NON spécifique     │
├────────────────────────────────────────────────┤
│ ÉCLAIRÉ                                        │
│ • Information claire sur le traitement         │
│ • ❌ CGU illisibles = NON éclairé            │
├────────────────────────────────────────────────┤
│ UNIVOQUE                                       │
│ • Action positive claire (clic, signature)     │
│ • ❌ Silence = NON univoque                   │
└────────────────────────────────────────────────┘
```

**Exemple conforme :**
```
☐ J'accepte de recevoir la newsletter hebdomadaire
  (Vous pouvez vous désabonner à tout moment)
```

**Exemple NON conforme :**
```
☑ J'accepte les CGU et la politique de confidentialité
  (case pré-cochée)
```

---

## 5️⃣ LES 8 DROITS DES PERSONNES (Art. 15-22)

**Tout individu dont les données sont traitées dispose de droits.**

---

### 1. Droit d'Accès (Art. 15)

**Principe :** Obtenir **copie** de ses données personnelles.

**Contenu :**
- Quelles données ?
- Finalités du traitement
- Destinataires
- Durée de conservation

**Délai réponse :** **1 mois**

---

### 2. Droit de Rectification (Art. 16)

**Principe :** Faire **corriger** des données inexactes.

**Exemple :** Adresse erronée dans l'annuaire → Demande de correction

---

### 3. Droit à l'Effacement / "Droit à l'Oubli" (Art. 17)

**Principe :** Obtenir **suppression** de ses données.

**Conditions (au moins une) :**
- Données plus nécessaires
- Consentement retiré
- Opposition au traitement
- Données illicitement traitées

**Exceptions :**
- Obligation légale de conservation
- Exercice liberté d'expression
- Constatation/exercice droits en justice

---

### 4. Droit à la Limitation (Art. 18)

**Principe :** **Geler** temporairement le traitement.

**Cas :**
- Contestation exactitude données (le temps de vérifier)
- Opposition au traitement

**Effet :** Données conservées mais plus utilisées.

---

### 5. Droit à la Portabilité (Art. 20)

**Principe :** Récupérer ses données dans un **format structuré** (CSV, JSON).

**Conditions :**
- Base légale = Consentement OU Contrat
- Traitement automatisé

**Exemple :** Export historique Facebook pour l'importer ailleurs

---

### 6. Droit d'Opposition (Art. 21)

**Principe :** S'opposer à un traitement.

**Cas :**
- Base légale = Intérêt légitime
- Prospection commerciale (toujours possible)

**Effet :** Arrêt du traitement (sauf motif impérieux)

---

### 7. Droit de ne pas faire l'objet d'une Décision Automatisée (Art. 22)

**Principe :** Refuser une décision **100% algorithmique** ayant des effets juridiques.

**Exemples :**
- Refus crédit automatique
- Recrutement par IA
- Profilage publicitaire

**Droit :** Demander intervention humaine

---

### 8. Droit de Définir des Directives Post-Mortem

**Principe :** Indiquer ce qu'il advient de ses données après décès.

---

**[ILLUSTRATION À INSÉRER]**
**Légende :** Infographie circulaire des 8 droits RGPD. Au centre "Personne Concernée", 8 flèches partant vers l'extérieur : Accès, Rectification, Effacement, Limitation, Portabilité, Opposition, Décision automatisée, Post-mortem. Chaque droit avec icône visuelle.

---

## 6️⃣ LES ACTEURS DU RGPD

### Responsable de Traitement

**Définition :** Entité qui **détermine les finalités et moyens** du traitement.

**Exemple :** L'entreprise qui collecte les données clients.

**Obligations :**
- Respecter les 6 principes
- Tenir registre des traitements
- Répondre aux demandes d'exercice de droits
- Notifier violations de données

---

### Sous-Traitant

**Définition :** Entité qui **traite des données pour le compte** du responsable.

**Exemple :** Hébergeur web, prestataire paie, société de sauvegarde.

**Obligations :**
- Suivre instructions du responsable
- Garantir sécurité des données
- Ne pas sous-traiter sans autorisation

---

### DPO (Délégué à la Protection des Données)

**Définition :** Personne chargée de **contrôler** la conformité RGPD.

**Obligatoire si :**
- Autorité publique
- > 250 salariés
- Traitement grande échelle de données sensibles

**Rôle :**
- Conseiller responsable/sous-traitant
- Contrôler conformité
- Point de contact CNIL
- Sensibiliser personnel

---

### CNIL (Commission Nationale Informatique et Libertés)

**Rôle :**
- Autorité de contrôle française
- Contrôle respect RGPD
- Prononce sanctions (amendes)
- Guide et informe

**Pouvoirs :**
- Contrôle sur place
- Mise en demeure
- Amende jusqu'à **20 M€** ou **4% CA mondial**

---

**[ILLUSTRATION À INSÉRER]**
**Légende :** Organigramme hiérarchique RGPD. En haut "CNIL (Contrôle)", au milieu "Responsable de Traitement" et "Sous-Traitant" (reliés par flèche), en bas "Personnes Concernées". DPO positionné en conseil du Responsable de Traitement.

---

## 7️⃣ RGPD ET TECHNICIEN SISR : Applications Concrètes

### Vous Manipulez des Données Perso Tous les Jours

**Exemples de situations :**

```
┌────────────────────────────────────────────────┐
│ CRÉATION COMPTE ACTIVE DIRECTORY               │
├────────────────────────────────────────────────┤
│ Données : Nom, prénom, email, login           │
│ Traitement : Collecte + Stockage              │
│ Base légale : Contrat de travail              │
│ Droits : Accès, rectification, effacement     │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ CONSULTATION LOGS SERVEUR                      │
├────────────────────────────────────────────────┤
│ Données : IP, login, horodatage, actions       │
│ Traitement : Consultation                      │
│ Base légale : Intérêt légitime (sécurité)     │
│ Principe : Conservation limitée (6-12 mois)    │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ SAUVEGARDE POSTE UTILISATEUR                   │
├────────────────────────────────────────────────┤
│ Données : Fichiers personnels, emails         │
│ Traitement : Copie + Stockage                  │
│ Base légale : Obligation légale OU Contrat    │
│ Principe : Sécurité (chiffrement)              │
└────────────────────────────────────────────────┘
```

---

### Obligations du Technicien SISR

**✅ À FAIRE :**
- Respecter principe de minimisation
- Sécuriser accès aux données (mots de passe, chiffrement)
- Répondre aux demandes d'exercice de droits (délai 1 mois)
- Signaler violations de données au DPO/RSSI
- Documenter actions (traçabilité)

**❌ À NE JAMAIS FAIRE :**
- Consulter données sans raison professionnelle
- Divulguer données à des tiers non autorisés
- Conserver données après suppression demandée
- Ignorer demande d'exercice de droits

---

### Responsabilité Personnelle

**Attention :** Violation RGPD = Responsabilité **pénale** possible.

**Exemple :** Divulgation données personnelles = Délit (5 ans + 300 000€)

---

## 📝 Points Clés à Retenir

### Pour l'Examen

**À connaître absolument :**
- Définition donnée personnelle (Art. 4.1)
- Les 6 principes (Art. 5)
- Les 8 droits (Art. 15-22)
- Les 6 bases légales (Art. 6)
- Délai réponse demande : 1 mois
- Sanction max : 20 M€ ou 4% CA

---

### Pour la Vie Professionnelle

**Réflexe RGPD (D.T.B.) :**

```
1. DONNÉE → Est-ce une donnée personnelle ?
2. TRAITEMENT → Quel traitement je fais ?
3. BASE LÉGALE → Ai-je le droit de le faire ?
```

**Si doute → Demander au DPO ou RSSI**

---

## 🎯 Auto-Évaluation

### Je sais...

- ☐ Définir une donnée personnelle
- ☐ Distinguer identification directe vs indirecte
- ☐ Citer les 6 principes du RGPD
- ☐ Expliquer le principe de minimisation
- ☐ Lister 5 droits des personnes
- ☐ Expliquer le droit d'accès
- ☐ Identifier les 6 bases légales
- ☐ Définir le consentement RGPD
- ☐ Expliquer le rôle du DPO
- ☐ Connaître la sanction maximale

**Si < 8 cases cochées, revoir la fiche cours.**


---

