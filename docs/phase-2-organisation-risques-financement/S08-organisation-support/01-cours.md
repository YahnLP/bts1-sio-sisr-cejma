# Cours – Ressources, organisation, management et service de support

*BTS SIO SISR 1re année – CEJM et CEJMA – S08 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S03 (indicateurs), S05 (faire ou faire-faire)

## À la fin de ce cours tu sauras

- [ ] Classer les **ressources** et décrire les **compétences**
- [ ] Distinguer **structures** et **mécanismes de coordination**
- [ ] Reconnaître les **niveaux** et les **styles** de management
- [ ] Décrire le **service desk** et les **niveaux N1, N2, N3**
- [ ] Calculer l'effet d'une amélioration du niveau 1 sur le coût

## I. Les ressources de l'entreprise

Pour fonctionner, une entreprise mobilise des **ressources**, qu'elle doit **organiser**.

| Type | Définition | Exemples dans un service informatique |
|---|---|---|
| **Tangibles** (matérielles) | On peut les **toucher** | Serveurs, postes, réseau, locaux |
| **Intangibles** (immatérielles) | On ne les touche pas, mais elles ont de la **valeur** | Logiciels, bases de connaissances, marque, **savoir-faire**, brevets, données |
| **Humaines** | Les personnes et leurs **compétences** | Techniciens, experts, responsable |
| **Financières** | Moyens de payer et d'investir | Budget, trésorerie |

Une **compétence** est la capacité à **mobiliser** des connaissances, des savoir-faire et des comportements pour réussir une tâche. Une organisation **combine** ressources et compétences pour créer un **avantage** durable.

## II. Organiser : structure, coordination, contrôle

### La structure

La **structure** répartit le travail et les responsabilités.

| Structure | Principe | Avantage | Limite |
|---|---|---|---|
| **Fonctionnelle** | Services par **fonction** (production, commercial, informatique…) | Expertise, clarté | Cloisonnement |
| **Divisionnelle** | Une unité par **produit, marché ou zone** | Proche du client | Doublons |
| **Matricielle** | Chaque personne dépend d'un **chef de fonction** et d'un **chef de projet** | Souplesse, projets | Double hiérarchie, conflits |

### Les mécanismes de coordination

Quand plusieurs personnes travaillent ensemble, il faut les **coordonner**. Mintzberg distingue cinq mécanismes :

| Mécanisme | Principe | Exemple |
|---|---|---|
| **Ajustement mutuel** | Les personnes se coordonnent par **échange direct** | Deux techniciens qui se répartissent un incident |
| **Supervision directe** | Un **chef** donne des ordres | Le responsable affecte les tickets |
| **Standardisation des procédés** | On suit la **même procédure** | Procédure d'escalade |
| **Standardisation des résultats** | On fixe les **résultats attendus** | Objectif de 90 % de tickets résolus dans le délai |
| **Standardisation des qualifications** | On s'appuie sur des **formations** communes | Certification de technicien |

### Le contrôle

Le **contrôle** compare les **résultats** aux **objectifs** et déclenche des **actions correctives** (voir les indicateurs de la séance 3).

## III. Manager : niveaux et styles

### Les trois niveaux

| Niveau | Décisions | Horizon | Exemple |
|---|---|---|---|
| **Stratégique** | Orientations globales | Long terme | Choisir de passer au cloud |
| **Tactique** (intermédiaire) | Mise en œuvre des orientations | Moyen terme | Planifier la migration |
| **Opérationnel** | Activités du quotidien | Court terme | Traiter un ticket |

### Les styles de management

| Style | Qui décide ? | Atout | Risque |
|---|---|---|---|
| **Autoritaire** | Le **chef seul**, sans expliquer | Rapide | Démotivation |
| **Persuasif** | Le chef décide, mais **explique** pour convaincre | Adhésion | Participation limitée |
| **Participatif** | Le chef **consulte** l'équipe et décide ensemble | Implication, qualité | Plus lent |
| **Délégatif** | L'équipe **décide** dans un cadre fixé | Autonomie | Risque de dérive sans suivi |

Il n'y a **pas de style idéal** : le choix dépend de la **situation** (urgence, maturité de l'équipe, enjeu).

## IV. Application : organiser un service de support

### Le référentiel ITIL

**ITIL** est un **référentiel de bonnes pratiques** de gestion des services informatiques. Il organise le travail en **pratiques** (gestion des incidents, des problèmes, des changements, des demandes, des niveaux de service…) autour d'un point d'entrée unique : le **service desk**.

### Le service desk et le point de contact unique

Le **service desk** (centre de services, ou **help desk**) est l'interface entre les **utilisateurs** et la DSI : un **point de contact unique** (SPOC) enregistre **tous** les incidents et demandes (téléphone, courriel, portail).

### Les niveaux de support

