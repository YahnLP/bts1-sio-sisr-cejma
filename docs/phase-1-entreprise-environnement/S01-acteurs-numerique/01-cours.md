# Cours – Agents économiques, acteurs du numérique et modèles économiques

*BTS SIO SISR 1re année – CEJMA – S01 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** Aucun

## À la fin de ce cours tu sauras

- [ ] Nommer les **agents économiques** et décrire leurs échanges
- [ ] Distinguer **DSI, éditeur, ESN, hébergeur, distributeur**
- [ ] Comparer **régie, forfait et infogérance** et dire qui porte le risque
- [ ] Décrire les principaux **modèles économiques** du numérique
- [ ] Calculer et comparer des coûts sur plusieurs années

## I. Les agents économiques et leurs échanges

Une **entreprise** ne vit pas seule : elle échange avec d'autres. L'économie regroupe ces acteurs en cinq grandes familles, les **agents économiques**.

| Agent | Rôle principal | Exemple dans le numérique |
|---|---|---|
| **Ménages** | Consomment, travaillent, épargnent | Un particulier abonné à une messagerie en ligne |
| **Entreprises** | Produisent des biens et des services | Une ESN, un éditeur de logiciels, une PME cliente |
| **Administrations publiques** | Règlent, redistribuent, fournissent des services publics | Une mairie, un ministère, la CNIL |
| **Institutions financières** | Collectent l'épargne, accordent des crédits | Une banque qui finance l'achat d'un parc de serveurs |
| **Reste du monde** | Échangent avec l'économie nationale | Un éditeur américain qui vend ses licences en France |

Ces agents échangent des **flux réels** (biens, services, travail) et des **flux financiers** (paiements, crédits, impôts).

