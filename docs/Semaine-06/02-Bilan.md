---
author: YLP
title: 📚 FICHE BILAN
---

# 📌 FICHE BILAN & MÉMO
## S6 — RGPD Fondamentaux : L'Essentiel à Retenir

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 6*

---

## 🔑 Définitions Essentielles

```
╔════════════════════════════════════════════════════╗
║              LES 3 DÉFINITIONS CLÉS                ║
╠════════════════════════════════════════════════════╣
║                                                    ║
║  DONNÉE PERSONNELLE (Art. 4.1)                    ║
║  Toute information relative à une personne        ║
║  physique IDENTIFIÉE ou IDENTIFIABLE              ║
║                                                    ║
║  TRAITEMENT (Art. 4.2)                            ║
║  Toute opération sur des données personnelles     ║
║  (collecte, stockage, consultation, effacement)   ║
║                                                    ║
║  CONSENTEMENT (Art. 4.11)                         ║
║  Accord LIBRE, SPÉCIFIQUE, ÉCLAIRÉ et UNIVOQUE   ║
║                                                    ║
╚════════════════════════════════════════════════════╝
```

---

## 📊 Les 6 Principes du RGPD (Art. 5)

| Principe | Signification | Exemple concret |
|----------|---------------|-----------------|
| **1. Licéité, loyauté, transparence** | Traitement légal, honnête, clair | Informer utilisateurs de la collecte |
| **2. Limitation finalités** | Usage conforme finalité annoncée | Email newsletter ≠ démarchage commercial |
| **3. Minimisation données** | Collecter uniquement le nécessaire | Compte AD : nom, email OK. Situation familiale KO. |
| **4. Exactitude** | Données exactes et à jour | MAJ adresse si changement |
| **5. Conservation limitée** | Durée limitée au nécessaire | Logs 6-12 mois, RH 5 ans |
| **6. Sécurité** | Protection contre accès non autorisé | Chiffrement, contrôle accès, sauvegardes |

---

## 👥 Les 8 Droits des Personnes

```
┌───────────────────────────────────────────────────┐
│ 1. ACCÈS (Art. 15)                                │
│    → Obtenir copie de ses données                 │
│    → Délai : 1 mois                               │
├───────────────────────────────────────────────────┤
│ 2. RECTIFICATION (Art. 16)                        │
│    → Corriger données inexactes                   │
├───────────────────────────────────────────────────┤
│ 3. EFFACEMENT / "Droit à l'oubli" (Art. 17)      │
│    → Supprimer ses données                        │
│    → SAUF obligations légales                     │
├───────────────────────────────────────────────────┤
│ 4. LIMITATION (Art. 18)                           │
│    → Geler temporairement le traitement          │
├───────────────────────────────────────────────────┤
│ 5. PORTABILITÉ (Art. 20)                          │
│    → Récupérer données (CSV, JSON)                │
├───────────────────────────────────────────────────┤
│ 6. OPPOSITION (Art. 21)                           │
│    → S'opposer à un traitement                    │
├───────────────────────────────────────────────────┤
│ 7. DÉCISION AUTOMATISÉE (Art. 22)                 │
│    → Refuser décision 100% algorithmique          │
├───────────────────────────────────────────────────┤
│ 8. DIRECTIVES POST-MORTEM                         │
│    → Définir sort données après décès             │
└───────────────────────────────────────────────────┘
```

---

## ⚖️ Les 6 Bases Légales (Art. 6)

**Un traitement est INTERDIT sauf si basé sur :**

| Base légale | Cas d'usage |
|-------------|-------------|
| **1. Consentement** | Newsletter marketing |
| **2. Contrat** | Livraison commande, paie salarié |
| **3. Obligation légale** | Conservation comptabilité (10 ans) |
| **4. Sauvegarde intérêts vitaux** | Urgence médicale |
| **5. Mission intérêt public** | Service public |
| **6. Intérêt légitime** | Vidéosurveillance anti-vol |

---

## 🎯 Le Réflexe D.T.B. (Donnée, Traitement, Base)

**AVANT tout traitement de données, se poser 3 questions :**

```
1. DONNÉE : Est-ce une donnée personnelle ?
   → Identifie-t-elle une personne ?

2. TRAITEMENT : Qu'est-ce que je fais avec ?
   → Collecte, stockage, consultation, modification ?

3. BASE LÉGALE : Ai-je le droit ?
   → Consentement ? Contrat ? Obligation légale ?
```

**Si doute → Demander au DPO ou RSSI**

---

## 💻 RGPD et Technicien SISR

### Vous Manipulez des Données Perso Quotidiennement

**Exemples concrets :**

| Action quotidienne | Données perso | Base légale | Principe RGPD |
|-------------------|---------------|-------------|---------------|
| Créer compte AD | Nom, email, login | Contrat travail | Minimisation |
| Consulter logs | IP, horodatage, actions | Intérêt légitime (sécurité) | Conservation limitée (6-12 mois) |
| Sauvegarder poste | Fichiers, emails | Obligation légale | Sécurité (chiffrement) |
| Ticket support | Nom, problème | Contrat travail | Confidentialité |

---

### Vos Obligations

**✅ À FAIRE :**
- Respecter principe de minimisation
- Sécuriser accès (mots de passe, chiffrement)
- Répondre demandes exercice droits (1 mois)
- Signaler violations au DPO/RSSI
- Documenter actions (traçabilité)

