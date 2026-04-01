---
author: YLP
title: 📖 Aide-Mémoire
---

# 📌 FICHE BILAN & MÉMO
## S16 — Responsabilité de l'Admin : L'Essentiel à Retenir

---

## 🎯 Synthèse de la Séance

| **Élément** | **Détail** |
|-------------|-----------|
| **Thème** | Responsabilité admin : pénale, civile, disciplinaire |
| **Durée** | 4 heures |
| **Approche** | Juridique + Cas pratiques + Protection |
| **Compétences** | B1.4, B2.2 |

---

## ✅ Objectifs Atteints

- ✅ Distinguer **3 responsabilités** (pénale, civile, disciplinaire)
- ✅ Connaître **Article 323-1** Code pénal (STAD)
- ✅ Comprendre **négligence** et conséquences
- ✅ Identifier **situations à risque**
- ✅ Appliquer **bonnes pratiques** protection
- ✅ Documenter ses **actions**

---

## 🔑 Le Principe Fondamental

```
╔════════════════════════════════════════════════════╗
║    RESPONSABILITÉ PERSONNELLE DE L'ADMIN           ║
╠════════════════════════════════════════════════════╣
║                                                    ║
║  Vous n'êtes PAS qu'un technicien                 ║
║  Vous êtes GARDIEN de la sécurité                 ║
║                                                    ║
║  NÉGLIGENCE GRAVE = SANCTIONS PERSONNELLES :       ║
║                                                    ║
║  1. PÉNALE : Prison + Amende + Casier            ║
║  2. CIVILE : Dommages et intérêts (€€€)          ║
║  3. DISCIPLINAIRE : Licenciement                  ║
║                                                    ║
║  LES 3 SE CUMULENT !                              ║
║                                                    ║
╚════════════════════════════════════════════════════╝
```

---

## 📊 Les 3 Responsabilités

### Tableau Comparatif

| Critère | Pénale | Civile | Disciplinaire |
|---------|--------|--------|---------------|
| **Autorité** | Juge pénal | Juge civil | Employeur |
| **Sanction** | Prison + Amende | Dommages € | Avertissement → Licenciement |
| **Qui poursuit ?** | Parquet (État) | Victime | Employeur |
| **Cumul possible ?** | ✅ Oui | ✅ Oui | ✅ Oui |
| **Casier judiciaire** | ✅ Oui | ❌ Non | ❌ Non |
| **Montant max** | 60 000€ (base) | Illimité (selon préjudice) | Perte emploi |

---

### Schéma Cumul des Responsabilités

**[ILLUSTRATION À INSÉRER]**
**Légende :** Admin au centre avec 3 flèches partant vers : 1) Prison (rouge), 2) Dommages € (orange), 3) Licenciement (jaune). Les 3 flèches convergent sur "Admin responsable". Annotation "Cumul = Triple sanction".

```
        ADMIN NÉGLIGENT
              │
        ┌─────┼─────┐
        │     │     │
        ▼     ▼     ▼
    PÉNALE  CIVILE  DISCIPLINAIRE
    Prison  €€€€€   Licenciement
```

---

## ⚖️ Article 323-1 Code Pénal

### Texte à Connaître PAR CŒUR

**Article 323-1 (STAD) :**
> *"Le fait d'accéder ou de se maintenir, frauduleusement, dans tout ou partie d'un système de traitement automatisé de données est puni de **2 ans d'emprisonnement** et de **60 000€ d'amende**."*

**Article 323-2 (aggravation) :**
- Avec suppression/modification données : **3 ans + 100 000€**

**Article 323-3 (aggravation maximale) :**
- Système État : **5 ans + 150 000€**

---

### Complicité (Art. 121-7)

```
┌────────────────────────────────────────────────┐
│ ADMIN = COMPLICE SI NÉGLIGENCE FACILITE        │
├────────────────────────────────────────────────┤
│                                                │
│ Complicité ≠ Intention de nuire               │
│                                                │
│ SUFFIT : Négligence GRAVE + Facilitation      │
│                                                │
│ Exemples :                                     │
│ • Mot de passe faible → Brute-force réussit   │
│ • Pas de MAJ → Exploit faille connue          │
│ • Port RDP exposé → Intrusion facilitée       │
│                                                │
│ Sanction : MÊME QUE L'AUTEUR (2 ans + 60k€)  │
│                                                │
└────────────────────────────────────────────────┘
```

---

## 🚨 Négligence : Les 3 Niveaux

```
┌────────────────────────────────────────────────┐
│ LÉGÈRE                                         │
│ • Erreur ponctuelle                           │
│ • Contexte difficile                          │
│ → Disciplinaire (avertissement)               │
├────────────────────────────────────────────────┤
│ GRAVE ⚠️                                       │
│ • Règles élémentaires non respectées          │
│ • Durée significative                         │
│ → Pénale + Civile + Disciplinaire            │
├────────────────────────────────────────────────┤
│ INTENTIONNELLE 🚨                              │
│ • Connaissance risque + inaction volontaire   │
│ • Mise en danger délibérée                    │
│ → Prison FERME + Interdiction exercer         │
└────────────────────────────────────────────────┘
```