| Niveau | Rôle | Compétence | Exemples |
|---|---|---|---|
| **N1** | **Accueil**, enregistrement, diagnostic initial, résolution des cas **simples** (procédures, scripts) | Généraliste | Réinitialiser un mot de passe, configurer une imprimante |
| **N2** | Résolution des cas **techniques** | Technicien confirmé | Dépanner un serveur de fichiers, un problème réseau |
| **N3** | Cas **complexes**, **expertise**, lien avec les éditeurs et constructeurs, correction de fond | Expert, architecte | Défaut logiciel, problème d'infrastructure |

L'**escalade** peut être **fonctionnelle** (on passe à un niveau plus expert) ou **hiérarchique** (on prévient un responsable quand l'enjeu ou le délai l'exige).

<figure class="graphe diagramme">
<svg viewBox="0.00 0.00 384.60 632.60" style="max-width:513px" role="img" aria-label="Schéma" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<g class="graph" transform="scale(1 1) rotate(0) translate(10.8 621.8)">
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M123.5,-611C123.5,-611 30.5,-611 30.5,-611 24.5,-611 18.5,-605 18.5,-599 18.5,-599 18.5,-586 18.5,-586 18.5,-580 24.5,-574 30.5,-574 30.5,-574 123.5,-574 123.5,-574 129.5,-574 135.5,-580 135.5,-586 135.5,-586 135.5,-599 135.5,-599 135.5,-605 129.5,-611 123.5,-611"/>
<text text-anchor="start" x="37.5" y="-589" font-family="Helvetica,sans-Serif" font-size="15.00">Utilisateur</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M142,-515C142,-515 12,-515 12,-515 6,-515 0,-509 0,-503 0,-503 0,-473 0,-473 0,-467 6,-461 12,-461 12,-461 142,-461 142,-461 148,-461 154,-467 154,-473 154,-473 154,-503 154,-503 154,-509 148,-515 142,-515"/>
<text text-anchor="start" x="29" y="-493" font-family="Helvetica,sans-Serif" font-size="15.00">Service desk</text>
<text text-anchor="start" x="19" y="-476" font-family="Helvetica,sans-Serif" font-size="15.00">enregistrement</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M77,-573.65C77,-560.12 77,-541.11 77,-524.53"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="80.15,-524.11 77,-515.11 73.85,-524.11 80.15,-524.11"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M127.5,-402C127.5,-402 26.5,-402 26.5,-402 20.5,-402 14.5,-396 14.5,-390 14.5,-390 14.5,-360 14.5,-360 14.5,-354 20.5,-348 26.5,-348 26.5,-348 127.5,-348 127.5,-348 133.5,-348 139.5,-354 139.5,-360 139.5,-360 139.5,-390 139.5,-390 139.5,-396 133.5,-402 127.5,-402"/>
<text text-anchor="start" x="43.5" y="-380" font-family="Helvetica,sans-Serif" font-size="15.00">Niveau 1</text>
<text text-anchor="start" x="33.5" y="-363" font-family="Helvetica,sans-Serif" font-size="15.00">cas simples</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M77,-460.98C77,-446.19 77,-427.48 77,-411.37"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="80.15,-411.25 77,-402.25 73.85,-411.25 80.15,-411.25"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M166.5,-37C166.5,-37 97.5,-37 97.5,-37 91.5,-37 85.5,-31 85.5,-25 85.5,-25 85.5,-12 85.5,-12 85.5,-6 91.5,0 97.5,0 97.5,0 166.5,0 166.5,0 172.5,0 178.5,-6 178.5,-12 178.5,-12 178.5,-25 178.5,-25 178.5,-31 172.5,-37 166.5,-37"/>
<text text-anchor="start" x="104.5" y="-15" font-family="Helvetica,sans-Serif" font-size="15.00">Clôture</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M75.3,-347.81C74.11,-328.08 72.62,-300.35 72,-276 71.39,-252.01 68.56,-245.75 72,-222 81.43,-157 107.04,-83.81 121.57,-45.72"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="124.54,-46.79 124.84,-37.26 118.66,-44.52 124.54,-46.79"/>
<text text-anchor="start" x="80" y="-182.6" font-family="Helvetica,sans-Serif" font-size="13.00">résolu</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M194,-276C194,-276 104,-276 104,-276 98,-276 92,-270 92,-264 92,-264 92,-234 92,-234 92,-228 98,-222 104,-222 104,-222 194,-222 194,-222 200,-222 206,-228 206,-234 206,-234 206,-264 206,-264 206,-270 200,-276 194,-276"/>
<text text-anchor="start" x="115.5" y="-254" font-family="Helvetica,sans-Serif" font-size="15.00">Niveau 2</text>
<text text-anchor="start" x="111" y="-237" font-family="Helvetica,sans-Serif" font-size="15.00">technique</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M92.27,-347.7C103.01,-329.21 117.48,-304.28 129.12,-284.24"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="131.96,-285.62 133.75,-276.26 126.51,-282.46 131.96,-285.62"/>
<text text-anchor="start" x="115" y="-308.6" font-family="Helvetica,sans-Serif" font-size="13.00">non résolu</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M147.05,-221.79C143.79,-177.99 137.28,-90.41 133.99,-46.26"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="137.13,-46.01 133.32,-37.27 130.85,-46.48 137.13,-46.01"/>
<text text-anchor="start" x="141" y="-119.6" font-family="Helvetica,sans-Serif" font-size="13.00">résolu</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M351,-150C351,-150 225,-150 225,-150 219,-150 213,-144 213,-138 213,-138 213,-108 213,-108 213,-102 219,-96 225,-96 225,-96 351,-96 351,-96 357,-96 363,-102 363,-108 363,-108 363,-138 363,-138 363,-144 357,-150 351,-150"/>
<text text-anchor="start" x="254.5" y="-128" font-family="Helvetica,sans-Serif" font-size="15.00">Niveau 3</text>
<text text-anchor="start" x="232" y="-111" font-family="Helvetica,sans-Serif" font-size="15.00">expert, éditeur</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M178.48,-221.7C199.86,-202.63 228.9,-176.73 251.7,-156.38"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="253.95,-158.6 258.56,-150.26 249.75,-153.9 253.95,-158.6"/>
<text text-anchor="start" x="222" y="-182.6" font-family="Helvetica,sans-Serif" font-size="13.00">non résolu</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M248.23,-95.87C222.98,-79.28 190.63,-58.02 166.47,-42.15"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="168.18,-39.51 158.93,-37.2 164.72,-44.77 168.18,-39.51"/>
</g>
</g>
</svg>
</figure>