**❌ NE JAMAIS FAIRE :**
- Consulter données sans raison professionnelle
- Divulguer à tiers non autorisés
- Ignorer demande d'exercice de droits
- Conserver après suppression demandée

---

## 📐 Schémas Récapitulatifs

### Schéma 1 : Classification des Données

**[ILLUSTRATION À INSÉRER]**
**Légende :** Pyramide à 3 niveaux. Base (large) : "Données techniques (température, SIRET)" - Milieu : "Données personnelles standards (nom, email, IP)" - Sommet (étroit) : "Données sensibles (santé, biométrie)". Couleur vert → orange → rouge selon sensibilité.

---

### Schéma 2 : Acteurs du RGPD

```
        ┌─────────────┐
        │    CNIL     │  ← Contrôle et sanctionne
        │  (Autorité) │
        └──────┬──────┘
               │ Contrôle
               ▼
   ┌───────────────────────┐
   │ RESPONSABLE TRAITEMENT │ ← Détermine finalités
   │    (Entreprise)        │
   └───────────┬───────────┘
               │
        ┌──────┴──────┐
        │             │
        ▼             ▼
   ┌────────┐   ┌─────────────┐
   │  DPO   │   │SOUS-TRAITANT│ ← Traite pour compte de
   │(Conseil)│   │ (Hébergeur) │
   └────────┘   └─────────────┘
        │
        │ Informe et conseille
        ▼
   ┌─────────────────────┐
   │ PERSONNES CONCERNÉES │
   │   (Utilisateurs)     │
   └─────────────────────┘
```

---

## 🚨 Sanctions et Risques

**Sanctions CNIL (Art. 83) :**
- Avertissement
- Mise en demeure
- Limitation temporaire ou définitive du traitement
- **Amende jusqu'à 20 M€ ou 4% du CA mondial**

**Exemples d'amendes :**
- Google (2020) : 90 M€ (cookies sans consentement)
- Amazon (2021) : 746 M€ (publicité ciblée)
- Meta (2023) : 1,2 Md€ (transferts USA)

**Responsabilité pénale :**
- Divulgation données : 5 ans + 300 000€
- Détournement finalité : 5 ans + 300 000€

---

## 📝 Auto-Évaluation Finale

### Je maîtrise...

**Connaissances :**
- ☐ Définir donnée personnelle (directe/indirecte)
- ☐ Expliquer les 6 principes RGPD
- ☐ Citer 5 droits des personnes sur 8
- ☐ Identifier les 6 bases légales
- ☐ Expliquer le consentement LSEU

**Application :**
- ☐ Reconnaître une donnée perso dans un système
- ☐ Identifier la base légale d'un traitement
- ☐ Traiter une demande d'accès (délai, contenu)
- ☐ Appliquer principe minimisation
- ☐ Sécuriser données (chiffrement, accès)

**Posture professionnelle :**
- ☐ Savoir quand demander au DPO
- ☐ Documenter actions RGPD
- ☐ Respecter confidentialité données
- ☐ Signaler violations

**Si < 10 cases cochées sur 14, revoir la fiche cours.**

---

## 🔗 Liens avec Autres Séances

| Séance | Lien avec S6 |
|--------|-------------|
| **S3 (Charte)** | Charte informatique = mise en œuvre RGPD |
| **S7 (RGPD 2)** | Approfondissement : DPO, PIA, violations |
| **Bloc 1 - AD** | Comptes utilisateurs = données personnelles |
| **Bloc 1 - Cybersécurité** | RGPD Art. 32 = obligation de sécurité |
| **Bloc 2 - Support** | Tickets = traitement données perso |

---

## 📚 Ressources Complémentaires

**Sites officiels :**
- **CNIL** : cnil.fr (guides, FAQ, jurisprudence)
- **EUR-Lex** : Texte intégral RGPD en français
- **CEPD** : Lignes directrices européennes

**Outils pratiques :**
- Registre des traitements (template CNIL)
- Modèles emails exercice droits
- Checklist conformité RGPD

**Formation continue :**
- MOOC CNIL "Atelier RGPD"
- Certifications RGPD (IAPP, AFCDP)

---

## 💡 Points Clés pour l'Examen

**À connaître PAR CŒUR :**

```
┌────────────────────────────────────────────────┐
│ • Donnée perso = personne identifiée          │
│                  ou identifiable               │
│                                                │
│ • IP = donnée personnelle (CJUE 2016)         │
│                                                │
│ • 6 principes (Art. 5)                        │
│                                                │
│ • Délai réponse demande = 1 mois              │
│                                                │
│ • Consentement = LSEU                          │
│   (Libre, Spécifique, Éclairé, Univoque)     │
│                                                │
│ • Sanction max = 20 M€ ou 4% CA               │
│                                                │
│ • Base légale contrat pour compte AD          │
│                                                │
│ • Droit effacement SAUF obligation légale     │
└────────────────────────────────────────────────┘
```

---

## 🎯 Conclusion

**Le RGPD n'est pas une contrainte, c'est une opportunité :**

✅ **Protéger les utilisateurs** → Confiance  
✅ **Sécuriser l'entreprise** → Éviter amendes  
✅ **Professionnaliser les pratiques** → Qualité de service  
✅ **Valoriser les compétences** → Expertise reconnue

**En tant que technicien SISR, vous êtes ACTEUR de la conformité RGPD.**

---