---

### Exemples Négligence Grave (Jurisprudence)

```
❌ Mot de passe faible (admin, 123456, password)
❌ Pas de MAJ > 6 mois (surtout si faille critique)
❌ Pas de sauvegarde OU sauvegarde jamais testée
❌ Port RDP/SSH exposé Internet sans protection
❌ Pas de journalisation
❌ Compte root partagé
❌ Ignorer alertes CERT/ANSSI répétées
❌ Pas de pare-feu / antivirus
❌ Serveur obsolète maintenu (fin de vie dépassée)
```

---

## 📖 Jurisprudence Clés

### TGI Paris (2018) — ✅ CONDAMNÉ

```
╔════════════════════════════════════════════════════╗
║  FAITS                                             ║
║  • Intrusion e-commerce                           ║
║  • Vol 50 000 clients                             ║
║                                                    ║
║  NÉGLIGENCES                                       ║
║  • Mdp "admin123"                                 ║
║  • Pas MAJ 2 ans                                  ║
║  • Pas sauvegarde                                 ║
║                                                    ║
║  SANCTION                                          ║
║  • 6 mois prison avec sursis                      ║
║  • 5 000€ amende                                  ║
║  • Licenciement faute grave                       ║
║  • Dommages solidaires entreprise                 ║
╚════════════════════════════════════════════════════╝
```

---

### CA Lyon (2020) — ❌ RELAXÉ

```
╔════════════════════════════════════════════════════╗
║  FAITS                                             ║
║  • Ransomware sophistiqué (0-day)                 ║
║                                                    ║
║  MESURES EN PLACE                                  ║
║  • ✅ Antivirus + Pare-feu                        ║
║  • ✅ Sauvegardes testées                         ║
║  • ✅ MAJ régulières                              ║
║  • ✅ Sensibilisation users                       ║
║  • ✅ Restauration 12h                            ║
║                                                    ║
║  DÉCISION                                          ║
║  • RELAXE                                         ║
║  • Obligation moyens respectée                    ║
║  • Attaque sophistiquée ≠ négligence             ║
╚════════════════════════════════════════════════════╝
```

**Principe :** Admin ne garantit PAS absence incident, mais doit mettre en œuvre moyens raisonnables.

---

## 🛡️ Les 5 Règles d'Or de Protection

```
1️⃣ RESPECTER LES BASES
   ✅ Mots de passe complexes (12+ car, majuscules, chiffres, symboles)
   ✅ MAJ critiques < 1 semaine
   ✅ Sauvegardes quotidiennes TESTÉES trimestriellement
   ✅ Pare-feu + Antivirus configurés
   ✅ VPN pour accès distants (JAMAIS RDP/SSH direct Internet)

2️⃣ DOCUMENTER TOUT
   ✅ Journal admin quotidien (actions, décisions, problèmes)
   ✅ Procédures écrites (sauvegarde, MAJ, incidents)
   ✅ Conserver preuves (emails, tickets, captures)
   → Traçabilité = Preuve diligence

3️⃣ ALERTER PAR ÉCRIT
   ✅ Si risque identifié + budget/temps insuffisant
   ✅ Email direction avec AR (accusé réception)
   ✅ Conserver copie (preuve signalement)
   → Transfert responsabilité

4️⃣ TESTER RÉGULIÈREMENT
   ✅ Sauvegardes : restauration complète trimestrielle
   ✅ PRA : exercice annuel
   ✅ Mesures sécurité : audit interne
   → Obligation Art. 32 RGPD (tester efficacité)

5️⃣ SE FORMER CONTINUELLEMENT
   ✅ Veille sécurité (CERT-FR, ANSSI, CVE)
   ✅ Formations (demander employeur)
   ✅ Certifications (CISSP, CEH, CompTIA Security+)
   → Compétence = Protection
```

---

## 📝 Modèle Email d'Alerte

**Template à utiliser en cas de risque identifié :**

```
De : [Votre nom], Administrateur Système
À : Direction / DSI
Objet : ⚠️ ALERTE SÉCURITÉ — [Résumé risque]

Madame, Monsieur,

Je vous informe d'un risque de sécurité identifié sur notre 
infrastructure :

SITUATION :
[Description précise du risque]

CONSÉQUENCES POTENTIELLES :
[Impact si incident : perte données, intrusion, indisponibilité]

SOLUTIONS PROPOSÉES :
1. [Solution 1 avec coût et délai]
2. [Solution 2 avec coût et délai]

DÉLAI RECOMMANDÉ :
[Urgent / Court terme / Moyen terme]

En l'absence de mise en œuvre de ces mesures, je décline toute 
responsabilité en cas d'incident.

Je reste à votre disposition pour tout complément d'information.

Cordialement,
[Signature]

---
IMPORTANT : Conserver cet email + accusé lecture/réception
```

---

## 🔧 Checklist Conformité Quotidienne

**À vérifier régulièrement :**

