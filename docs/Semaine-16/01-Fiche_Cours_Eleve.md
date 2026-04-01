---
author: YLP
title: 📖 Fiche de Cours Élève
---

# 📖 FICHE DE COURS ÉLÈVE
## S16 — Responsabilité de l'Admin : Pénale, Civile, Disciplinaire

*BTS SIO SISR — Année 1 — Semaine 16*

---

À la fin de cette séance, je serai capable de :

✅ Distinguer **3 types de responsabilité** (pénale, civile, disciplinaire)  
✅ Connaître **Article 323-1** Code pénal (STAD)  
✅ Comprendre la **négligence** et ses conséquences  
✅ Identifier les **situations à risque**  
✅ Appliquer les **bonnes pratiques** de protection  
✅ Documenter mes **actions** (traçabilité)

---

## 📚 Vocabulaire Juridique

| **Terme** | **Définition** |
|-----------|----------------|
| **Responsabilité pénale** | Obligation de répondre de ses actes devant la justice pénale |
| **Responsabilité civile** | Obligation de réparer le préjudice causé à autrui |
| **Responsabilité disciplinaire** | Obligation de répondre devant l'employeur (sanctions internes) |
| **Négligence** | Manquement à une obligation de prudence |
| **STAD** | Système de Traitement Automatisé de Données |
| **Complicité** | Faciliter sciemment la commission d'une infraction |
| **Obligation de moyens** | Obligation de mettre en œuvre tous les moyens raisonnables |

---

## 1️⃣ LES 3 TYPES DE RESPONSABILITÉ

### Vue d'Ensemble

```
╔════════════════════════════════════════════════════╗
║   RESPONSABILITÉ DE L'ADMINISTRATEUR SYSTÈME       ║
╠════════════════════════════════════════════════════╣
║                                                    ║
║  1. PÉNALE (Code pénal)                           ║
║     Autorité : Parquet, Juge pénal                ║
║     Sanction : Prison + Amende                    ║
║     Conséquence : Casier judiciaire               ║
║                                                    ║
║  2. CIVILE (Code civil)                           ║
║     Autorité : Juge civil                         ║
║     Sanction : Dommages et intérêts               ║
║     Conséquence : Réparation financière           ║
║                                                    ║
║  3. DISCIPLINAIRE (Code du travail)               ║
║     Autorité : Employeur                          ║
║     Sanction : Avertissement → Licenciement       ║
║     Conséquence : Perte emploi                    ║
║                                                    ║
║  ⚠️ LES 3 PEUVENT SE CUMULER !                    ║
║                                                    ║
╚════════════════════════════════════════════════════╝
```

**[ILLUSTRATION À INSÉRER]**
**Légende :** Schéma circulaire avec administrateur au centre. 3 flèches partant vers 3 cercles : 1) Juge pénal (prison), 2) Juge civil (€), 3) Employeur (licenciement). Annotation "Cumul possible".

---

### 1. Responsabilité Pénale

**Définition :**
> Obligation de répondre de ses actes devant la **justice pénale** en cas d'infraction.

