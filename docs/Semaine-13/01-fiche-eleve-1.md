---
author: YLP
title: 📚 FICHE DE COURS
---

# 📚 FICHE DE COURS ÉLÈVE
## Licences Logicielles (2) : Open Source (GPL, MIT, BSD) et Creative Commons

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 13*

---

## 🎯 Objectifs de Cette Fiche

À la fin de ce cours, vous serez capable de :
- ✅ Comparer en détail GPL, MIT, BSD, Apache (variantes, subtilités)
- ✅ Comprendre et utiliser la matrice de compatibilité des licences
- ✅ Expliquer les différences GPL v2 vs v3, BSD 2-clause vs 3-clause
- ✅ Maîtriser les licences Creative Commons (BY, SA, NC, ND)
- ✅ Choisir la licence appropriée selon le type de contenu et le contexte

---

### 📖 PARTIE I — Approfondissement des Licences Open Source

### I.A. La Famille MIT / BSD (Licences Permissives)

#### 1. MIT License

**Texte complet : ~170 mots, 1 page**

**Caractéristiques :**
- ✅ **Ultra-permissive** : tout est autorisé (usage commercial, modification, redistribution)
- ✅ **Courte et simple** : facile à lire et comprendre
- ❌ **Pas de clause de brevets** : pas de protection explicite contre les litiges de brevets

**Obligations :**
- Inclure la licence MIT dans toute distribution
- Inclure la notice de copyright

