# Cours – Preuve électronique, signature et identité numérique

*BTS SIO SISR 1re année – CEJM et CEJMA – S18 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S11, S15

## À la fin de ce cours tu sauras

- [ ] Citer les conditions de l'**écrit électronique**
- [ ] Distinguer les niveaux de **signature**
- [ ] Appliquer la **chaîne de conservation**
- [ ] Distinguer **identifier** et **authentifier**
- [ ] Respecter la **loyauté** de la preuve

## I. La preuve en droit

Quand un litige naît (contrat contesté, faute reprochée, intrusion), il faut **prouver**. Le régime de la preuve dépend du domaine.

| Domaine | Principe |
|---|---|
| **Civil** (contrats, consommation) | Preuve **écrite** pour les actes d'un certain montant, sinon liberté de preuve ; règles du Code civil |
| **Commercial** (entre commerçants) | **Liberté de la preuve** |
| **Pénal** | **Liberté de la preuve**, mais la preuve doit être **obtenue loyalement** |
| **Travail** | Liberté de la preuve, avec le respect de la **vie privée** et de la **loyauté** (séance 11) |

## II. L'écrit et la signature électroniques

| Notion | Règle |
|---|---|
| **Écrit électronique** | Admis comme preuve **s'il permet d'identifier son auteur** et s'il est établi et conservé dans des conditions qui en **garantissent l'intégrité** (Code civil, article 1366) |
| **Signature électronique** | Manifeste le **consentement** ; fiabilité présumée si procédé conforme (Code civil, article 1367) |
| **Règlement eIDAS** (UE 910/2014) | Trois niveaux : **simple**, **avancée**, **qualifiée** ; la signature qualifiée a la **même valeur** qu'une signature manuscrite |
| **Horodatage** | Prouve qu'un document existait à une date donnée |
| **Cachet électronique** | Équivalent pour les personnes morales |

> [!NOTE]
> Un simple courriel peut servir de preuve, mais sa **force** dépend de la possibilité d'**identifier l'auteur** et de prouver que le contenu n'a pas été **modifié**.

## III. Les preuves numériques en pratique

| Preuve | Qualité nécessaire | Bonnes pratiques |
|---|---|---|
| **Journaux** (logs) | Horodatés, **intègres**, **complets** | Horloge synchronisée (NTP), centralisation, droits en écriture limités |
| **Courriels** | En-têtes complets, intégrité | Conserver l'**original** (format source) |
| **Captures d'écran** | Limitée seule | Compléter par un **constat** |
| **Disques et fichiers** | Intégrité démontrable | Copie **bit à bit**, **empreinte** (hash) avant et après |
| **Pages web** | Contenu évolutif | **Constat de commissaire de justice**, outils d'archivage horodaté |

### La chaîne de conservation

Pour qu'une preuve soit **recevable et crédible** :

1. **Identifier** ce qu'on conserve et où ;
2. **Préserver** sans altérer : copie de travail, original intact, **empreinte** (SHA-256) ;
3. **Documenter** qui a accédé, quand, pourquoi (**chaîne de conservation**) ;
4. **Conserver** dans un lieu sûr, accès limité ;
5. **Présenter** avec les explications nécessaires.