**Caractéristiques :**
- **TOUJOURS personnelle** (pas l'entreprise à votre place)
- Sanctions : Prison + Amende
- Casier judiciaire (conséquences emploi futur)

**Infractions possibles pour un admin :**

| Infraction | Article | Peine maximale |
|------------|---------|----------------|
| **Accès frauduleux (STAD)** | 323-1 CP | 2 ans + 60 000€ |
| **Complicité intrusion** | 121-7 + 323-1 | 2 ans + 60 000€ |
| **Mise en danger d'autrui** | 223-1 CP | 1 an + 15 000€ |
| **Violation secret professionnel** | 226-13 CP | 1 an + 15 000€ |
| **Non-assistance personne en danger** | 223-6 CP | 5 ans + 75 000€ |

---

### 2. Responsabilité Civile

**Définition :**
> Obligation de **réparer le préjudice** causé à autrui (Article 1240 Code civil).

**Principe :**
```
Faute + Dommage + Lien causalité = Responsabilité civile
```

**Types de dommages :**
- **Matériel** : Perte données, arrêt activité, coût restauration
- **Immatériel** : Perte image, clients perdus
- **Moral** : Stress, angoisse

**Montants :**
- Selon préjudice réel
- Peut atteindre plusieurs millions €
- Admin peut être condamné **solidairement** avec entreprise

---

### 3. Responsabilité Disciplinaire

**Définition :**
> Sanctions internes prononcées par l'**employeur** (Code du travail).

**Échelle des sanctions :**

```
LÉGÈRES
  ↓
  Avertissement oral
  ↓
  Avertissement écrit
  ↓
  Mise à pied (sans salaire)
  ↓
  Mutation
  ↓
  Rétrogradation
  ↓
  Licenciement pour faute simple
  ↓
  Licenciement pour faute grave
  ↓
  Licenciement pour faute lourde
  ↓
LOURDES (+ dommages employeur)
```

**Conséquences :**
- Faute grave/lourde : Pas d'indemnités, pas de préavis
- Perte emploi immédiate
- Difficultés retrouver emploi (références)

---

## 2️⃣ ARTICLE 323-1 CODE PÉNAL (STAD)

### Texte Intégral

**Article 323-1 :**
> *"Le fait d'accéder ou de se maintenir, frauduleusement, dans tout ou partie d'un système de traitement automatisé de données est puni de **2 ans d'emprisonnement** et de **60 000€ d'amende**."*

**Article 323-2 (aggravation) :**
> *"Lorsqu'il en est résulté soit la suppression ou la modification de données, soit une altération du fonctionnement du système, la peine est de **3 ans** et **100 000€**."*

**Article 323-3 (aggravation maximale) :**
> *"Lorsque les infractions prévues aux articles 323-1 et 323-2 ont été commises à l'encontre d'un système de traitement automatisé de données à caractère personnel mis en œuvre par l'État, la peine est de **5 ans** et **150 000€**."*

---

### Complicité (Article 121-7)

**Texte :**
> *"Est complice d'un crime ou d'un délit la personne qui **sciemment**, par aide ou assistance, **en a facilité** la préparation ou la consommation."*

**Application à l'admin :**
```
Admin négligent → Facilite intrusion → Complicité possible

Exemples :
• Mot de passe faible (facilite brute-force)
• Pas de MAJ (facilite exploit faille connue)
• Port RDP ouvert Internet (facilite intrusion)
```

**ATTENTION :** Pas besoin d'intention de nuire. La **négligence grave** suffit.

---

## 3️⃣ LA NÉGLIGENCE : DEGRÉS ET CONSÉQUENCES

### Définition Juridique

**Négligence :**
> Manquement à une **obligation de prudence** dans l'exercice de sa profession.

**3 niveaux de gravité :**

```
┌────────────────────────────────────────────────┐
│ NÉGLIGENCE LÉGÈRE                              │
├────────────────────────────────────────────────┤
│ • Erreur ponctuelle, inhabituelle             │
│ • Contexte difficile (pression, moyens)       │
│ • Pas de conséquence grave                    │
│                                                │
│ Responsabilité : Disciplinaire (avertissement)│
│ Sanction type : Avertissement, mise à pied    │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ NÉGLIGENCE GRAVE                               │
├────────────────────────────────────────────────┤
│ • Non-respect règles élémentaires             │
│ • Durée significative (mois, années)          │
│ • Conséquences importantes                     │
│                                                │
│ Responsabilité : Pénale + Civile + Disciplinaire│
│ Sanction type : Prison sursis + Dommages +    │
│                 Licenciement faute grave       │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ NÉGLIGENCE INTENTIONNELLE (Faute intentionnelle)│
├────────────────────────────────────────────────┤
│ • Connaissance du risque                       │
│ • Inaction volontaire malgré risque           │
│ • Mise en danger délibérée                     │
│                                                │
│ Responsabilité : Pénale aggravée               │
│ Sanction type : Prison FERME + Amende + Inter-│
│                 diction d'exercer + Dommages   │
└────────────────────────────────────────────────┘
```

---

### Exemples de Négligence Grave

**Reconnus par la jurisprudence :**

```
❌ Mot de passe faible (admin, 123456, password)
❌ Pas de mise à jour > 6 mois
❌ Pas de sauvegarde OU sauvegarde jamais testée
❌ Pas de journalisation
❌ Port sensible exposé Internet sans protection (RDP, SSH sans VPN)
❌ Compte root/admin partagé
❌ Pas de politique de sécurité
❌ Ignorer alertes critiques répétées
❌ Pas de formation sur outils critiques
❌ Pas d'antivirus / pare-feu
```

---

## 4️⃣ OBLIGATION DE MOYENS VS OBLIGATION DE RÉSULTAT

### Distinction Fondamentale

**Admin système = Obligation de MOYENS (pas de résultat)**

```
┌────────────────────────────────────────────────┐
│ OBLIGATION DE RÉSULTAT                         │
├────────────────────────────────────────────────┤
│ • Garantir le résultat                         │
│ • Si échec = responsabilité automatique        │
│ • Exemple : Transporteur (livrer colis)       │
│                                                │
│ ≠ Admin système                                │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ OBLIGATION DE MOYENS                           │
├────────────────────────────────────────────────┤
│ • Mettre en œuvre moyens raisonnables          │
│ • Pas de garantie résultat                     │
│ • Si échec MALGRÉ moyens = PAS responsable    │
│ • Exemple : Médecin (soigner, pas guérir)     │
│                                                │
│ = Admin système ✅                             │
└────────────────────────────────────────────────┘
```

**Conséquence :**
> Admin ne garantit PAS l'absence totale d'incident, mais doit mettre en œuvre **tous les moyens raisonnables** pour l'éviter.

---

### Moyens Raisonnables (Jurisprudence)

**Considérés comme raisonnables :**
- ✅ Mots de passe complexes (politique écrite)
- ✅ Mises à jour régulières (< 1 mois pour critiques)
- ✅ Sauvegardes testées (au moins trimestrielles)
- ✅ Antivirus + Pare-feu configurés
- ✅ Journalisation activée
- ✅ VPN pour accès distants
- ✅ Séparation des privilèges (comptes nominatifs)
- ✅ Sensibilisation utilisateurs
- ✅ Documentation procédures
- ✅ Veille sécurité (bulletins, CVE)

**PAS raisonnables d'exiger :**
- ❌ Sécurité absolue (impossible)
- ❌ Protection contre 0-day sophistiqués
- ❌ Surveillance 24/7 si pas de moyens
- ❌ Outils enterprise (si PME budget limité)

---

## 5️⃣ JURISPRUDENCE CLÉS

### CAS 1 : TGI Paris (2018) — Admin CONDAMNÉ

**Faits :**
- Intrusion serveur e-commerce
- Vol 50 000 clients (noms, CB)

**Négligences admin :**
- Mot de passe "admin123" (compte root)
- Pas de MAJ depuis 2 ans
- Aucune sauvegarde
- Pas de journalisation

**Décision :**
✅ **CONDAMNATION**
- 6 mois prison avec sursis
- 5 000€ amende personnelle
- Licenciement faute grave
- Dommages et intérêts solidaires avec entreprise

**Motif :** Négligence **grave et caractérisée** facilitant intrusion (complicité involontaire).

---

### CAS 2 : CA Lyon (2020) — Admin RELAXÉ

**Faits :**
- Ransomware sophistiqué (APT, 0-day)
- Serveur chiffré

**Mesures admin :**
- ✅ Antivirus à jour
- ✅ Pare-feu configuré
- ✅ Sauvegardes quotidiennes testées
- ✅ Sensibilisation personnel
- ✅ Patches < 7 jours
- ✅ Restauration réussie 12h

**Décision :**
❌ **RELAXE**

**Motif :** Obligation de moyens **respectée**. Attaque sophistiquée ne peut être reprochée si moyens adaptés mis en œuvre.

---

## 6️⃣ SE PROTÉGER JURIDIQUEMENT

### Les 5 Règles d'Or

```
1️⃣ RESPECTER LES RÈGLES ÉLÉMENTAIRES
   → Mots de passe, MAJ, sauvegardes, pare-feu
   → Appliquer ANSSI, CNIL, bonnes pratiques

2️⃣ DOCUMENTER TOUTES SES ACTIONS
   → Traçabilité = preuve de diligence
   → Tenir journal actions, décisions
   → Conserver preuves (emails, tickets)

3️⃣ ALERTER PAR ÉCRIT (EMAIL)
   → Si risque identifié + budget/temps insuffisant
   → Email direction : "Je vous informe que..."
   → Conserver accusé lecture

4️⃣ TESTER RÉGULIÈREMENT
   → Sauvegardes : test restauration trimestriel
   → PRA : exercice annuel
   → Mesures sécurité : audit interne

5️⃣ SE FORMER CONTINUELLEMENT
   → Veille sécurité (CERT, ANSSI, CVE)
   → Certifications (CISSP, CEH, OSCP)
   → Formations employeur (demander)
```

---

### Documentation Essentielle

**Que documenter ?**

```
┌────────────────────────────────────────────────┐
│ JOURNAL ADMINISTRATEUR (quotidien)             │
├────────────────────────────────────────────────┤
│ Date | Action | Motif | Résultat              │
│                                                │
│ Exemple :                                      │
│ 15/02 | MAJ Apache 2.4.58 | CVE-2024-1234    │
│       | critique | Succès                     │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ ALERTES ET SIGNALEMENTS (par écrit)           │
├────────────────────────────────────────────────┤
│ À : Direction                                  │
│ Objet : Alerte sécurité - Serveur obsolète    │
│                                                │
│ "Je vous informe que le serveur XXX n'a pas   │
│ été mis à jour depuis X mois faute de budget. │
│ Risque d'intrusion élevé. Patch nécessaire."  │
│                                                │
│ → CONSERVER EMAIL + ACCUSÉ LECTURE            │
└────────────────────────────────────────────────┘

┌────────────────────────────────────────────────┐
│ PROCÉDURES ET POLITIQUES (écrites)            │
├────────────────────────────────────────────────┤
│ • Politique mots de passe                      │
│ • Procédure sauvegarde/restauration            │
│ • Procédure gestion incidents                  │
│ • Politique mises à jour                       │
│                                                │
│ → VALIDÉES PAR DIRECTION                       │
└────────────────────────────────────────────────┘
```

---

## 📝 Points Clés à Retenir

### Pour l'Examen

**À connaître PAR CŒUR :**

```
┌────────────────────────────────────────────────┐
│ • 3 responsabilités : Pénale, Civile, Disciplinaire│
│   LES 3 SE CUMULENT                            │
│                                                │
│ • Article 323-1 : 2 ans + 60 000€ (STAD)      │
│                                                │
│ • Complicité = Faciliter intrusion (même involontaire)│
│                                                │
│ • Obligation de MOYENS (pas résultat)         │
│                                                │
│ • Négligence grave :                           │
│   Mdp faible, pas MAJ >6 mois, pas sauvegarde │
│                                                │
│ • Protection : DOCUMENTER + ALERTER + TESTER  │
│                                                │
│ • TGI 2018 : Condamné (mdp faible)            │
│ • CA 2020 : Relaxé (mesures OK)               │
└────────────────────────────────────────────────┘
```

---

### Pour la Vie Professionnelle

**Réflexe quotidien :**

✅ **Avant toute action :**
- Est-ce conforme aux règles ?
- Ai-je les moyens techniques ?
- Dois-je alerter direction ?

✅ **Après toute action :**
- Documenter dans journal
- Tester si critique
- Archiver preuves

✅ **En cas de risque identifié :**
- Email direction IMMÉDIAT
- Proposer solutions
- Conserver preuve signalement

---

## 🎯 Auto-Évaluation

### Je sais...

- ☐ Distinguer les 3 responsabilités
- ☐ Citer Article 323-1 (peine STAD)
- ☐ Définir négligence grave
- ☐ Expliquer obligation moyens vs résultat
- ☐ Lister 5 exemples négligence grave
- ☐ Expliquer complicité involontaire
- ☐ Citer 2 jurisprudences (TGI 2018, CA 2020)
- ☐ Appliquer les 5 règles d'or protection
- ☐ Documenter mes actions quotidiennes

**Si < 7 cases cochées, revoir la fiche cours.**


---
