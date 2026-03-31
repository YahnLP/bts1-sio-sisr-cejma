---
author: YLP
title: 📚 FICHE DE COURS
---


# 📚 FICHE DE COURS ÉLÈVE
## Propriété Intellectuelle : Le Droit d'Auteur Appliqué au Code et au Logiciel

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 11*

---

## 🎯 Objectifs de Cette Fiche

À la fin de ce cours, vous serez capable de :
- ✅ Définir le droit d'auteur et ses composantes (moral et patrimonial)
- ✅ Expliquer la protection juridique du code source et des logiciels
- ✅ Distinguer logiciel propriétaire, libre, open source, freeware
- ✅ Identifier les principales licences open source et leurs implications
- ✅ Comprendre vos droits en tant que développeur salarié
- ✅ Reconnaître et éviter la contrefaçon de code

---

## 📖 PARTIE I — Les Fondements du Droit d'Auteur

### I.A. Définition et Principes

Le **droit d'auteur** est un droit de **propriété intellectuelle** qui protège les **œuvres de l'esprit**.

**Base légale :** Code de la Propriété Intellectuelle (CPI), articles L111-1 et suivants.

**Principe fondamental (art. L111-1) :**
> *"L'auteur d'une œuvre de l'esprit jouit sur cette œuvre, du seul fait de sa création, d'un droit de propriété incorporelle exclusif et opposable à tous."*

**En clair :** Dès que vous créez une œuvre originale (texte, musique, code...), vous en êtes automatiquement propriétaire. **Pas besoin de dépôt, d'enregistrement ou de formalité.**

### I.B. Les Deux Composantes du Droit d'Auteur

Le droit d'auteur se divise en **2 catégories de droits** :

#### 1. Le Droit Moral (art. L121-1)

**Définition :** Droits **personnels** de l'auteur, liés à sa personne.

**Caractéristiques :**
- ⚠️ **Perpétuel** : ne s'éteint jamais (même après la mort)
- ⚠️ **Inaliénable** : ne peut pas être vendu ou cédé
- ⚠️ **Imprescriptible** : ne disparaît jamais par le temps

**Les 4 prérogatives du droit moral :**

| **Droit** | **Signification** | **Exemple Code** |
|---|---|---|
| **Divulgation** | Décider si et quand publier l'œuvre | Choisir de publier ou non son code sur GitHub |
| **Paternité** | Être reconnu comme auteur | Exiger que son nom apparaisse dans les crédits |
| **Respect de l'œuvre** | Interdire les modifications qui dénaturent | Interdire de modifier son code de manière inappropriée |
| **Retrait** | Retirer l'œuvre (avec indemnisation) | Retirer son code d'un projet (rare, coûteux) |

#### 2. Les Droits Patrimoniaux (art. L122-1)

**Définition :** Droits **économiques** permettant d'exploiter l'œuvre.

**Caractéristiques :**
- ✅ **Temporaires** : durent 70 ans après la mort de l'auteur
- ✅ **Cessibles** : peuvent être vendus, cédés, licenciés
- ✅ **Prescriptibles** : disparaissent après un certain délai

**Les 2 droits patrimoniaux principaux :**

| **Droit** | **Signification** | **Exemple Code** |
|---|---|---|
| **Reproduction** | Copier, dupliquer l'œuvre | Copier du code, compiler un logiciel |
| **Représentation** | Communiquer l'œuvre au public | Publier sur GitHub, déployer sur un serveur |

> 💡 **Important pour les développeurs :** Les **droits patrimoniaux** sont souvent **cédés à l'employeur** par le contrat de travail. Mais le **droit moral** reste toujours à l'auteur.

### I.C. Durée de Protection

**Durée générale :**
- **70 ans** après la mort de l'auteur (art. L123-1)
- Ensuite, l'œuvre entre dans le **domaine public** (libre d'utilisation)

**Exemples :**
- Code écrit par un développeur décédé en 2024 → protégé jusqu'en 2094
- Shakespeare (mort en 1616) → domaine public depuis 1686

**Exception : œuvres collectives**
- 70 ans après publication (pour les logiciels développés en équipe par une entreprise)

### I.D. Conditions de Protection

Pour être protégée, une œuvre doit être :

1. **Originale** : refléter la personnalité de l'auteur (choix créatifs)
2. **Mise en forme** : concrétisée, pas juste une idée