<figure class="graphe diagramme">
<svg viewBox="0.00 0.00 418.10 411.60" style="max-width:557px" role="img" aria-label="Schéma" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<g class="graph" transform="scale(1 1) rotate(0) translate(10.8 400.8)">
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M231,-390C231,-390 123,-390 123,-390 117,-390 111,-384 111,-378 111,-378 111,-348 111,-348 111,-342 117,-336 123,-336 123,-336 231,-336 231,-336 237,-336 243,-342 243,-348 243,-348 243,-378 243,-378 243,-384 237,-390 231,-390"/>
<text text-anchor="start" x="148" y="-368" font-family="Helvetica,sans-Serif" font-size="15.00">Constat</text>
<text text-anchor="start" x="130" y="-351" font-family="Helvetica,sans-Serif" font-size="15.00">de l&#39;incident</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M231.5,-278C231.5,-278 122.5,-278 122.5,-278 116.5,-278 110.5,-272 110.5,-266 110.5,-266 110.5,-236 110.5,-236 110.5,-230 116.5,-224 122.5,-224 122.5,-224 231.5,-224 231.5,-224 237.5,-224 243.5,-230 243.5,-236 243.5,-236 243.5,-266 243.5,-266 243.5,-272 237.5,-278 231.5,-278"/>
<text text-anchor="start" x="155.5" y="-256" font-family="Helvetica,sans-Serif" font-size="15.00">Copie</text>
<text text-anchor="start" x="129.5" y="-239" font-family="Helvetica,sans-Serif" font-size="15.00">+ empreinte</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M177,-335.93C177,-321.52 177,-303.39 177,-287.68"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="180.15,-287.26 177,-278.26 173.85,-287.26 180.15,-287.26"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M134,-166C134,-166 12,-166 12,-166 6,-166 0,-160 0,-154 0,-154 0,-124 0,-124 0,-118 6,-112 12,-112 12,-112 134,-112 134,-112 140,-112 146,-118 146,-124 146,-124 146,-154 146,-154 146,-160 140,-166 134,-166"/>
<text text-anchor="start" x="19" y="-144" font-family="Helvetica,sans-Serif" font-size="15.00">Original scellé</text>
<text text-anchor="start" x="29" y="-127" font-family="Helvetica,sans-Serif" font-size="15.00">et conservé</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M152.35,-223.93C137.95,-208.7 119.64,-189.33 104.23,-173.04"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="106.3,-170.64 97.83,-166.26 101.72,-174.97 106.3,-170.64"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M363.5,-157.5C363.5,-157.5 198.5,-157.5 198.5,-157.5 192.5,-157.5 186.5,-151.5 186.5,-145.5 186.5,-145.5 186.5,-132.5 186.5,-132.5 186.5,-126.5 192.5,-120.5 198.5,-120.5 198.5,-120.5 363.5,-120.5 363.5,-120.5 369.5,-120.5 375.5,-126.5 375.5,-132.5 375.5,-132.5 375.5,-145.5 375.5,-145.5 375.5,-151.5 369.5,-157.5 363.5,-157.5"/>
<text text-anchor="start" x="205.5" y="-135.5" font-family="Helvetica,sans-Serif" font-size="15.00">Analyse sur la copie</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M201.65,-223.93C218.72,-205.87 241.3,-181.99 258,-164.32"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="260.42,-166.35 264.32,-157.64 255.85,-162.02 260.42,-166.35"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M384.5,-54C384.5,-54 177.5,-54 177.5,-54 171.5,-54 165.5,-48 165.5,-42 165.5,-42 165.5,-12 165.5,-12 165.5,-6 171.5,0 177.5,0 177.5,0 384.5,0 384.5,0 390.5,0 396.5,-6 396.5,-12 396.5,-12 396.5,-42 396.5,-42 396.5,-48 390.5,-54 384.5,-54"/>
<text text-anchor="start" x="251" y="-32" font-family="Helvetica,sans-Serif" font-size="15.00">Rapport</text>
<text text-anchor="start" x="184.5" y="-15" font-family="Helvetica,sans-Serif" font-size="15.00">+ chaîne de conservation</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M281,-120.33C281,-104.98 281,-82.3 281,-63.26"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="284.15,-63.25 281,-54.25 277.85,-63.25 284.15,-63.25"/>
</g>
</g>
</svg>
</figure>

> [!WARNING]
> **Ne jamais travailler sur l'original.** Une preuve modifiée, sans traçabilité, peut être écartée, et le technicien est accusé d'avoir altéré des éléments.

## IV. L'identité numérique