<figure class="graphe diagramme">
<svg viewBox="0.00 0.00 839.10 276.60" style="max-width:1119px;min-width:900px" role="img" aria-label="Schéma" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<g class="graph" transform="scale(1 1) rotate(0) translate(10.8 265.8)">
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M484,-255C484,-255 403,-255 403,-255 397,-255 391,-249 391,-243 391,-243 391,-230 391,-230 391,-224 397,-218 403,-218 403,-218 484,-218 484,-218 490,-218 496,-224 496,-230 496,-230 496,-243 496,-243 496,-249 490,-255 484,-255"/>
<text text-anchor="start" x="410" y="-233" font-family="Helvetica,sans-Serif" font-size="15.00">Ménages</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M493,-146C493,-146 394,-146 394,-146 388,-146 382,-140 382,-134 382,-134 382,-121 382,-121 382,-115 388,-109 394,-109 394,-109 493,-109 493,-109 499,-109 505,-115 505,-121 505,-121 505,-134 505,-134 505,-140 499,-146 493,-146"/>
<text text-anchor="start" x="401" y="-124" font-family="Helvetica,sans-Serif" font-size="15.00">Entreprises</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M390.75,-232.31C360.5,-227.45 324.82,-215.9 305.5,-189 283.87,-158.89 328.49,-143.57 372.64,-135.9"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="373.35,-138.98 381.73,-134.42 372.34,-132.76 373.35,-138.98"/>
<text text-anchor="start" x="305.5" y="-178.6" font-family="Helvetica,sans-Serif" font-size="13.00">travail</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M411.23,-217.79C395.7,-206.74 381.93,-191.51 389.5,-175 393.48,-166.31 399.98,-158.63 407.11,-152.15"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="409.5,-154.25 414.38,-146.06 405.46,-149.42 409.5,-154.25"/>
<text text-anchor="start" x="389.5" y="-178.6" font-family="Helvetica,sans-Serif" font-size="13.00">achats</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M444.05,-146.24C444.36,-158.29 444.65,-174.61 444.5,-189 444.43,-195.4 444.31,-202.3 444.17,-208.77"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="441.02,-208.77 443.97,-217.84 447.32,-208.91 441.02,-208.77"/>
<text text-anchor="start" x="445.5" y="-178.6" font-family="Helvetica,sans-Serif" font-size="13.00">salaires</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M483.02,-146.18C500.88,-156.91 516.25,-171.83 507.5,-189 502.77,-198.28 495.24,-206.13 486.97,-212.6"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="485.03,-210.12 479.56,-217.93 488.71,-215.23 485.03,-210.12"/>
<text text-anchor="start" x="510.5" y="-178.6" font-family="Helvetica,sans-Serif" font-size="13.00">biens et services</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M223,-37C223,-37 12,-37 12,-37 6,-37 0,-31 0,-25 0,-25 0,-12 0,-12 0,-6 6,0 12,0 12,0 223,0 223,0 229,0 235,-6 235,-12 235,-12 235,-25 235,-25 235,-31 229,-37 223,-37"/>
<text text-anchor="start" x="19" y="-15" font-family="Helvetica,sans-Serif" font-size="15.00">Administrations publiques</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M381.71,-124.09C271.15,-119.15 48.81,-106.05 25.5,-80 11.42,-64.27 26.61,-50.85 48.44,-40.68"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="49.73,-43.55 56.74,-37.08 47.23,-37.77 49.73,-43.55"/>
<text text-anchor="start" x="25.5" y="-69.6" font-family="Helvetica,sans-Serif" font-size="13.00">impôts, cotisations</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M548.5,-37C548.5,-37 362.5,-37 362.5,-37 356.5,-37 350.5,-31 350.5,-25 350.5,-25 350.5,-12 350.5,-12 350.5,-6 356.5,0 362.5,0 362.5,0 548.5,0 548.5,0 554.5,0 560.5,-6 560.5,-12 560.5,-12 560.5,-25 560.5,-25 560.5,-31 554.5,-37 548.5,-37"/>
<text text-anchor="start" x="369.5" y="-15" font-family="Helvetica,sans-Serif" font-size="15.00">Institutions financières</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M439.68,-108.92C437.62,-96.78 435.96,-80.32 438.5,-66 439.7,-59.25 441.8,-52.19 444.12,-45.68"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="447.09,-46.73 447.37,-37.2 441.21,-44.48 447.09,-46.73"/>
<text text-anchor="start" x="438.5" y="-69.6" font-family="Helvetica,sans-Serif" font-size="13.00">remboursements</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M760.5,-37C760.5,-37 624.5,-37 624.5,-37 618.5,-37 612.5,-31 612.5,-25 612.5,-25 612.5,-12 612.5,-12 612.5,-6 618.5,0 624.5,0 624.5,0 760.5,0 760.5,0 766.5,0 772.5,-6 772.5,-12 772.5,-12 772.5,-25 772.5,-25 772.5,-31 766.5,-37 760.5,-37"/>
<text text-anchor="start" x="631.5" y="-15" font-family="Helvetica,sans-Serif" font-size="15.00">Reste du monde</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M505.36,-116.74C539.95,-109.67 583.09,-98.1 618.5,-80 637,-70.55 655.1,-55.87 668.77,-43.34"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="671.09,-45.48 675.49,-37.03 666.77,-40.89 671.09,-45.48"/>
<text text-anchor="start" x="641.5" y="-69.6" font-family="Helvetica,sans-Serif" font-size="13.00">exportations, importations</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M145.55,-37.17C168.03,-50.63 200.79,-68.72 231.5,-80 277.31,-96.82 331.02,-108.52 372.92,-115.98"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="372.53,-119.11 381.94,-117.55 373.61,-112.9 372.53,-119.11"/>
<text text-anchor="start" x="231.5" y="-69.6" font-family="Helvetica,sans-Serif" font-size="13.00">services publics, commandes</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M527.9,-37.1C552.29,-46.76 570.42,-60.78 557.5,-80 547.15,-95.4 530.71,-105.7 513.51,-112.59"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="512.39,-109.65 505.02,-115.71 514.56,-115.56 512.39,-109.65"/>
<text text-anchor="start" x="562.5" y="-69.6" font-family="Helvetica,sans-Serif" font-size="13.00">crédits</text>
</g>
</g>
</svg>
</figure>

