---
author: YLP
title: 📚 FICHE DE COURS
---

# 📚 FICHE DE COURS ÉLÈVE
## Droit des Réseaux : Neutralité du Net et Responsabilité des Hébergeurs

*Version 1.0 — BTS SIO SISR — Année 1 — Semaine 5*

---

## 🎯 Objectifs de Cette Fiche

À la fin de ce cours, vous serez capable de :
- ✅ Définir la neutralité du net et ses exceptions
- ✅ Distinguer FAI, hébergeur, éditeur, plateforme
- ✅ Expliquer les régimes de responsabilité (LCEN, DSA)
- ✅ Identifier les obligations légales des hébergeurs
- ✅ Analyser des cas concrets de blocage ou de retrait de contenus


---

## 📖 PARTIE I — La Neutralité du Net

### I.A. Définition

La **neutralité du net** (ou neutralité d'Internet) est un principe selon lequel **tous les flux de données sur Internet doivent être traités de manière égale**, sans discrimination, restriction ou interférence, quels que soient :
- L'**expéditeur** (qui envoie les données)
- Le **destinataire** (qui reçoit les données)
- Le **type de contenu** (vidéo, texte, mail, jeux en ligne...)
- L'**équipement** utilisé (ordinateur, smartphone, tablette...)
- L'**application** ou le **service** (Netflix, YouTube, Twitch, jeux vidéo...)

> 💡 **En résumé :** Les Fournisseurs d'Accès Internet (FAI) doivent laisser passer **tout le trafic** sans favoritisme ni blocage (sauf exceptions légales).

### I.B. Les Trois Principes Fondamentaux

| **Principe** | **Signification** | **Exemple** |
|---|---|---|
| **1. Pas de blocage** | Un FAI ne peut pas bloquer l'accès à un site ou un service légal | ❌ Free ne peut pas bloquer Netflix parce qu'il concurrence Freebox TV |
| **2. Pas de ralentissement** | Un FAI ne peut pas ralentir certains services | ❌ Orange ne peut pas brider YouTube pour favoriser sa propre plateforme vidéo |
| **3. Pas de priorisation payante** | Un FAI ne peut pas faire payer un service (ex : Netflix) pour être plus rapide | ❌ SFR ne peut pas proposer une "voie rapide" payante à certains sites |

### I.C. Pourquoi la Neutralité du Net Est Importante ?

**Pour les utilisateurs :**
- ✅ **Liberté d'accès** : tous les contenus sont accessibles de la même manière
- ✅ **Égalité** : pas de discrimination entre services (pas de Netflix "premium" plus rapide)
- ✅ **Innovation** : les nouvelles startups peuvent émerger sans avoir à payer les FAI

**Pour les services en ligne (Netflix, YouTube, startups...) :**
- ✅ **Égalité de traitement** : ils ne sont pas désavantagés face aux géants qui pourraient payer pour être prioritaires
- ✅ **Pas de censure économique** : un FAI ne peut pas bloquer un concurrent

**Pour la démocratie :**
- ✅ **Liberté d'expression** : pas de censure arbitraire des FAI
- ✅ **Pluralisme** : diversité des contenus accessibles

### I.D. Les Exceptions à la Neutralité du Net

La neutralité du net **n'est pas absolue**. Des exceptions sont prévues par la loi :

| **Exception Autorisée** | **Justification** | **Exemple** |
|---|---|---|
| **Décision de justice** | Un juge ordonne le blocage d'un site illégal | Blocage de sites de streaming pirate (ex : The Pirate Bay) |
| **Sécurité du réseau** | Protection contre les cyberattaques | Blocage d'un site qui envoie du spam massif ou des DDoS |
| **Mesures de gestion du trafic** | Éviter la congestion du réseau (temporaire, exceptionnel) | Ralentir temporairement le P2P en cas de saturation |
| **Protection de l'ordre public** | Lutte contre le terrorisme, pédopornographie | Blocage de sites djihadistes ou pédophiles |

> ⚠️ **Important :** Ces exceptions doivent être **proportionnées, temporaires et transparentes**. Un FAI ne peut pas bloquer arbitrairement.

### I.E. Cadre Légal de la Neutralité du Net

**En Europe :**
- **Règlement européen 2015/2120** : impose la neutralité du net dans tous les pays de l'UE
- Entrée en vigueur : **30 avril 2016**
- Tous les FAI européens doivent respecter ce règlement

**En France :**
- **ARCEP** (Autorité de Régulation des Communications Électroniques et des Postes) : autorité qui veille au respect de la neutralité du net
- Les FAI doivent publier des **informations transparentes** sur la gestion du trafic

**Aux États-Unis :**
- Débat permanent : neutralité abolie en 2017, partiellement rétablie en 2024 (varie selon les présidents)

---

![Schéma de la neutralité du net : FAI au centre, tous les services (Netflix, YouTube, sites web, jeux) traités de manière égale, avec même vitesse. Pas de voie rapide payante.]

*Légende : Principe de la neutralité du net — tous les flux sont traités de manière égale*

---

## 📖 PARTIE II — Les Acteurs Techniques d'Internet

### II.A. Les Différents Acteurs

Comprendre **qui fait quoi** sur Internet est essentiel pour comprendre **qui est responsable** en cas de contenu illicite.

| **Acteur** | **Rôle** | **Exemples** |
|---|---|---|
| **FAI (Fournisseur d'Accès Internet)** | Donne accès à Internet (connexion) | Orange, Free, SFR, Bouygues Telecom |
| **Hébergeur** | Stocke des sites web, des données, des serveurs | OVH, AWS, Google Cloud, Gandi |
| **Éditeur de contenu** | Crée et contrôle le contenu d'un site | Lemonde.fr, une entreprise qui gère son site |
| **Plateforme** | Permet aux utilisateurs de publier des contenus | YouTube, Facebook, Twitter/X, TikTok |

### II.B. Le Fournisseur d'Accès Internet (FAI)

**Définition :** Entreprise qui **fournit une connexion à Internet** (box, fibre, 4G/5G).

**Rôle :**
- Vous connecte au réseau Internet
- Achemine les données entre votre ordinateur et les serveurs du monde entier
- **Ne contrôle pas** les contenus qui transitent (principe de neutralité)

**Régime de responsabilité :**
- ✅ **Responsabilité très limitée** : le FAI est un simple "tuyau", il ne peut pas surveiller tout ce qui transite
- ✅ **Obligation de blocage** sur décision de justice uniquement
- ❌ **Pas d'obligation générale de surveillance**

**Exemples de FAI en France :**
- Orange (23 millions d'abonnés)
- Free (13 millions)
- SFR (12 millions)
- Bouygues Telecom (8 millions)

---

### II.C. L'Hébergeur

**Définition :** Entreprise qui **stocke des sites web ou des données** sur des serveurs.

**Rôle :**
- Loue de l'espace de stockage sur ses serveurs
- Fournit la bande passante pour que les sites soient accessibles
- **Ne contrôle pas** le contenu stocké (il ne lit pas ce que vous mettez sur le serveur)

**Régime de responsabilité :**
- ✅ **Responsabilité limitée** si l'hébergeur agit "en simple stockage"
- ✅ **Pas d'obligation générale de surveillance** des contenus
- ⚠️ **Obligation de retrait** d'un contenu illicite **après notification**
- ⚠️ **Obligation de conservation** des données de connexion (logs) pendant 1 an

**Exemples d'hébergeurs :**
- OVH (leader français, 400 000 serveurs)
- AWS (Amazon Web Services)
- Google Cloud
- Microsoft Azure

---

### II.D. L'Éditeur de Contenu

**Définition :** Personne ou organisation qui **crée et contrôle** le contenu d'un site web.

**Rôle :**
- Rédige, publie, modifie, supprime les contenus
- Choisit ce qui est publié
- **Contrôle éditorial complet**

**Régime de responsabilité :**
- ❌ **Responsabilité totale** : l'éditeur est responsable de **tout** ce qu'il publie
- ❌ **Pas d'excuse** : "je ne savais pas" ne fonctionne pas
- ⚠️ Responsabilité **civile** (dommages et intérêts) ET **pénale** (amendes, prison)

**Exemples d'éditeurs :**
- **Lemonde.fr** : Le Monde est éditeur de son site, responsable de tous les articles
- **Une entreprise** qui gère son site corporate : elle est éditeur
- **Un blogueur** qui publie ses articles : il est éditeur de son blog

---

### II.E. La Plateforme

**Définition :** Site ou service qui permet aux **utilisateurs de publier du contenu** (UGC = User Generated Content).

**Rôle :**
- Héberge des contenus créés par les utilisateurs (vidéos, posts, commentaires...)
- Met à disposition des outils de publication
- Modère (ou non) les contenus

**Régime de responsabilité :**
- ✅ **Responsabilité limitée** (comme un hébergeur) SI la plateforme ne modifie pas le contenu et ne le sélectionne pas
- ⚠️ **Responsabilité accrue** si la plateforme a un rôle éditorial (algorithmes de recommandation, modération proactive...)
- ⚠️ **Nouvelles obligations avec le DSA** (2024) : retrait rapide, transparence, signalement facile

**Exemples de plateformes :**
- YouTube (vidéos UGC)
- Facebook / Instagram (posts, photos)
- Twitter / X (tweets)
- TikTok (vidéos courtes)

---

### II.F. Tableau Comparatif des Acteurs

| **Critère** | **FAI** | **Hébergeur** | **Éditeur** | **Plateforme** |
|---|:---:|:---:|:---:|:---:|
| **Contrôle du contenu** | ❌ Non | ❌ Non | ✅ Oui | ⚠️ Partiel |
| **Responsabilité** | Très limitée | Limitée | Totale | Limitée → accrue |
| **Obligation de surveillance** | ❌ Non | ❌ Non | ✅ Oui | ⚠️ Partiellement (DSA) |
| **Obligation de retrait** | Décision justice | Sur notification | Immédiate | Sur notification/signalement |

---

![Schéma montrant les 4 acteurs : Utilisateur → FAI (connexion) → Internet → Hébergeur (serveur) → Site (Éditeur ou Plateforme). Distinctions de responsabilité indiquées par des couleurs : FAI et Hébergeur (vert = responsabilité limitée), Éditeur (rouge = responsabilité totale), Plateforme (orange = intermédiaire).]

*Légende : Les différents acteurs techniques et leurs rôles*

---

## 📖 PARTIE III — Les Régimes de Responsabilité

### III.A. La Loi LCEN (2004)

**LCEN** = **Loi pour la Confiance dans l'Économie Numérique** (2004)

C'est la loi française qui régit **la responsabilité des acteurs d'Internet**.

**Texte clé : Article 6**

#### Article 6-I-2 : Responsabilité des FAI

> *"Les personnes dont l'activité est d'offrir un accès à des services de communication au public en ligne [= FAI] ne sont pas responsables des contenus transmis, **sauf si** elles sont à l'origine de la demande de transmission, ou si elles sélectionnent le destinataire ou le contenu."*

**Conséquences :**
- ✅ Un FAI n'est **pas responsable** de ce que vous faites sur Internet
- ⚠️ Sauf s'il modifie ou sélectionne les contenus (ce qui violerait la neutralité du net)

#### Article 6-I-7 : Responsabilité des Hébergeurs

> *"Les personnes qui assurent le stockage de contenus [= hébergeurs] ne sont pas responsables **si** :*
> *1. Elles n'ont pas effectivement connaissance du contenu illicite*
> *2. Ou, dès qu'elles en ont connaissance, elles agissent promptement pour retirer ce contenu."*

**Conséquences :**
- ✅ Un hébergeur n'est **pas responsable** des contenus illicites **tant qu'il n'en a pas connaissance**
- ⚠️ Dès qu'il est **notifié**, il doit **agir rapidement** pour retirer le contenu
- ❌ **Pas d'obligation générale de surveillance** : un hébergeur ne peut pas tout surveiller 24h/24

#### Article 6-I-8 : Pas d'Obligation Générale de Surveillance

> *"Les hébergeurs ne sont soumis à **aucune obligation générale de surveiller** les informations qu'ils stockent."*

**Pourquoi ?**
- Impossible techniquement (millions de sites, milliards de contenus)
- Contraire à la liberté d'expression (surveillance généralisée = censure potentielle)

### III.B. La Procédure de Notification (Article 6-I-5 LCEN)

Pour qu'un hébergeur soit **obligé de retirer un contenu**, il faut une **notification formelle** contenant :

1. **Date de la notification**
2. **Identité du notifiant** (nom, adresse, email)
3. **Description du contenu litigieux** (URL exacte, capture d'écran...)
4. **Motif du retrait** (quel texte de loi est violé : diffamation, contrefaçon, apologie du terrorisme...)
5. **Copie de la correspondance** avec l'auteur du contenu (si possible)

> ⚠️ **Attention :** Une simple plainte par email ne suffit pas. La notification doit être **complète et formelle**.

**Délai de retrait :**
- **Aucun délai légal précis** dans la LCEN
- Jurisprudence : l'hébergeur doit agir **"promptement"** (généralement sous 24-48h)
- **Exception pédopornographie/terrorisme** : retrait **immédiat** (sous 1h avec le DSA)

### III.C. Le DSA (Digital Services Act) — 2024

**DSA** = **Règlement européen sur les services numériques** (entré en vigueur le 17 février 2024)

**Objectif :** Harmoniser les règles pour **les plateformes en ligne** dans toute l'Union Européenne.

#### Nouvelles Obligations pour les Plateformes

| **Obligation** | **Détail** |
|---|---|
| **1. Retrait rapide de contenus illicites** | Délai de retrait : **1 heure** pour terrorisme/pédopornographie, **24h** pour le reste |
| **2. Système de signalement facile** | Bouton "Signaler" clair et accessible |
| **3. Transparence** | Publication de rapports sur les retraits de contenus |
| **4. Algorithmes de recommandation** | Les utilisateurs doivent pouvoir désactiver les recommandations personnalisées |
| **5. Vérification des vendeurs** | Sur les marketplaces (Amazon, eBay...), vérifier l'identité des vendeurs |
| **6. Protection des mineurs** | Pas de publicité ciblée pour les mineurs |

#### Très Grandes Plateformes (VLOP = Very Large Online Platforms)

Les plateformes de **plus de 45 millions d'utilisateurs actifs dans l'UE** ont des obligations renforcées :
- YouTube, Facebook, Instagram, TikTok, X (Twitter), Amazon, Google...

**Obligations supplémentaires :**
- Audit annuel des risques (désinformation, haine en ligne...)
- Modération proactive renforcée
- Transparence totale sur les algorithmes

**Sanctions :** Jusqu'à **6 % du chiffre d'affaires mondial** en cas de non-respect.

---

![Schéma de la procédure de notification : 1. Utilisateur signale un contenu illicite, 2. Hébergeur/Plateforme reçoit la notification, 3. Analyse (illicite ou non ?), 4. Retrait sous 24-48h (ou 1h si grave), 5. Conservation des logs (1 an).]

*Légende : Procédure de notification et de retrait d'un contenu illicite*

---

## 📖 PARTIE IV — Obligations Légales des Hébergeurs

### IV.A. Conservation des Données de Connexion (Logs)

**Obligation :** Les hébergeurs et FAI doivent **conserver les données de connexion** pendant **1 an** (LCEN, art. 6-II).

**Données concernées :**
- Identifiant de connexion (login, email)
- Adresse IP utilisée
- Date et heure de connexion
- Type de protocole utilisé

**Données NON concernées :**
- ❌ Le contenu des messages (emails, posts...)
- ❌ L'historique de navigation

**Objectif :** Permettre aux autorités judiciaires de **retrouver l'auteur** d'un contenu illicite en cas d'enquête.

**Qui peut demander ces données ?**
- ✅ Juge d'instruction ou tribunal
- ✅ Police judiciaire (avec autorisation judiciaire)
- ❌ Pas d'accès libre pour n'importe qui

### IV.B. Obligation de Désignation d'un Représentant Légal

Les plateformes doivent désigner un **représentant légal en France** (ou dans l'UE) pour recevoir les notifications.

**Pourquoi ?**
- Faciliter les procédures judiciaires
- Éviter que les plateformes se "cachent" derrière leur siège à l'étranger

### IV.C. Obligation de Transparence (DSA)

Les plateformes doivent publier **tous les 6 mois** :
- Nombre de signalements reçus
- Nombre de contenus retirés
- Motifs de retrait
- Pays d'origine des signalements

**Exemple :** Rapport de transparence de YouTube (Google) : [transparencyreport.google.com](https://transparencyreport.google.com)

---

## 📖 PARTIE V — Cas Pratiques

### Cas 1 : Blocage de Sites Pirate

**Situation :** The Pirate Bay (site de torrents) est bloqué en France sur décision de justice.

**Questions :**
- **Qui bloque le site ?** Les FAI (Orange, Free, SFR...) sur ordre judiciaire
- **Pourquoi ?** Contrefaçon massive (partage illégal de films, séries, musiques...)
- **Est-ce légal ?** Oui, c'est une **exception à la neutralité du net** (décision de justice)
- **Est-ce efficace ?** Partiellement, car les utilisateurs peuvent contourner via VPN ou en changeant de DNS

---

### Cas 2 : Retrait de Vidéos sur YouTube

**Situation :** YouTube retire des vidéos de désinformation sur la santé (ex : fausses infos sur les vaccins).

**Questions :**
- **YouTube est-il obligé de retirer ces vidéos ?** Oui, si elles violent ses CGU (Conditions Générales d'Utilisation) ou si elles sont signalées comme illicites (apologie de pratiques dangereuses)
- **YouTube est-il un hébergeur ou un éditeur ?** Hybride : hébergeur (stockage UGC) + rôle éditorial (algorithmes de recommandation)
- **Responsabilité ?** Limitée, mais avec le DSA, YouTube doit être plus transparent et réactif

---

### Cas 3 : Diffamation sur un Forum

**Situation :** Un utilisateur publie des messages diffamatoires sur un forum hébergé par OVH.

**Questions :**
- **Qui est responsable ?** Prioritairement **l'auteur du message** (diffamation = délit pénal)
- **Et le propriétaire du forum ?** Responsable **SI** il a été notifié et n'a pas retiré le message
- **Et OVH ?** Pas responsable tant qu'il n'a pas été notifié. Dès notification, il doit demander au propriétaire du forum de retirer le message.

---

### Cas 4 : Conservation de Données (Logs)

**Situation :** La police enquête sur une cyberattaque. Elle demande à OVH les logs de connexion d'un serveur suspect.

**Questions :**
- **OVH peut-il refuser ?** Non, si la demande émane d'un juge ou de la police avec autorisation judiciaire
- **Quelles données OVH doit-il fournir ?** Adresse IP, date/heure de connexion, identifiant du compte
- **OVH peut-il fournir le contenu des emails ?** Non, sauf avec une autorisation judiciaire spécifique (secret des correspondances)

---

## 🔑 VOCABULAIRE CLÉ À MAÎTRISER (pour l'examen)

| **Terme** | **Définition Simple** |
|---|---|
| **Neutralité du net** | Principe selon lequel tous les flux Internet doivent être traités de manière égale |
| **FAI** | Fournisseur d'Accès Internet (donne accès à Internet) |
| **Hébergeur** | Entreprise qui stocke des sites web ou des données sur des serveurs |
| **Éditeur** | Personne/organisation qui crée et contrôle le contenu d'un site |
| **Plateforme** | Site permettant aux utilisateurs de publier du contenu (UGC) |
| **LCEN** | Loi pour la Confiance dans l'Économie Numérique (2004) |
| **DSA** | Digital Services Act (Règlement européen 2024 sur les services numériques) |
| **Notification** | Procédure formelle pour signaler un contenu illicite à un hébergeur |
| **Logs** | Fichiers enregistrant les connexions et actions sur un serveur (conservés 1 an) |
| **ARCEP** | Autorité de Régulation des Communications Électroniques (veille à la neutralité du net) |
| **UGC** | User Generated Content (contenu créé par les utilisateurs) |
| **VLOP** | Very Large Online Platform (plateforme de + 45M utilisateurs UE, obligations renforcées DSA) |

---

## ✅ Points Clés à Retenir

1. **La neutralité du net impose aux FAI de traiter tous les flux de manière égale**, sauf exceptions (justice, sécurité, terrorisme).

2. **Les acteurs ont des responsabilités différentes** : FAI et hébergeurs ont une responsabilité limitée, éditeurs ont une responsabilité totale.

3. **La loi LCEN (2004) protège les hébergeurs** : pas de responsabilité tant qu'ils n'ont pas connaissance du contenu illicite, obligation de retrait après notification formelle.

4. **Le DSA (2024) renforce les obligations des plateformes** : retrait rapide (1h pour terrorisme), transparence, protection des mineurs.

5. **Les hébergeurs doivent conserver les logs pendant 1 an** pour permettre aux autorités d'identifier les auteurs de contenus illicites.

6. **En tant que technicien SISR, vous devez connaître ces règles** pour administrer des services (forums, sites web...) dans le respect de la loi.

---

## 📚 Pour Aller Plus Loin

**Textes de loi :**
- [LCEN (2004) sur Legifrance](https://www.legifrance.gouv.fr/loda/id/JORFTEXT000000801164) — Article 6 sur la responsabilité
- [DSA (2024) - Commission Européenne](https://digital-strategy.ec.europa.eu/fr/policies/digital-services-act-package)

**Ressources pédagogiques :**
- [ARCEP — Neutralité du net](https://www.arcep.fr/la-regulation/grands-dossiers-thematiques-transverses/la-neutralite-de-linternet.html)
- [CNIL — Vie privée et Internet](https://www.cnil.fr)

**Questions de réflexion :**
- La neutralité du net est-elle compatible avec la lutte contre les fake news ?
- Faut-il obliger les plateformes à surveiller proactivement tous les contenus ?
- Jusqu'où peut aller la responsabilité d'un hébergeur ?

---