**Avantages :**
- Adoption maximale (entreprises l'acceptent facilement)
- Compatible avec presque toutes les autres licences
- Pas de contrainte de redistribution

**Inconvénients :**
- Pas de protection contre l'appropriation (un concurrent peut fermer le code)
- Pas de clause de brevets (risque dans certains contextes)

**Projets célèbres :** Node.js, jQuery, React, Angular, .NET Core, Ruby on Rails

---

#### 2. BSD Licenses (Berkeley Software Distribution)

**Il existe 3 variantes :**

| **Variante** | **Clauses** | **Différence avec MIT** |
|---|:---:|---|
| **BSD 0-clause** | 0 | = Domaine public (comme CC0) |
| **BSD 2-clause** | 2 | Quasi-identique à MIT |
| **BSD 3-clause** | 3 | + Clause de non-endorsement |

**BSD 3-clause — La clause supplémentaire :**

> *"Le nom de l'auteur ne peut pas être utilisé pour promouvoir des produits dérivés sans autorisation écrite."*

**Exemple pratique :**
- ❌ Interdit : "Ce logiciel est basé sur la technologie développée par l'Université de Berkeley" (dans une pub)
- ✅ Autorisé : Citer l'auteur dans les crédits

**Projets célèbres :** FreeBSD, Nginx

**Différence MIT vs BSD 3-clause :**
- MIT : pas de protection du nom
- BSD 3-clause : protection du nom (pas d'endorsement)

---

### I.B. Apache License 2.0 (Permissive + Brevets)

**Texte complet : ~9 pages (vs 1 page pour MIT)**

**Caractéristiques :**
- ✅ **Permissive** : comme MIT/BSD (usage commercial, modification, redistribution)
- ✅ **Clause de licence de brevets** : protection explicite contre les litiges de brevets
- ✅ **Clause NOTICE** : obligation de documenter les modifications

**Obligations :**
- Inclure la licence Apache 2.0
- Inclure le fichier NOTICE s'il existe
- Documenter les modifications apportées
- Conserver les notices de copyright et brevets

**Avantages :**
- **Protection brevets** : si vous utilisez du code Apache, le contributeur ne peut pas vous attaquer pour violation de brevets
- Compatible GPL v3 (mais PAS GPL v2)
- Prisée par les entreprises (Google, Apache Foundation)

**Inconvénients :**
- Plus longue et complexe que MIT
- Incompatible GPL v2 (clause brevets)

**Projets célèbres :** Android, Kubernetes, Hadoop, Apache HTTP, TensorFlow

---

**Comparaison MIT vs Apache 2.0 :**

| **Critère** | **MIT** | **Apache 2.0** |
|---|:---:|:---:|
| **Longueur** | 1 page | 9 pages |
| **Brevets** | ❌ Pas de clause | ✅ Clause explicite |
| **Compatibilité GPL v2** | ✅ Oui | ❌ Non |
| **Compatibilité GPL v3** | ✅ Oui | ✅ Oui |
| **Obligation NOTICE** | ❌ Non | ✅ Oui |

**Quand choisir Apache 2.0 plutôt que MIT ?**
- Projet avec des **algorithmes potentiellement brevetés**
- Contribution de **grandes entreprises** (qui veulent protéger leurs brevets)
- Projet nécessitant une **traçabilité des modifications**

---

### I.C. Les Licences GPL (Copyleft)

#### 1. GPL v2 (1991)

**Texte complet : ~12 pages**

**Principes :**
- ✅ **Copyleft fort** : toute modification doit être redistribuée sous GPL v2
- ✅ **Viralité** : tout code combiné devient GPL v2
- ❌ **Pas de protection brevets explicite**

**"Only" vs "or later" :**
- **GPL v2 only** : UNIQUEMENT la version 2 (ex : Linux)
- **GPL v2 or later** : version 2 OU toute version ultérieure (ex : WordPress)

**Projet emblématique :** Linux Kernel (GPL v2 only, par choix de Linus Torvalds)

---

#### 2. GPL v3 (2007)

**Texte complet : ~15 pages**

**Nouveautés par rapport à v2 :**

| **Ajout** | **Explication** |
|---|---|
| **Anti-DRM (Tivoization)** | Interdit de verrouiller le matériel pour empêcher l'exécution de versions modifiées |
| **Compatibilité Apache 2.0** | GPL v3 est compatible avec Apache 2.0 (pas la v2) |
| **Protection brevets renforcée** | Clause de licence de brevets explicite |
| **Internationalisation** | Meilleure adaptation aux législations non-US |

**Controverse :** Linus Torvalds a refusé de passer Linux en GPL v3, principalement à cause de la clause anti-DRM.

**Projets GPL v3 :** GCC, Bash, GIMP, WordPress (v2 or later, donc accepte v3)

---

#### 3. LGPL (Lesser GPL)

**Principe :** Copyleft **modéré** — compromis entre GPL et MIT.

**Différence avec GPL :**
- GPL : Si vous utilisez du code GPL, TOUT devient GPL
- LGPL : Si vous utilisez une librairie LGPL, SEULE la librairie doit rester LGPL (pas votre code)

**Usage typique :** Librairies que l'on veut voir adoptées, même par du logiciel propriétaire.

**Exemples :** Qt, GTK, GNU C Library (glibc), LibreOffice

**Scénario d'usage :**
```
Application propriétaire
  ↓ (lien dynamique)
Librairie LGPL
  ↓
Résultat : OK, application reste propriétaire
          Mais si vous modifiez la librairie LGPL, ces modifs doivent être LGPL
```

---

#### 4. AGPL (Affero GPL)

**Principe :** GPL v3 **+ clause SaaS (Software as a Service)**.

**Différence avec GPL :**
- GPL : Obligation de redistribuer le code si vous **distribuez** le logiciel
- AGPL : Obligation de redistribuer le code si vous **donnez accès** au logiciel (même par web/API)

**Cas d'usage :**
- Vous créez un logiciel AGPL et le déployez sur votre serveur web
- Les utilisateurs y accèdent via navigateur (pas de téléchargement)
- **Obligation AGPL** : vous devez quand même fournir le code source aux utilisateurs

**Objectif :** Éviter le "ASP loophole" (Application Service Provider) où des entreprises utilisaient du GPL en SaaS sans redistribuer le code.

**Projets AGPL :** Nextcloud, Mastodon, MongoDB (anciennement, maintenant SSPL)

---

![Schéma : Spectre de viralité des licences - MIT/BSD (aucune) ← Apache (aucune) ← LGPL (modérée) ← GPL (forte) ← AGPL (très forte)]

*Légende : Intensité du copyleft selon les licences*

---

## 📖 PARTIE II — Compatibilité des Licences

### II.A. Règles Générales de Compatibilité

#### Règle 1 : Direction du Flux

La compatibilité n'est **PAS symétrique** :
- **Permissive → Copyleft** = ✅ OK (MIT → GPL = OK)
- **Copyleft → Permissive** = ❌ NON (GPL → MIT = IMPOSSIBLE)

**Explication :**
- MIT permet tout (y compris de changer la licence)
- GPL impose que tout reste GPL (viralité)

**Analogie :** Une rue à sens unique.

```
MIT ────✅───→ GPL
    ←───❌─── 
```

#### Règle 2 : La Licence la Plus Restrictive L'Emporte

Si vous combinez plusieurs licences, le résultat final doit respecter la **plus restrictive**.

**Exemple :**
```
Projet :
  - Fichier A (MIT)
  - Fichier B (Apache 2.0)
  - Fichier C (GPL v3)

Résultat : TOUT le projet devient GPL v3
```

#### Règle 3 : Compatibilité des Versions GPL

| **Combinaison** | **Compatible ?** | **Explication** |
|---|:---:|---|
| **GPL v2 + GPL v2** | ✅ Oui | Même licence |
| **GPL v2 + GPL v3** | ⚠️ Dépend | Si "or later" = oui, si "only" = non |
| **GPL v2 + Apache 2.0** | ❌ Non | Clause brevets Apache incompatible v2 |
| **GPL v3 + Apache 2.0** | ✅ Oui | GPL v3 a été conçue pour ça |

---

### II.B. Matrice de Compatibilité (Simplifiée)

**Légende :** 
- ✅ = Compatible (peut combiner)
- ❌ = Incompatible
- ⚠️ = Dépend (conditions)

| **De ↓ Vers →** | **MIT** | **BSD** | **Apache** | **GPL v2** | **GPL v3** | **Propriétaire** |
|---|:---:|:---:|:---:|:---:|:---:|:---:|
| **MIT** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **BSD** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Apache 2.0** | ✅ | ✅ | ✅ | ❌ | ✅ | ✅ |
| **GPL v2 only** | ❌ | ❌ | ❌ | ✅ | ❌ | ❌ |
| **GPL v2 or later** | ❌ | ❌ | ⚠️ | ✅ | ✅ | ❌ |
| **GPL v3** | ❌ | ❌ | ❌ | ⚠️ | ✅ | ❌ |
| **Propriétaire** | ⚠️ | ⚠️ | ⚠️ | ❌ | ❌ | ✅ |

**Comment lire ce tableau :**
- Ligne = Licence du code source
- Colonne = Licence du projet de destination
- Exemple : Apache vers GPL v2 = ❌ (incompatible)

---

### II.C. Cas Pratiques de Compatibilité

#### Cas 1 : Projet Propriétaire + Librairies Open Source

**Situation :** Vous développez un logiciel propriétaire. Quelles librairies pouvez-vous utiliser ?

| **Licence** | **Utilisable ?** | **Condition** |
|---|:---:|---|
| **MIT, BSD, Apache** | ✅ Oui | Inclure les licences |
| **LGPL** | ✅ Oui | Lien dynamique (ne pas modifier la librairie) |
| **GPL** | ❌ Non | Tout deviendrait GPL |

---

#### Cas 2 : Projet GPL + Librairies Tierces

**Situation :** Vous développez un logiciel GPL. Quelles librairies pouvez-vous utiliser ?

| **Licence** | **Utilisable ?** | **Condition** |
|---|:---:|---|
| **MIT, BSD** | ✅ Oui | Aucune (compatibles) |
| **Apache 2.0** | ⚠️ GPL v3 oui, GPL v2 non | Passer en GPL v3 |
| **GPL** | ✅ Oui | Même famille |
| **Propriétaire** | ❌ Non | Incompatible |

---

#### Cas 3 : Dual Licensing (MySQL, Qt)

**Principe :** Proposer le logiciel sous **deux licences** au choix :
- **GPL** (gratuite) → pour projets open source
- **Commerciale** (payante) → pour projets propriétaires

**Exemple MySQL :**
- Gratuit sous GPL v2
- Payant sous licence commerciale Oracle

**Avantage :** Permet à l'entreprise de gagner de l'argent tout en restant open source.

---

## 📖 PARTIE III — Creative Commons (CC)

### III.A. Qu'est-ce que Creative Commons ?

**Définition :** Famille de licences pour **contenus non-logiciels** (textes, images, musiques, vidéos, bases de données).

**Créateur :** Lawrence Lessig (2001)

**Objectif :** Faciliter le partage culturel avec un cadre juridique clair.

> ⚠️ **Important :** Creative Commons n'est **PAS conçu** pour du logiciel. Pour du code, utiliser des licences open source (MIT, GPL...).

---

### III.B. Les 4 Conditions Creative Commons

Les licences CC se construisent par **combinaison de 4 conditions** :

| **Condition** | **Symbole** | **Signification** |
|---|:---:|---|
| **BY** (Attribution) | ![BY] | Citer l'auteur (obligatoire dans toutes les CC sauf CC0) |
| **SA** (Share Alike) | ![SA] | Partager à l'identique (même licence pour œuvres dérivées) |
| **NC** (Non Commercial) | ![NC] | Pas d'usage commercial |
| **ND** (No Derivatives) | ![ND] | Pas de modification |

---

### III.C. Les 6 Licences Creative Commons

Les 4 conditions se combinent pour former **6 licences principales** + **2 outils** :

#### Licences Standard (du plus permissif au plus restrictif)

| **Licence** | **Conditions** | **Permet** | **Interdit** | **Usage** |
|---|:---:|---|---|---|
| **CC BY** | BY | Tout (y compris commercial et modif) | — | Max. permissif |
| **CC BY-SA** | BY + SA | Tout, mais dérivés sous même licence | — | Wikipédia |
| **CC BY-ND** | BY + ND | Usage commercial, pas de modif | Modifications | Rare |
| **CC BY-NC** | BY + NC | Modifs OK, pas commercial | Commercial | Photos, musiques |
| **CC BY-NC-SA** | BY + NC + SA | Modifs sous même licence, pas commercial | Commercial | Éducation |
| **CC BY-NC-ND** | BY + NC + ND | Juste partager, rien d'autre | Commercial + Modifs | Très restrictif |

#### Outils Spéciaux

| **Outil** | **Signification** |
|---|---|
| **CC0** (Zero) | Domaine public (renonciation à tous les droits) |
| **Public Domain Mark** | Marque du domaine public (œuvres anciennes) |

---

### III.D. Comparaison CC BY-SA vs GPL

| **Critère** | **CC BY-SA** | **GPL** |
|---|---|---|
| **Type de contenu** | Textes, images, vidéos | Code logiciel |
| **Viralité** | Oui (Share Alike) | Oui (Copyleft) |
| **Compatible ?** | ⚠️ **NON** (en général) | — |
| **Exemple** | Wikipédia | Linux |

> ⚠️ **Attention :** CC BY-SA et GPL ne sont **PAS compatibles** ! Ne pas mélanger du code GPL avec de la doc CC BY-SA dans un même projet (sauf cas spécifiques).

---

### III.E. Cas d'Usage Creative Commons

| **Type de Contenu** | **Licence Recommandée** | **Raison** |
|---|---|---|
| **Photos perso (portfolio)** | CC BY | Partage maximal + crédit |
| **Documentation technique** | CC BY-SA | Partage + amélioration communautaire |
| **Musique (artiste amateur)** | CC BY-NC-SA | Protège contre exploitation commerciale |
| **Vidéo éducative** | CC BY ou CC BY-SA | Réutilisation en classe |
| **Base de données scientifiques** | CC0 | Domaine public, science ouverte |
| **Logo d'entreprise** | ❌ Pas de CC | Utiliser copyright classique |

---

### III.F. Où Trouver des Ressources Creative Commons ?

| **Plateforme** | **Type** | **Licences** |
|---|---|---|
| **Wikipédia** | Textes | CC BY-SA |
| **Wikimedia Commons** | Images, vidéos | Variées (CC BY, CC BY-SA) |
| **Unsplash** | Photos | Unsplash License (type CC0) |
| **Flickr** | Photos | Variées (filtrer par licence) |
| **YouTube** | Vidéos | Certaines sous CC BY |
| **OpenStreetMap** | Cartes | ODbL (similaire CC BY-SA) |

---

![Schéma : Les 6 licences CC en cercles concentriques - CC BY au centre (plus permissif), CC BY-NC-ND en périphérie (plus restrictif)]

*Légende : Hiérarchie de permissivité des licences Creative Commons*

---

## 📖 PARTIE IV — Choisir une Licence : Arbres de Décision

### IV.A. Arbre de Décision — Licences Logicielles

```
Quel type de projet ?
│
├─ Logiciel PROPRIÉTAIRE (code fermé)
│   → Licence propriétaire (EULA personnalisée)
│
├─ Librairie / Framework (adoption max)
│   │
│   ├─ Brevets importants ? OUI → Apache 2.0
│   └─ Brevets importants ? NON → MIT ou BSD
│
├─ Projet idéologique (protéger contre appropriation)
│   │
│   ├─ SaaS (accès web) → AGPL v3
│   ├─ Logiciel classique → GPL v3
│   └─ Librairie (adoption + protection) → LGPL
│
└─ Projet perso (portfolio)
    → MIT (simple et universel)
```

---

### IV.B. Arbre de Décision — Creative Commons

```
Quel type de contenu ?
│
├─ CODE LOGICIEL
│   → ❌ Pas de CC, utiliser MIT/GPL/Apache
│
├─ Contenu NON-CODE (image, texte, vidéo, musique)
│   │
│   ├─ Accepter usage commercial ?
│   │   │
│   │   ├─ OUI → Accepter modifications ?
│   │   │         │
│   │   │         ├─ OUI → Imposer même licence ?
│   │   │         │         │
│   │   │         │         ├─ OUI → CC BY-SA
│   │   │         │         └─ NON → CC BY
│   │   │         │
│   │   │         └─ NON → CC BY-ND
│   │   │
│   │   └─ NON → Accepter modifications ?
│   │             │
│   │             ├─ OUI → CC BY-NC-SA (ou CC BY-NC)
│   │             └─ NON → CC BY-NC-ND
│   │
│   └─ Domaine public total → CC0
```

---

### IV.C. Outils de Choix de Licence

| **Outil** | **URL** | **Usage** |
|---|---|---|
| **Choose a License** | [choosealicense.com](https://choosealicense.com) | Licences logicielles (GitHub) |
| **CC License Chooser** | [creativecommons.org/choose](https://creativecommons.org/choose/) | Licences Creative Commons |
| **TLDRLegal** | [tldrlegal.com](https://tldrlegal.com) | Résumés de licences |

---

## 🔑 VOCABULAIRE CLÉ À MAÎTRISER (pour l'examen)

| **Terme** | **Définition Simple** |
|---|---|
| **Compatibilité de licences** | Possibilité de combiner du code sous différentes licences |
| **Viralité / Copyleft** | Obligation de redistribuer les modifications sous la même licence |
| **GPL v2 vs v3** | v3 ajoute anti-DRM, compatibilité Apache, brevets renforcés |
| **BSD 3-clause** | BSD + clause de non-endorsement (protection du nom) |
| **Apache 2.0** | Licence permissive + clause de brevets explicite |
| **LGPL** | GPL "light" pour librairies (copyleft modéré) |
| **AGPL** | GPL pour SaaS (obligation même sans distribution) |
| **Dual licensing** | Même logiciel sous 2 licences (GPL + Commercial) |
| **Creative Commons** | Licences pour contenus non-logiciels |
| **CC BY-SA** | Attribution + Partage à l'identique (≈ GPL pour contenus) |
| **CC BY-NC** | Attribution + Pas d'usage commercial |
| **CC0** | Domaine public (renonciation à tous droits) |

---

## ✅ Points Clés à Retenir

1. **MIT, BSD, Apache = permissives** → compatibles avec presque tout (même propriétaire).

2. **Apache 2.0 > MIT** pour projets avec enjeux de brevets (clause explicite).

3. **GPL v2 ≠ GPL v3** : v3 compatible Apache, v2 non. Linux = v2 only (choix de Linus).

4. **Compatibilité = unidirectionnelle** : MIT → GPL OK, GPL → MIT NON.

5. **Licence la plus restrictive l'emporte** : MIT + Apache + GPL = Tout GPL.

6. **LGPL = compromis** : permet usage par du propriétaire (librairies).

7. **AGPL = GPL + SaaS** : obligation même si pas de distribution (accès web).

8. **Creative Commons ≠ Licences logicielles** : CC pour contenus (images, textes), pas pour code.

9. **CC BY-SA ≈ GPL** : partage à l'identique (copyleft pour contenus).

10. **CC0 = domaine public** : renonciation totale aux droits.

---

## 📚 Pour Aller Plus Loin

**Outils pratiques :**
- [Choose a License](https://choosealicense.com)
- [Creative Commons Chooser](https://creativecommons.org/choose/)
- [GNU License List](https://www.gnu.org/licenses/license-list.html)

**Lectures recommandées :**
- [The Cathedral and the Bazaar](http://www.catb.org/~esr/writings/cathedral-bazaar/) (Eric S. Raymond)
- [Why GPL v3](https://www.gnu.org/licenses/rms-why-gplv3.html) (Richard Stallman)

**Questions de réflexion :**
- Pourquoi Linus Torvalds refuse-t-il de passer Linux en GPL v3 ?
- Peut-on créer un business model viable avec de l'open source ?
- Faut-il utiliser CC BY-SA ou CC BY pour de la documentation technique ?

---