> [!NOTE]
> L'entreprise **cliente** peut être elle-même un ménage (on parle de **B to C**), une autre entreprise (**B to B**), une administration (**B to G**). Entre particuliers, c'est du **C to C**.

## II. L'écosystème des services numériques

Dans le monde de l'informatique, les entreprises se répartissent des **rôles** complémentaires.

| Acteur | Ce qu'il fait | D'où vient son revenu | Exemple de poste |
|---|---|---|---|
| **DSI** (direction des systèmes d'information) | Gère le système d'information **de sa propre organisation** | Budget interne de l'organisation | Technicien support, administrateur |
| **Éditeur de logiciels** | Conçoit et commercialise des logiciels | Licences, abonnements, maintenance | Développeur, support éditeur |
| **ESN** (entreprise de services du numérique) | Vend des **prestations** à d'autres organisations : conseil, intégration, infogérance, maintenance | Prestations facturées à ses clients | Consultant, technicien, chef de projet |
| **Constructeur et distributeur** | Fabriquent ou revendent du matériel | Ventes de matériel, services associés | Technicien avant-vente |
| **Hébergeur et fournisseur de cloud** | Louent de la capacité de calcul, de stockage, de réseau | Abonnements, facturation à l'usage | Exploitant de datacenter |
| **Opérateur et fournisseur d'accès** | Fournissent la connectivité | Abonnements | Technicien réseau |

Le sigle **ESN** remplace l'ancien sigle SSII (société de services en ingénierie informatique). On la qualifie aussi d'entreprise **prestataire** : elle intervient pour le compte d'un **client**.

<figure class="graphe diagramme">
<svg viewBox="0.00 0.00 470.60 327.60" style="max-width:628px" role="img" aria-label="Schéma" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<g class="graph" transform="scale(1 1) rotate(0) translate(10.8 316.8)">
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M88,-306C88,-306 12,-306 12,-306 6,-306 0,-300 0,-294 0,-294 0,-264 0,-264 0,-258 6,-252 12,-252 12,-252 88,-252 88,-252 94,-252 100,-258 100,-264 100,-264 100,-294 100,-294 100,-300 94,-306 88,-306"/>
<text text-anchor="start" x="22.5" y="-284" font-family="Helvetica,sans-Serif" font-size="15.00">Éditeur</text>
<text text-anchor="start" x="19" y="-267" font-family="Helvetica,sans-Serif" font-size="15.00">logiciels</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M306.5,-180C306.5,-180 207.5,-180 207.5,-180 201.5,-180 195.5,-174 195.5,-168 195.5,-168 195.5,-138 195.5,-138 195.5,-132 201.5,-126 207.5,-126 207.5,-126 306.5,-126 306.5,-126 312.5,-126 318.5,-132 318.5,-138 318.5,-138 318.5,-168 318.5,-168 318.5,-174 312.5,-180 306.5,-180"/>
<text text-anchor="start" x="241.5" y="-158" font-family="Helvetica,sans-Serif" font-size="15.00">ESN</text>
<text text-anchor="start" x="214.5" y="-141" font-family="Helvetica,sans-Serif" font-size="15.00">intégrateur</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M81.29,-251.73C98.33,-238.08 120.16,-221.66 141,-209 155.68,-200.08 172.04,-191.55 187.73,-183.98"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="189.08,-186.82 195.86,-180.11 186.38,-181.13 189.08,-186.82"/>
<text text-anchor="start" x="141" y="-212.6" font-family="Helvetica,sans-Serif" font-size="13.00">licences</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M340.5,-54C340.5,-54 173.5,-54 173.5,-54 167.5,-54 161.5,-48 161.5,-42 161.5,-42 161.5,-12 161.5,-12 161.5,-6 167.5,0 173.5,0 173.5,0 340.5,0 340.5,0 346.5,0 352.5,-6 352.5,-12 352.5,-12 352.5,-42 352.5,-42 352.5,-48 346.5,-54 340.5,-54"/>
<text text-anchor="start" x="180.5" y="-32" font-family="Helvetica,sans-Serif" font-size="15.00">Organisation cliente</text>
<text text-anchor="start" x="185" y="-15" font-family="Helvetica,sans-Serif" font-size="15.00">(DSI + utilisateurs)</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M45.04,-251.84C40.4,-219.39 37.5,-163.75 63,-126 84.28,-94.51 118.84,-72.63 152.94,-57.67"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="154.53,-60.42 161.59,-54.02 152.07,-54.62 154.53,-60.42"/>
<text text-anchor="start" x="63" y="-149.6" font-family="Helvetica,sans-Serif" font-size="13.00">licences directes</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M257,-125.7C257,-107.54 257,-83.17 257,-63.31"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="260.15,-63.26 257,-54.26 253.85,-63.26 260.15,-63.26"/>
<text text-anchor="start" x="257" y="-86.6" font-family="Helvetica,sans-Serif" font-size="13.00">prestations</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M270,-306C270,-306 158,-306 158,-306 152,-306 146,-300 146,-294 146,-294 146,-264 146,-264 146,-258 152,-252 158,-252 158,-252 270,-252 270,-252 276,-252 282,-258 282,-264 282,-264 282,-294 282,-294 282,-300 276,-306 270,-306"/>
<text text-anchor="start" x="165" y="-284" font-family="Helvetica,sans-Serif" font-size="15.00">Constructeur</text>
<text text-anchor="start" x="169.5" y="-267" font-family="Helvetica,sans-Serif" font-size="15.00">distributeur</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M206.98,-251.7C204.72,-238.5 203.94,-222.5 209,-209 211.91,-201.24 216.46,-193.86 221.63,-187.17"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="224.1,-189.13 227.43,-180.2 219.25,-185.1 224.1,-189.13"/>
<text text-anchor="start" x="209" y="-212.6" font-family="Helvetica,sans-Serif" font-size="13.00">matériel</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M437,-306C437,-306 343,-306 343,-306 337,-306 331,-300 331,-294 331,-294 331,-264 331,-264 331,-258 337,-252 343,-252 343,-252 437,-252 437,-252 443,-252 449,-258 449,-264 449,-264 449,-294 449,-294 449,-300 443,-306 437,-306"/>
<text text-anchor="start" x="350" y="-284" font-family="Helvetica,sans-Serif" font-size="15.00">Hébergeur</text>
<text text-anchor="start" x="369" y="-267" font-family="Helvetica,sans-Serif" font-size="15.00">cloud</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M346.59,-251.78C334.16,-243.34 321.01,-233.44 310,-223 298.94,-212.51 288.37,-199.57 279.61,-187.74"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="281.96,-185.61 274.14,-180.17 276.86,-189.31 281.96,-185.61"/>
<text text-anchor="start" x="310" y="-212.6" font-family="Helvetica,sans-Serif" font-size="13.00">capacité</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M389.58,-251.79C387.7,-211.78 379.1,-134.69 342,-83 335.53,-73.99 327.08,-66.07 318.03,-59.27"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="319.82,-56.68 310.66,-54.05 316.18,-61.82 319.82,-56.68"/>
<text text-anchor="start" x="380" y="-149.6" font-family="Helvetica,sans-Serif" font-size="13.00">services</text>
</g>
</g>
</svg>
</figure>

### Où se situe ton entreprise d'alternance ?

Elle est l'un de ces acteurs. Pour la situer, pose trois questions :

1. **Vend-elle** des prestations informatiques à d'autres (ESN) ou **utilise-t-elle** l'informatique pour son propre métier (DSI d'une organisation) ?
2. **Qui est son client**, et qui sont ses **fournisseurs** (éditeurs, hébergeurs, distributeurs) ?
3. **Comment est-elle payée** ou comment finance-t-elle son service informatique ?

## III. La relation client – prestataire

Quand une ESN intervient chez un client, trois formes de prestations sont fréquentes.

| Forme | Principe | Qui dirige le travail ? | Qui porte le risque de dérive ? | Obligation du prestataire |
|---|---|---|---|---|
| **Régie** (assistance technique) | Le prestataire met des **personnes à disposition** pour un temps donné ; facturation au **temps passé** (jours) | Le **client** | Le **client** (il paie le temps passé) | De **moyens** |
| **Forfait** | Un **résultat** est promis pour un **prix fixe** | Le **prestataire** | Le **prestataire** (le prix est fixe) | De **résultat** |
| **Infogérance** (tierce maintenance) | Le prestataire prend en charge l'exploitation d'un ensemble de services selon un **niveau de service** contractuel | Le **prestataire** | Partagé, selon le contrat | De **résultat**, selon les engagements |

> [!NOTE]
> **Obligation de moyens** : le prestataire s'engage à faire de son mieux, sans garantir le résultat. **Obligation de résultat** : il s'engage à atteindre un résultat précis ; s'il n'est pas atteint, sa responsabilité est engagée sans qu'on lui reproche une faute. Cette distinction revient en séance 4 (contrats) et en séance 7 (responsabilités).

**Le prix d'une journée en régie** s'appelle le **TJM** (taux journalier moyen). Il couvre le coût du salarié (salaire, charges, frais) **et** les coûts de structure de l'ESN (commerciaux, locaux, gestion), plus sa **marge**.

> [!WARNING]
> En régie, le client ne peut pas donner d'ordres au salarié de l'ESN **comme s'il était son propre employé** : le salarié reste sous l'**autorité de son employeur**. Le Code du travail interdit le **prêt de main-d'œuvre à but lucratif** hors cadres autorisés (article L8241-1) et le **marchandage** (article L8231-1). Une régie conforme est une prestation de service réelle, qui apporte une **compétence**, avec un contrat précisant la mission.

## IV. Les modèles économiques du numérique

| Modèle | Principe | Exemple d'usage |
|---|---|---|
| **Licence** | Le client paie pour obtenir le **droit d'utiliser** un logiciel (souvent avec maintenance annuelle) | Poste de travail sous licence propriétaire |
| **Abonnement (SaaS)** | Le client **loue** un service accessible par Internet, facturé par mois ou par utilisateur | Messagerie, suite bureautique en ligne |
| **Open source et services** | Le logiciel est libre ; l'éditeur ou l'ESN vend le **support**, l'intégration, la formation | Système d'exploitation libre accompagné d'un contrat de support |
| **Freemium** | Une version gratuite attire, une version payante apporte plus de fonctions | Outil de supervision avec une version limitée |
| **Plateforme** | Une place de marché met en relation offreurs et demandeurs et prend une **commission** | Boutique d'applications |
| **Prestation** | Le client paie un **service** : temps, projet, niveau de service | Régie, forfait, infogérance |

### Ce qui change avec le numérique

- **Du capital vers l'usage** : on **loue** plutôt qu'on **achète** (cloud, abonnements). Les dépenses d'investissement deviennent des dépenses de fonctionnement.
- **Des effets de réseau** : plus un service a d'utilisateurs, plus il a de valeur pour chacun. Cela favorise des acteurs très grands (voir séance 2).
- **Une dépendance** : changer de fournisseur peut être coûteux (formats propriétaires, migration). C'est le **verrouillage** (*lock-in*).

## V. Un exemple chiffré : régie ou forfait ?

Une ESN fictive facture un client pour migrer des postes. Données :

- coût complet d'un consultant pour l'ESN : **390 €** par jour travaillé (salaire, charges, frais de structure) ;
- mission prévue : **2 consultants × 20 jours = 40 jours** ;
- en **régie** : TJM de **480 €** ; en **forfait** : prix fixe de **21 500 €**.

| | Régie | Forfait |
|---|---|---|
| Prix payé par le client (charge prévue) | 40 × 480 = **19 200 €** | **21 500 €** |
| Coût pour l'ESN (charge prévue) | 40 × 390 = **15 600 €** | **15 600 €** |
| Marge de l'ESN | **3 600 €** (18,75 % du prix) | **5 900 €** (27,4 % du prix) |
| Si la charge dépasse de **30 %** : prix payé par le client | 19 200 × 1,3 = **24 960 €** | **21 500 €** (inchangé) |
| Si la charge dépasse de **30 %** : coût pour l'ESN | 15 600 × 1,3 = **20 280 €** | **20 280 €** |
| Si la charge dépasse de **30 %** : marge de l'ESN | **4 680 €** (18,75 %) | **1 220 €** (5,7 %) |

**Lecture.** En régie, la dérive est payée par le **client** et l'ESN garde sa marge. En forfait, la dérive est supportée par l'**ESN**, dont la marge s'effondre. Le forfait est plus cher au départ (21 500 € contre 19 200 €) mais protège le client **si le projet dérape** ; la régie est moins chère si tout va bien.

## Comprendre pas à pas

### Reconnaître un modèle économique : une grille

| Modèle | Qui paie ? | Pour quoi ? | Exemple |
|---|---|---|---|
| **Vente de produit** | Le client | Un matériel ou un logiciel, une fois | Achat d'un poste |
| **Abonnement** | Le client | L'accès et le service dans la durée | Messagerie, antivirus |
| **Freemium** | Une minorité de clients | Des fonctions avancées | Stockage gratuit limité, version payante |
| **Publicité** | Les annonceurs | L'attention des utilisateurs | Moteur de recherche |
| **Plateforme / commission** | Une des faces du marché | La mise en relation | Place de marché |
| **Services autour du libre** | Le client | Support, installation, formation | Red Hat |

> [!TIP]
> Pour un modèle donné, pose toujours **deux questions** : **qui paie ?** et **pour quoi ?** Le service peut être gratuit pour l'utilisateur **parce qu'un tiers paie** (publicité).

### Régie ou forfait : un calcul

Un projet est estimé à **18 jours** de travail. Le prestataire facture **600 € par jour** en régie, ou **11 000 €** au forfait.

| Scénario | Régie | Forfait |
|---|---:|---:|
| Le projet dure **18 jours** | \(18 \times 600 = 10\,800\) € | 11 000 € |
| Le projet dure **24 jours** (dérive) | \(24 \times 600 = 14\,400\) € | 11 000 € |

**Lecture :** en **régie**, le **client** porte le risque de dérive (il paie les jours réels) ; au **forfait**, c'est le **prestataire** (il perd la différence). Le forfait exige un **besoin précisément défini** : voir le cas du projet de Lidl en séance 4.

Un cas réel sur un modèle de services est détaillé dans [IBM et Red Hat](04-cas-reels.md).

## À retenir

- Cinq agents économiques : **ménages, entreprises, administrations, institutions financières, reste du monde** ; ils échangent des flux réels et financiers.
- Un **écosystème** : DSI, éditeurs, ESN, constructeurs et distributeurs, hébergeurs, opérateurs.
- **Régie** (temps passé, obligation de moyens, risque pour le client), **forfait** (résultat, prix fixe, risque pour le prestataire), **infogérance** (niveau de service).
- Modèles économiques : **licence**, **abonnement (SaaS)**, **open source et services**, **freemium**, **plateforme**, **prestation**.
- Le numérique pousse à **louer plutôt qu'acheter** et crée des **dépendances** (verrouillage).
