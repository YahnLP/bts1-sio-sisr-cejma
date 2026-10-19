# Cours – Gestion des incidents : processus, priorités, SLA et indicateurs

*BTS SIO SISR 1re année – CEJMA – S09 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S03 (indicateurs), S08 (service desk, niveaux de support)

## À la fin de ce cours tu sauras

- [ ] Distinguer **incident, problème, demande, changement**
- [ ] Décrire les **étapes du processus** et rédiger un **ticket** utile
- [ ] Appliquer la **matrice impact × urgence** et un **SLA**
- [ ] Calculer **taux de respect, MTTR, disponibilité**
- [ ] Expliquer l'**effet d'expérience** et le **retour d'expérience**

## I. Le vocabulaire

| Terme | Définition | Exemple |
|---|---|---|
| **Incident** | **Interruption** ou **dégradation** non prévue d'un service | L'ERP est inaccessible |
| **Demande de service** | Demande **prévue** et **standard** d'un utilisateur | Commander un écran, créer un compte |
| **Problème** | **Cause** (inconnue) d'un ou plusieurs incidents | Un pilote réseau défectueux provoque des coupures répétées |
| **Changement** | Ajout, modification ou retrait d'un élément du système | Mise à jour d'un serveur |
| **Ticket** | **Fiche de suivi** d'un incident ou d'une demande | Numéro, date, description, priorité, historique |