L'**identité numérique** est l'ensemble des **traces** et des **données** associées à une personne en ligne : comptes, publications, profils, historique, avis.

### Identifier et authentifier

| Notion | Sens |
|---|---|
| **Identification** | Dire qui l'on est |
| **Authentification** | **Prouver** que l'on est bien cette personne (mot de passe, second facteur, certificat) |
| **Fédération d'identité** | Utiliser une identité existante pour se connecter ailleurs (ex. : FranceConnect) |

### E-réputation et droits

- **E-réputation** : image d'une personne ou d'une entreprise sur Internet. Les avis et publications comptent.
- **Droit à l'effacement** et **déréférencement** : demander la suppression de données ou le retrait d'un résultat de recherche (RGPD, séance 14).
- **Usurpation d'identité** : utiliser l'identité d'autrui pour nuire ou obtenir un avantage est une **infraction** (Code pénal, article 226-4-1, à vérifier).

### Pour l'entreprise

Politique d'**identités et d'accès** (un compte par personne, gestion des départs), **communication** maîtrisée, **veille** sur sa réputation, **réponse** aux avis.

## Comprendre pas à pas

### Identifier ou authentifier : un exemple du quotidien

| Situation | Identifier | Authentifier |
|---|---|---|
| Tu te connectes à l'ENT | Tu tapes ton **identifiant** : tu dis **qui tu prétends être** | Tu tapes ton **mot de passe** (ou un code reçu) : tu **prouves** que c'est toi |
| Tu entres dans les locaux | Tu présentes ton **badge** | Le **code** ou l'empreinte confirme que le badge est bien le tien |

Un identifiant seul ne prouve rien : n'importe qui peut le connaître. D'où l'authentification **forte** (deux éléments de natures différentes : ce que je **sais**, ce que je **possède**, ce que je **suis**).

### De quoi est faite l'e-réputation d'une entreprise ?

| Source | Exemples | Qui la contrôle ? |
|---|---|---|
| **Ce que l'entreprise publie** | Site, réseaux sociaux, communiqués | L'entreprise |
| **Ce que les autres disent** | Avis clients, commentaires, articles | Les tiers |
| **Ce que les moteurs montrent** | Résultats pour le nom de l'entreprise ou d'une personne | Les moteurs de recherche |

L'entreprise ne contrôle **qu'une partie** de son e-réputation : le reste se **surveille** et se **traite**.

### Exemple guidé : répondre à un avis négatif

Un client écrit : « Panne de trois jours, personne ne répond. » Quatre étapes :

1. **Vérifier** : le client existe-t-il ? la panne a-t-elle eu lieu ? (consulter le journal d'incidents)
2. **Répondre en public**, brièvement et poliment, en reconnaissant le problème et en proposant un contact : *« Nous sommes désolés de cette gêne. Le service a été rétabli le […]. Nous vous contactons directement. »*
3. **Traiter en privé** : contacter le client, corriger la cause.
4. **Capitaliser** : noter l'incident et ajouter une action au plan de prévention.

> [!WARNING]
> Un avis négatif **n'est pas illégal** par lui-même : la liberté d'expression le permet. Il devient problématique s'il est **faux**, **injurieux** ou **diffamatoire**. On ne supprime pas un avis parce qu'il déplaît.

Deux cas réels documentés sont à lire dans [Cas réels](04-cas-reels.md) : un faux restaurant classé numéro 1 sur TripAdvisor, et le droit au déréférencement (Google Spain).

## À retenir

- **Liberté de la preuve** en matière commerciale et pénale, mais **loyauté** exigée.
- **Écrit électronique** : **auteur identifié** et **intégrité** garantie (art. 1366) ; signature **qualifiée** = valeur de la signature manuscrite (eIDAS).
- Preuve numérique : **copie + empreinte**, **chaîne de conservation**, **jamais sur l'original**.
- **Identité numérique** : identifier ≠ authentifier ; e-réputation ; effacement ; usurpation punissable.