**Pour le code source :**
- ✅ **Protégé** : la manière dont le code est écrit (syntaxe, structure, algorithmes originaux)
- ❌ **Non protégé** : les fonctionnalités (idées), les algorithmes standards, les langages de programmation

**Exemple :**
- ✅ Protégé : Votre implémentation originale d'un algorithme de tri
- ❌ Non protégé : L'idée de trier des données, l'algorithme quicksort lui-même (domaine public)

---

![Schéma du droit d'auteur : au centre "Œuvre originale", à gauche "Droit moral" (perpétuel, inaliénable : paternité, respect, divulgation, retrait), à droite "Droits patrimoniaux" (70 ans, cessibles : reproduction, représentation)]

*Légende : Les deux composantes du droit d'auteur*

---

## 📖 PARTIE II — Le Code Source et les Logiciels

### II.A. Protection Juridique du Code Source

**Base légale :** Article L112-2 CPI, alinéa 13 :
> *"Sont considérés notamment comme œuvres de l'esprit [...] les logiciels, y compris le matériel de conception préparatoire."*

**Conséquence :** Le code source est protégé **comme une œuvre littéraire** (au même titre qu'un livre ou un poème).

**Ce qui est protégé :**
- ✅ Le code source (fichiers .py, .js, .java...)
- ✅ Le code objet (compilé, binaire)
- ✅ La documentation technique
- ✅ Les maquettes (wireframes, mockups)
- ✅ Les bases de données (si structure originale)

**Ce qui n'est PAS protégé :**
- ❌ Les fonctionnalités (idées)
- ❌ Les langages de programmation (Python, Java sont libres)
- ❌ Les algorithmes standards (tri, recherche...)
- ❌ Les interfaces (débat : Oracle vs Google sur les API Java)

### II.B. Droits du Développeur Salarié (art. L113-9 CPI)

**Règle générale :** Les droits patrimoniaux sur le code écrit par un **salarié** dans le cadre de son travail sont **automatiquement cédés à l'employeur**.

**Texte de loi (L113-9) :**
> *"Sauf dispositions statutaires ou stipulations contraires, les droits patrimoniaux sur les logiciels et leur documentation créés par un ou plusieurs employés dans l'exercice de leurs fonctions [...] sont dévolus à l'employeur qui est seul habilité à les exercer."*

**En clair :**

| **Situation** | **Propriétaire des Droits** |
|---|---|
| Code écrit **pendant les heures de travail** | ✅ Employeur |
| Code écrit **avec les moyens de l'entreprise** (PC pro, outils pro) | ✅ Employeur |
| Code lié aux **missions professionnelles** | ✅ Employeur |
| Code écrit **chez soi, le soir, sur projet perso, sans lien avec le travail** | ✅ Vous (sauf clause contraire) |

**Attention aux clauses contractuelles :**
- **Clause de cession étendue** : cède TOUS vos développements, même persos → à négocier !
- **Clause de non-concurrence** : interdit de travailler pour un concurrent → limite vos projets persos

**Cas particulier : fonctionnaires**
- Statut encore plus restrictif : l'État est propriétaire de TOUTES les créations (même hors service)

### II.C. Le Droit Moral du Développeur Salarié

**Particularité du logiciel :** Le droit moral du développeur salarié est **fortement limité** (art. L121-7 CPI).

**En pratique :**
- ❌ Pas de droit de retrait (l'employeur garde le code)
- ⚠️ Droit de paternité limité (l'employeur peut ne pas citer les développeurs)
- ⚠️ Droit au respect limité (l'employeur peut modifier le code sans demander)

> 💡 **Pourquoi ?** Pour des raisons économiques : une entreprise doit pouvoir exploiter, modifier, maintenir les logiciels sans demander l'autorisation de chaque développeur qui a contribué.

### II.D. Preuve de l'Antériorité

**Problème :** Comment prouver que vous êtes l'auteur d'un code en cas de litige ?

**Solutions :**

| **Méthode** | **Coût** | **Valeur Juridique** |
|---|:---:|:---:|
| **Enveloppe Soleau** (INPI) | 15 € | ⭐⭐⭐ Forte |
| **Dépôt chez APP** (Agence Protection Programmes) | 45 €/an | ⭐⭐⭐ Forte |
| **Commit Git avec horodatage** | Gratuit | ⭐⭐ Moyenne |
| **Email à soi-même (non ouvert)** | Gratuit | ⭐ Faible |
| **Huissier de justice** | 200-500 € | ⭐⭐⭐⭐ Très forte |

**Recommandation pour projets importants :** Enveloppe Soleau ou dépôt APP.

---

## 📖 PARTIE III — Les Licences Logicielles

### III.A. Qu'est-ce qu'une Licence ?

**Définition :** Une licence logicielle est un **contrat** par lequel le titulaire des droits d'auteur **autorise** un tiers à utiliser son logiciel sous certaines **conditions**.

**Analogie :** 
- Acheter un logiciel ≠ acheter les droits d'auteur
- C'est comme louer un appartement : vous pouvez y habiter, mais vous n'êtes pas propriétaire

**Types d'autorisations :**
- ✅ Utiliser (exécuter le logiciel)
- ✅ Copier (installer sur plusieurs machines)
- ✅ Modifier (adapter, corriger)
- ✅ Redistribuer (donner ou vendre à d'autres)

### III.B. Les Grandes Familles de Licences

#### 1. Logiciel Propriétaire (Closed Source)

**Définition :** Le code source est **secret**. L'utilisateur n'a que le droit d'**exécuter** le logiciel.

**Caractéristiques :**
- ❌ Pas d'accès au code source
- ❌ Interdiction de modifier, copier (sauf exceptions)
- ⚠️ Souvent payant (licence commerciale)

**Exemples :** Microsoft Windows, Adobe Photoshop, SAP, Oracle Database

**Avantages :**
- ✅ Support commercial
- ✅ Garanties
- ✅ Interface soignée

**Inconvénients :**
- ❌ Coût élevé
- ❌ Dépendance envers l'éditeur
- ❌ Pas de personnalisation

#### 2. Logiciel Libre (Free Software)

**Définition :** Logiciel qui respecte les **4 libertés fondamentales** (définies par la Free Software Foundation).

**Les 4 libertés :**
0. **Liberté d'exécuter** le programme comme on le souhaite
1. **Liberté d'étudier** le fonctionnement du programme (accès au code source)
2. **Liberté de redistribuer** des copies (gratuitement ou contre paiement)
3. **Liberté de modifier** et de redistribuer les versions modifiées

**Philosophie :** Le logiciel libre est un mouvement **politique et éthique** (liberté, partage, solidarité).

**Figure emblématique :** Richard Stallman (créateur du projet GNU et de la FSF)

#### 3. Open Source

**Définition :** Logiciel dont le code source est **ouvert** et respecte les critères de l'Open Source Initiative (OSI).

**Différence avec le logiciel libre :**
- Logiciel libre = **philosophie éthique** (liberté, droits humains)
- Open source = **approche pragmatique** (qualité, sécurité, collaboration)

> 💡 **En pratique :** Les deux se recoupent largement (90% des licences libres sont aussi open source).

**Avantages de l'open source :**
- ✅ Transparence (sécurité, pas de backdoors)
- ✅ Collaboration mondiale
- ✅ Correction rapide des bugs
- ✅ Personnalisation
- ✅ Gratuit (le plus souvent)

**Inconvénients :**
- ❌ Pas toujours de support officiel
- ❌ Interface parfois moins soignée
- ❌ Risque de fragmentation (forks)

#### 4. Autres Catégories

| **Catégorie** | **Définition** | **Exemples** |
|---|---|---|
| **Freeware** | Gratuit mais source fermé (propriétaire) | WinRAR (version gratuite), Adobe Reader |
| **Shareware** | Gratuit temporairement, puis payant | WinRAR (version complète), Sublime Text |
| **Freemium** | Base gratuite, fonctions avancées payantes | Slack, Trello, GitHub (plans gratuits + pro) |
| **Abandonware** | Logiciel ancien, éditeur disparu (zone grise juridique) | Jeux DOS, Windows 3.1 |

---

### III.C. Les Licences Open Source — Typologie

Il existe **plus de 100 licences** open source. Voici les principales :

#### Licences Permissives (Copyleft Faible ou Nul)

**Principe :** Très peu de contraintes. Vous pouvez presque tout faire (y compris fermer le code).

| **Licence** | **Caractéristiques** | **Obligation** | **Exemples** |
|---|---|---|---|
| **MIT** | Ultra-permissive, 1 page | Inclure la licence MIT | Node.js, jQuery, React |
| **BSD** | Similaire MIT, 3 clauses | Inclure la licence, citer l'auteur | FreeBSD, Nginx |
| **Apache 2.0** | Permissive + clauses brevets | Inclure licence + NOTICE | Android, Kubernetes, Apache HTTP |

**Avantages :**
- ✅ Compatibles avec du code propriétaire
- ✅ Pas de contrainte de redistribution
- ✅ Favorisées par les entreprises

**Utilisation typique :** Librairies, frameworks, outils

#### Licences Copyleft (Viralité)

**Principe :** Si vous distribuez le code (ou un logiciel qui l'utilise), vous devez redistribuer TOUT sous la même licence (y compris vos modifications).

| **Licence** | **Viralité** | **Obligation** | **Exemples** |
|---|:---:|---|---|
| **GPL v2/v3** | ⚠️⚠️⚠️ Forte | Redistribution complète du code source | Linux, GIMP, WordPress |
| **LGPL** | ⚠️ Modérée | Redistribution seulement de la bibliothèque modifiée | Qt, LibreOffice |
| **AGPL** | ⚠️⚠️⚠️⚠️ Très forte | Même pour du SaaS (accès distant) | MongoDB (ancien), Nextcloud |

**GPL = "Viral" :** Si vous utilisez du code GPL dans votre projet, TOUT votre projet devient GPL.

**Exemple :**
```
Projet propriétaire (commercial)
  + Librairie GPL
  ────────────────────────────────
  = TOUT le projet doit être GPL
  = Obligation de fournir TOUT le code source
```

**LGPL = "GPL Light" :**
- Permet d'utiliser la librairie LGPL dans un logiciel propriétaire
- Mais si vous modifiez la librairie LGPL, vous devez redistribuer ces modifications

**AGPL = "GPL pour le Cloud" :**
- Même si vous n'**distribuez** pas le logiciel (juste accès web/API)
- Vous devez quand même fournir le code source aux utilisateurs

**Utilisation typique :** Systèmes d'exploitation, outils GNU, logiciels idéologiques

#### Tableau Comparatif Rapide

| **Critère** | **MIT / BSD** | **Apache 2.0** | **LGPL** | **GPL** | **AGPL** |
|---|:---:|:---:|:---:|:---:|:---:|
| **Utilisation commerciale** | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Modification** | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Redistribution modifs** | ⚠️ Optionnel | ⚠️ Optionnel | 🔴 Obligatoire (librairie) | 🔴 Obligatoire (tout) | 🔴 Obligatoire (tout) |
| **Compatible propriétaire** | ✅ Oui | ✅ Oui | ✅ Oui | ❌ Non | ❌ Non |
| **Viralité** | ❌ Aucune | ❌ Aucune | ⚠️ Faible | 🔴 Forte | 🔴 Très forte |
| **Clause brevets** | ❌ | ✅ | ❌ | ⚠️ (v3) | ✅ |

---

### III.D. Dual Licensing (Double Licence)

**Définition :** Un même logiciel proposé sous **deux licences différentes** :
- Une licence **open source** (GPL) → gratuite
- Une licence **commerciale** (propriétaire) → payante

**Avantages :**
- ✅ Open source pour la communauté (transparence, contributions)
- ✅ Revenu commercial pour l'éditeur (entreprises qui ne veulent pas GPL)

**Exemples :**
- **MySQL** : GPL (gratuit) OU Commerciale (payant)
- **Qt** : LGPL (gratuit) OU Commerciale (payant)
- **Elasticsearch** (ancien modèle) : Apache OU Commerciale

---

### III.E. Comment Choisir une Licence pour Son Projet ?

**Outil recommandé :** [choosealicense.com](https://choosealicense.com) (par GitHub)

**Arbre de décision simplifié :**

```
Vous voulez que votre code soit réutilisé librement ?
│
├─ OUI → Vous voulez forcer le partage des modifications ?
│         │
│         ├─ OUI → GPL v3 (viralité forte, idéologique)
│         │
│         └─ NON → MIT ou Apache 2.0 (permissif, pragmatique)
│
└─ NON → Pas de licence (tous droits réservés)
          OU Licence propriétaire
```

**Recommandations selon le contexte :**

| **Contexte** | **Licence Recommandée** | **Raison** |
|---|---|---|
| Librairie / Framework | MIT, Apache | Adoption maximale, compatibilité |
| Système / OS | GPL | Protéger contre l'appropriation |
| Projet personnel / Portfolio | MIT | Simple, universel |
| Startup (avant pivot) | Propriétaire ou MIT | Flexibilité |
| Logiciel SaaS | AGPL (si idéologique) | Forcer le partage du code serveur |

---

![Schéma des licences : axe horizontal "Permissivité" (MIT/BSD très permissif à gauche, GPL/AGPL restrictif à droite), exemples de projets positionnés sur l'axe]

*Légende : Spectre de permissivité des licences open source*

---

## 📖 PARTIE IV — Contrefaçon et Plagiat de Code

### IV.A. Définition de la Contrefaçon (art. L335-2 CPI)

**Définition :** Toute **reproduction, représentation ou diffusion** d'une œuvre protégée **sans autorisation** de l'auteur.

**Pour le code :** Copier du code sans respecter la licence = contrefaçon.

**Sanctions pénales (art. L335-2) :**
- **3 ans de prison**
- **300 000 € d'amende**
- Possibilité de **saisie** du matériel informatique

**Sanctions civiles :**
- **Dommages et intérêts** (préjudice subi par l'auteur)
- **Publication du jugement** (atteinte à la réputation)
- **Destruction des copies** illicites

### IV.B. Cas de Contrefaçon Fréquents

| **Situation** | **Contrefaçon ?** | **Risque** |
|---|:---:|---|
| Copier du code Stack Overflow sans citer | ⚠️ Oui (licence CC BY-SA) | Moyen |
| Utiliser du code GPL dans un logiciel propriétaire | 🔴 Oui | Élevé |
| Copier une fonction de 10 lignes d'un projet MIT sans licence | ⚠️ Risqué | Faible (mais inclure MIT) |
| Reprendre l'intégralité d'un projet sans licence | 🔴 Oui | Très élevé |
| Reverse engineering d'un logiciel propriétaire | 🔴 Généralement oui (sauf exceptions) | Élevé |

### IV.C. Qu'est-ce que le Plagiat de Code ?

**Différence plagiat vs contrefaçon :**
- **Contrefaçon** : copie littérale (même code, caractère pour caractère)
- **Plagiat** : reprise de la structure, de l'algorithme, en **changeant les noms** de variables

**Exemple de plagiat :**

**Code original :**
```python
def calculate_factorial(n):
    if n == 0:
        return 1
    return n * calculate_factorial(n - 1)
```

**Code plagié :**
```python
def compute_fact(number):
    if number == 0:
        return 1
    return number * compute_fact(number - 1)
```

> ⚠️ **Même structure, mêmes choix, juste les noms changés = plagiat**

**Outils de détection :**
- [MOSS (Measure Of Software Similarity)](https://theory.stanford.edu/~aiken/moss/) — Utilisé dans les universités
- [JPlag](https://jplag.ipd.kit.edu) — Détection de plagiat académique
- [SonarQube](https://www.sonarqube.org) — Détection de code dupliqué

### IV.D. Exceptions au Droit d'Auteur

Le code de la propriété intellectuelle prévoit des **exceptions** permettant l'utilisation d'œuvres protégées sans autorisation :

| **Exception** | **Définition** | **Exemple Code** |
|---|---|---|
| **Copie privée** | Copie pour usage personnel | Installer un logiciel sur son PC perso |
| **Citation courte** | Courte citation à but pédagogique | Citer 5 lignes de code dans un tutoriel |
| **Analyse / étude** | Décompilation pour interopérabilité | Reverse engineering pour compatibilité |
| **Parodie** | Œuvre humoristique | Rare pour du code |

> ⚠️ **Attention :** Ces exceptions sont **strictement encadrées**. En cas de doute, demander l'autorisation.

### IV.E. Cas Célèbres de Contrefaçon

#### 1. Oracle vs Google (API Java)

**Contexte :** Google a utilisé 11 000 lignes de code des API Java dans Android.

**Débat :** Les API (noms de fonctions, paramètres) sont-elles protégées par le droit d'auteur ?

**Évolution :**
- 2012 : Tribunal → API non protégées
- 2014 : Appel → API protégées (contrefaçon de Google)
- 2016 : Google invoque le "fair use" (usage loyal)
- 2021 : **Cour Suprême USA** → Fair use accepté, Google gagne

**Montant réclamé par Oracle :** 9 milliards $

**Leçon :** Même les noms de fonctions peuvent être protégés (selon les juridictions).

#### 2. SCO vs IBM/Linux (2003-2010)

**Contexte :** SCO (propriétaire d'UNIX) accuse IBM et la communauté Linux d'avoir copié du code UNIX dans le noyau Linux.

**Résultat :** Après 7 ans de procès, les tribunaux rejettent les demandes de SCO. Linux est déclaré propre.

**Leçon :** La communauté open source a su prouver l'origine indépendante de son code.

### IV.F. Comment Éviter la Contrefaçon ?

**10 Règles d'Or :**

1. ✅ **Toujours vérifier la licence** avant d'utiliser du code tiers
2. ✅ **Lire les fichiers LICENSE** des projets GitHub
3. ✅ **Citer les auteurs** (même pour des licences permissives)
4. ✅ **Respecter les obligations** (redistribution, mention de modifications...)
5. ✅ **Utiliser des outils** de scan de licences (FOSSA, Black Duck)
6. ✅ **Former les développeurs** aux bonnes pratiques
7. ✅ **Documenter l'origine** du code (commentaires : "Source : URL")
8. ✅ **Éviter Stack Overflow copy-paste** sans comprendre (et vérifier licence CC BY-SA)
9. ✅ **Consulter le service juridique** en cas de doute (ESN, grandes entreprises)
10. ✅ **Privilégier les licences permissives** (MIT, Apache) pour minimiser les risques

---

## 🔑 VOCABULAIRE CLÉ À MAÎTRISER (pour l'examen)

| **Terme** | **Définition Simple** |
|---|---|
| **Droit d'auteur** | Droit de propriété intellectuelle sur les œuvres de l'esprit |
| **Droit moral** | Droits personnels de l'auteur (perpétuels, inaliénables) |
| **Droits patrimoniaux** | Droits économiques (70 ans, cessibles) |
| **Code source** | Fichiers texte écrits dans un langage de programmation |
| **Logiciel propriétaire** | Code source fermé, utilisation restreinte |
| **Logiciel libre** | Respecte les 4 libertés (exécuter, étudier, redistribuer, modifier) |
| **Open source** | Code source ouvert, approche pragmatique |
| **Licence** | Contrat autorisant l'utilisation d'un logiciel sous conditions |
| **GPL** | GNU General Public License (copyleft fort, viral) |
| **MIT** | Licence très permissive, peu de contraintes |
| **Copyleft** | Principe de viralité (modifications redistribuées sous même licence) |
| **Contrefaçon** | Reproduction illicite d'une œuvre protégée |
| **Plagiat** | Reprise de la structure/idées sans copie littérale |

---

## ✅ Points Clés à Retenir

1. **Le code source est protégé par le droit d'auteur dès sa création** (pas besoin de dépôt).

2. **Le droit d'auteur = droit moral (perpétuel) + droits patrimoniaux (70 ans).**

3. **Le code écrit au travail appartient à l'employeur** (sauf exceptions).

4. **Il existe 3 grandes familles** : propriétaire (fermé), libre (4 libertés), open source (ouvert).

5. **Les licences open source se divisent en 2 catégories** : permissives (MIT, Apache) et copyleft (GPL, AGPL).

6. **GPL = viralité** : si vous utilisez du GPL, tout devient GPL (incompatible avec du propriétaire).

7. **Pas de licence = tous droits réservés** (plus restrictif que GPL).

8. **Contrefaçon de code = risque pénal** (3 ans, 300 000 €) + civil (dommages et intérêts).

9. **Toujours vérifier la licence avant d'utiliser du code** (fichier LICENSE sur GitHub).

10. **En tant que technicien SISR, vous devez respecter les licences** pour éviter des problèmes juridiques à votre entreprise.

---

## 📚 Pour Aller Plus Loin

**Textes de référence :**
- [Code de la Propriété Intellectuelle](https://www.legifrance.gouv.fr/codes/id/LEGITEXT000006069414/)
- [Choose a License](https://choosealicense.com) (guide GitHub)
- [TLDRLegal](https://tldrlegal.com) (licences simplifiées)

**Organisations :**
- [Free Software Foundation](https://www.fsf.org) (philosophie du libre)
- [Open Source Initiative](https://opensource.org) (définition open source)

**Questions de réflexion :**
- Faut-il mettre tout son code en open source pour contribuer à la communauté ?
- Comment les entreprises peuvent-elles gagner de l'argent avec l'open source ?
- Les brevets logiciels (interdits en Europe, autorisés aux USA) sont-ils une bonne chose ?


---