> [!NOTE]
> On **résout** d'abord l'**incident** (rétablir vite le service) puis on traite le **problème** (supprimer la cause pour éviter qu'il se reproduise).

## II. Le processus de traitement d'un incident

Un **processus** est une **suite d'activités organisées** qui transforme des **entrées** en **résultats** de valeur pour le client.

<figure class="graphe diagramme">
<svg viewBox="0.00 0.00 332.60 783.60" style="max-width:444px" role="img" aria-label="Schéma" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<g class="graph" transform="scale(1 1) rotate(0) translate(10.8 772.8)">
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M207,-762C207,-762 90,-762 90,-762 84,-762 78,-756 78,-750 78,-750 78,-720 78,-720 78,-714 84,-708 90,-708 90,-708 207,-708 207,-708 213,-708 219,-714 219,-720 219,-720 219,-750 219,-750 219,-756 213,-762 207,-762"/>
<text text-anchor="start" x="106.5" y="-740" font-family="Helvetica,sans-Serif" font-size="15.00">1. Détecter</text>
<text text-anchor="start" x="97" y="-723" font-family="Helvetica,sans-Serif" font-size="15.00">et enregistrer</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M192,-649C192,-649 105,-649 105,-649 99,-649 93,-643 93,-637 93,-637 93,-607 93,-607 93,-601 99,-595 105,-595 105,-595 192,-595 192,-595 198,-595 204,-601 204,-607 204,-607 204,-637 204,-637 204,-643 198,-649 192,-649"/>
<text text-anchor="start" x="112" y="-627" font-family="Helvetica,sans-Serif" font-size="15.00">2. Classer</text>
<text text-anchor="start" x="113" y="-610" font-family="Helvetica,sans-Serif" font-size="15.00">catégorie</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M148.5,-707.98C148.5,-693.19 148.5,-674.48 148.5,-658.37"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="151.65,-658.25 148.5,-649.25 145.35,-658.25 151.65,-658.25"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M223.5,-536C223.5,-536 73.5,-536 73.5,-536 67.5,-536 61.5,-530 61.5,-524 61.5,-524 61.5,-494 61.5,-494 61.5,-488 67.5,-482 73.5,-482 73.5,-482 223.5,-482 223.5,-482 229.5,-482 235.5,-488 235.5,-494 235.5,-494 235.5,-524 235.5,-524 235.5,-530 229.5,-536 223.5,-536"/>
<text text-anchor="start" x="108" y="-514" font-family="Helvetica,sans-Serif" font-size="15.00">3. Prioriser</text>
<text text-anchor="start" x="80.5" y="-497" font-family="Helvetica,sans-Serif" font-size="15.00">impact × urgence</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M148.5,-594.98C148.5,-580.19 148.5,-561.48 148.5,-545.37"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="151.65,-545.25 148.5,-536.25 145.35,-545.25 151.65,-545.25"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M218,-423C218,-423 79,-423 79,-423 73,-423 67,-417 67,-411 67,-411 67,-381 67,-381 67,-375 73,-369 79,-369 79,-369 218,-369 218,-369 224,-369 230,-375 230,-381 230,-381 230,-411 230,-411 230,-417 224,-423 218,-423"/>
<text text-anchor="start" x="86" y="-401" font-family="Helvetica,sans-Serif" font-size="15.00">4. Diagnostiquer</text>
<text text-anchor="start" x="105.5" y="-384" font-family="Helvetica,sans-Serif" font-size="15.00">et résoudre</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M148.5,-481.98C148.5,-467.19 148.5,-448.48 148.5,-432.37"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="151.65,-432.25 148.5,-423.25 145.35,-432.25 151.65,-432.25"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M93,-297C93,-297 12,-297 12,-297 6,-297 0,-291 0,-285 0,-285 0,-255 0,-255 0,-249 6,-243 12,-243 12,-243 93,-243 93,-243 99,-243 105,-249 105,-255 105,-255 105,-285 105,-285 105,-291 99,-297 93,-297"/>
<text text-anchor="start" x="19" y="-275" font-family="Helvetica,sans-Serif" font-size="15.00">Escalade</text>
<text text-anchor="start" x="26.5" y="-258" font-family="Helvetica,sans-Serif" font-size="15.00">N2, N3</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M77.08,-368.95C65.27,-361.44 54.59,-351.93 47.5,-340 41.55,-329.98 40.83,-317.64 42.23,-306.18"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="45.34,-306.64 43.74,-297.24 39.13,-305.58 45.34,-306.64"/>
<text text-anchor="start" x="47.5" y="-329.6" font-family="Helvetica,sans-Serif" font-size="13.00">non résolu</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M249.5,-297C249.5,-297 157.5,-297 157.5,-297 151.5,-297 145.5,-291 145.5,-285 145.5,-285 145.5,-255 145.5,-255 145.5,-249 151.5,-243 157.5,-243 157.5,-243 249.5,-243 249.5,-243 255.5,-243 261.5,-249 261.5,-255 261.5,-255 261.5,-285 261.5,-285 261.5,-291 255.5,-297 249.5,-297"/>
<text text-anchor="start" x="164.5" y="-275" font-family="Helvetica,sans-Serif" font-size="15.00">5. Rétablir</text>
<text text-anchor="start" x="167" y="-258" font-family="Helvetica,sans-Serif" font-size="15.00">et vérifier</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M161.17,-368.81C165.48,-359.73 170.28,-349.45 174.5,-340 179.47,-328.86 184.7,-316.61 189.32,-305.56"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="192.34,-306.52 192.89,-297 186.52,-304.1 192.34,-306.52"/>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M94.4,-297.21C105,-305.4 115.6,-315.16 123.5,-326 130.85,-336.09 136.24,-348.57 140.09,-360.13"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="137.08,-361.06 142.74,-368.74 143.1,-359.21 137.08,-361.06"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M273,-184C273,-184 134,-184 134,-184 128,-184 122,-178 122,-172 122,-172 122,-142 122,-142 122,-136 128,-130 134,-130 134,-130 273,-130 273,-130 279,-130 285,-136 285,-142 285,-142 285,-172 285,-172 285,-178 279,-184 273,-184"/>
<text text-anchor="start" x="163.5" y="-162" font-family="Helvetica,sans-Serif" font-size="15.00">6. Clôturer</text>
<text text-anchor="start" x="141" y="-145" font-family="Helvetica,sans-Serif" font-size="15.00">avec l&#39;utilisateur</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M203.5,-242.98C203.5,-228.19 203.5,-209.48 203.5,-193.37"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="206.65,-193.25 203.5,-184.25 200.35,-193.25 206.65,-193.25"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M299,-71C299,-71 108,-71 108,-71 102,-71 96,-65 96,-59 96,-59 96,-12 96,-12 96,-6 102,0 108,0 108,0 299,0 299,0 305,0 311,-6 311,-12 311,-12 311,-59 311,-59 311,-65 305,-71 299,-71"/>
<text text-anchor="start" x="158" y="-49" font-family="Helvetica,sans-Serif" font-size="15.00">Capitaliser :</text>
<text text-anchor="start" x="115" y="-32" font-family="Helvetica,sans-Serif" font-size="15.00">base de connaissances,</text>
<text text-anchor="start" x="132.5" y="-15" font-family="Helvetica,sans-Serif" font-size="15.00">problème éventuel</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M203.5,-129.78C203.5,-115.28 203.5,-96.9 203.5,-80.29"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="206.65,-80.28 203.5,-71.28 200.35,-80.28 206.65,-80.28"/>
</g>
</g>
</svg>
</figure>

À chaque étape, on **communique** avec l'utilisateur (accusé de réception, point d'avancement, clôture).