```
QUOTIDIEN
☐ Sauvegardes exécutées correctement
☐ Logs consultés (alertes critiques)
☐ Espace disque suffisant

HEBDOMADAIRE
☐ Revue alertes sécurité (CERT, éditeurs)
☐ Vérification antivirus/pare-feu
☐ Logs détaillés analysés

MENSUEL
☐ MAJ non critiques appliquées
☐ Revue comptes utilisateurs (désactiver inactifs)
☐ Vérification procédures à jour

TRIMESTRIEL
☐ Test restauration sauvegarde COMPLET
☐ Revue politique sécurité
☐ Audit interne sécurité

ANNUEL
☐ Exercice PRA/PCA
☐ Formation sécurité
☐ Pentest (si budget)
```

---

## 💡 Situations à Risque et Actions

| Situation à risque | Action OBLIGATOIRE | Délai |
|--------------------|--------------------|-------|
| **Alerte CERT critique** | Lire + Évaluer + Patcher | < 48h |
| **Serveur fin de vie** | Alerter direction + Planifier migration | Immédiat |
| **Mot de passe compromis** | Changer immédiatement + Auditer accès | < 1h |
| **Budget sécurité refusé** | Email formel direction + Documenter | Immédiat |
| **Sauvegarde échouée** | Investiguer + Corriger + Tester | < 24h |
| **Alerte IDS/IPS** | Analyser + Traiter si réel + Documenter | < 4h |

---

## 📝 Auto-Évaluation Finale

### Je maîtrise...

**Connaissances juridiques :**
- ☐ Distinguer 3 responsabilités (pénale, civile, disciplinaire)
- ☐ Citer Article 323-1 (2 ans + 60 000€)
- ☐ Expliquer complicité involontaire
- ☐ Définir obligation moyens vs résultat
- ☐ Citer 2 jurisprudences (TGI 2018, CA 2020)

**Identification risques :**
- ☐ Reconnaître négligence grave (5 exemples)
- ☐ Évaluer risque situation donnée
- ☐ Distinguer négligence légère/grave/intentionnelle

**Protection juridique :**
- ☐ Appliquer 5 règles d'or
- ☐ Rédiger email d'alerte conforme
- ☐ Documenter actions quotidiennes
- ☐ Savoir quand alerter direction

**Si < 10 cases cochées sur 12, revoir la fiche cours.**

---

## 🔗 Liens avec Autres Séances

| Séance | Lien avec S16 |
|--------|---------------|
| **S9 (Article 32)** | Obligation sécurité → Responsabilité si manquement |
| **S14 (Preuve)** | Logs = preuves responsabilité (ou innocence) |
| **S6 (RGPD)** | Violation RGPD → Responsabilité admin |
| **Bloc 1 - Sécurité** | Mise en œuvre technique = éviter responsabilité |

---

## 💡 Points Clés pour l'Examen

**À retenir PAR CŒUR :**

```
┌────────────────────────────────────────────────┐
│ • 3 responsabilités : Pénale, Civile, Disciplinaire│
│   LES 3 SE CUMULENT                            │
│                                                │
│ • Article 323-1 : 2 ans + 60 000€             │
│   Complicité = MÊME PEINE                     │
│                                                │
│ • Négligence grave :                           │
│   - Mdp faible                                 │
│   - Pas MAJ > 6 mois                          │
│   - Pas sauvegarde testée                     │
│   - Port exposé Internet                       │
│                                                │
│ • Obligation de MOYENS (pas résultat)         │
│                                                │
│ • Protection : DOCUMENTER + ALERTER + TESTER  │
│                                                │
│ • TGI 2018 : Condamné (6 mois + 5 000€)       │
│ • CA 2020 : Relaxé (mesures OK)               │
└────────────────────────────────────────────────┘
```

---

## 🎯 Message Final

**Vous êtes PERSONNELLEMENT responsable**

```
Négligence grave :
❌ Prison
❌ Amende personnelle
❌ Dommages (€€€)
❌ Licenciement
❌ Casier judiciaire
❌ Difficulté retrouver emploi

Diligence professionnelle :
✅ Sécurité maîtrisée
✅ Responsabilité protégée
✅ Carrière préservée
✅ Crédibilité professionnelle
✅ Valorisation compétences
```

**La documentation et l'alerte écrite sont vos MEILLEURES protections juridiques.**

---

## 📅 Prochaine Séance

**S17 : Contrats Informatiques**
- Contrat prestation services
- SLA (Service Level Agreement)
- Clauses limitatives responsabilité
- Litiges et résolution

---

## 📚 Ressources Complémentaires

**Textes juridiques :**
- Code pénal : Articles 323-1 à 323-7 (STAD)
- Code pénal : Article 121-7 (complicité)
- Code civil : Article 1240 (responsabilité civile)

**Veille sécurité :**
- **CERT-FR** : cert.ssi.gouv.fr (alertes officielles)
- **ANSSI** : cyber.gouv.fr (guides, recommandations)
- **CVE** : cve.mitre.org (vulnérabilités)

**Formation continue :**
- ANSSI : Formations cybersécurité
- CLUSIF : Bonnes pratiques admin
- Certifications : CISSP, CEH, CompTIA Security+

---