### Exemple chiffré : le coût par niveau

Un support traite **1 200 tickets** par mois. Coût moyen d'un ticket : **12 €** en N1, **45 €** en N2, **130 €** en N3.

| | **Situation actuelle** | **Avec une base de connaissances** |
|---|---|---|
| Tickets résolus en N1 | 70 % = **840** | 80 % = **960** |
| Tickets résolus en N2 | 22 % = **264** | 16 % = **192** |
| Tickets résolus en N3 | 8 % = **96** | 4 % = **48** |
| Coût N1 | 840 × 12 = **10 080 €** | 960 × 12 = **11 520 €** |
| Coût N2 | 264 × 45 = **11 880 €** | 192 × 45 = **8 640 €** |
| Coût N3 | 96 × 130 = **12 480 €** | 48 × 130 = **6 240 €** |
| **Total** | **34 440 €** (28,70 € par ticket) | **26 400 €** (22 € par ticket) |

Économie : 34 440 − 26 400 = **8 040 € par mois**, soit **23,3 %**. L'idée : faire **monter le taux de résolution du niveau 1** grâce aux **procédures** et à la **base de connaissances** (standardisation des procédés), plus économique.

## Comprendre pas à pas

### Structure, coordination, contrôle : un schéma de lecture

Pour analyser une organisation, pose trois questions :

| Question | Notion | Exemple de service support |
|---|---|---|
| **Qui fait quoi ?** | **Structure** | Service desk (N1), experts (N2), spécialistes (N3) |
| **Comment s'assure-t-on que tout le monde va dans le même sens ?** | **Coordination** | Outil de tickets, réunions, règles d'escalade |
| **Comment vérifie-t-on ?** | **Contrôle** | Indicateurs : délais, satisfaction, tickets en retard |

### Niveaux de support : un exemple chiffré

Un service reçoit **200 tickets par mois**.

| Niveau | Part des tickets résolus | Tickets |
|---|---:|---:|
| **N1** (service desk) | 70 % | 140 |
| **N2** (techniciens) | 20 % | 40 |
| **N3** (experts) | 10 % | 20 |
| **Total** | **100 %** | **200** |

**Pourquoi c'est efficace :** les experts (les plus coûteux) ne traitent que **10 %** des tickets ; la majorité est résolue au niveau le **moins coûteux**.

> [!WARNING]
> Ces pourcentages sont un **exemple de cours**, pas une norme : ils varient selon le service et la qualité de la base de connaissances.

### Styles de management : quand les utiliser ?

| Style | Quand il convient | Limite |
|---|---|---|
| **Directif** | Urgence, incident majeur | Peu d'initiative |
| **Participatif** | Amélioration du service, équipe expérimentée | Décision plus lente |
| **Délégation** | Équipe autonome et compétente | Besoin d'un contrôle adapté |

Un cas réel d'organisation sans chefs est détaillé dans [Zappos](04-cas-reels.md).

## À retenir

- **Ressources** tangibles, intangibles, humaines, financières ; **compétences** = mobiliser savoirs, savoir-faire, comportements.
- **Structures** fonctionnelle, divisionnelle, matricielle ; **coordination** : ajustement mutuel, supervision directe, standardisation des procédés, des résultats, des qualifications.
- **Niveaux** de management : stratégique, tactique, opérationnel ; **styles** : autoritaire, persuasif, participatif, délégatif ; pas de style idéal.
- **ITIL** : référentiel de bonnes pratiques ; **service desk** = point de contact unique ; **N1, N2, N3** + **escalade**.
- Améliorer le **niveau 1** (procédures, base de connaissances) **réduit le coût**.