### Les informations d'un bon ticket

**Qui** a signalé, **quand**, **quoi** (symptôme observé, message d'erreur, capture), **où** (poste, service, site), **depuis quand**, **ce qui a changé**, **impact** (combien de personnes ?), **actions déjà tentées**.

## III. Prioriser : impact et urgence

- **Impact** : **combien** de personnes ou de services sont touchés ?
- **Urgence** : **dans quel délai** faut-il agir ?

| Impact ↓ / Urgence → | **Haute** | **Moyenne** | **Basse** |
|---|---|---|---|
| **Élevé** (plusieurs services, service critique) | **P1** | **P2** | **P3** |
| **Moyen** (un service, un groupe) | **P2** | **P3** | **P4** |
| **Faible** (un utilisateur) | **P3** | **P4** | **P4** |

## IV. Les engagements de service

Le **SLA** (*service level agreement*) est l'**accord de niveau de service** : il fixe des engagements mesurables pour chaque priorité.

| Sigle | Sens |
|---|---|
| **GTI** | **Garantie de temps d'intervention** : délai de **prise en charge** |
| **GTR** | **Garantie de temps de rétablissement** : délai pour **rétablir** le service |

Exemple de grille (en heures **ouvrées**) :

| Priorité | GTI | GTR |
|---|---|---|
| **P1** | 15 minutes | **4 h** |
| **P2** | 1 h | **8 h** |
| **P3** | 4 h | **24 h** |
| **P4** | 8 h | **72 h** |

Les heures **ouvrées** ne comptent que les heures d'ouverture du service (par exemple 8 h–18 h, du lundi au vendredi).

## V. Mesurer le processus

| Indicateur | Calcul | Remarque |
|---|---|---|
| **Taux de respect du SLA** | tickets dans les délais ÷ tickets traités × 100 | Par priorité |
| **MTTR** (*mean time to repair*, temps moyen de réparation) | somme des durées de rétablissement ÷ nombre d'incidents | Plus il baisse, mieux c'est |
| **MTBF** (*mean time between failures*, temps moyen entre pannes) | durée de fonctionnement ÷ nombre de pannes | Plus il augmente, mieux c'est |
| **Disponibilité** | (temps total − arrêt) ÷ temps total, ou **MTBF ÷ (MTBF + MTTR)** | Exprimée en % |

Exemple : MTBF de 720 h et MTTR de 4 h : disponibilité = 720 ÷ 724 = **99,45 %**.

## VI. L'effet d'expérience

Plus on **répète** une activité, plus on devient **efficace**. L'**effet d'expérience** désigne la **baisse du coût unitaire** à mesure que la **production cumulée** augmente. On le modélise parfois par une **courbe à 80 %** : à chaque **doublement** de la production cumulée, le coût unitaire est multiplié par 0,8.

| Production cumulée | 1 | 2 | 4 | 8 |
|---|---|---|---|---|
| **Coût unitaire** (base 100) | 100 | **80** | **64** | **51,2** |

Dans un support, la **base de connaissances**, les **procédures** et la **formation** transforment l'expérience individuelle en **expérience collective**.

## VII. Incident majeur et incident de sécurité

- **Incident majeur** : impact très fort (service critique indisponible) : on **active une cellule de crise**, on désigne un **responsable de l'incident** et un **porte-parole**, on **informe** régulièrement la direction et les utilisateurs.
- **Incident de sécurité** : atteinte à la **confidentialité**, l'**intégrité** ou la **disponibilité** (attaque, fuite). Il suit un processus voisin avec des étapes supplémentaires : **isoler**, **préserver les preuves** (séance 18), **notifier** si des données personnelles sont concernées (séance 15).
- Après un incident majeur, on fait un **retour d'expérience** (analyse **sans chercher de coupable**) : chronologie, causes, ce qui a bien fonctionné, actions d'amélioration.

## À retenir

- **Incident** (rétablir), **problème** (supprimer la cause), **demande** (prévue), **changement** (modification).
- Processus : enregistrer, classer, **prioriser (impact × urgence)**, diagnostiquer, escalader, rétablir, **clôturer**, **capitaliser**.
- **SLA**, **GTI**, **GTR** ; indicateurs : respect du SLA, **MTTR**, **MTBF**, **disponibilité**.
- **Effet d'expérience** : le coût unitaire baisse quand la production cumulée augmente.
- **Incident majeur** : cellule de crise ; **retour d'expérience** sans chercher de coupable.
