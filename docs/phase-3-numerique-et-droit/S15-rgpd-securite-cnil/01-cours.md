# Cours – RGPD : sécurité, violations de données, AIPD et sanctions

*BTS SIO SISR 1re année – CEJMA – S15 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S13, S14, S07

## À la fin de ce cours tu sauras

- [ ] Citer des mesures de **sécurité** adaptées
- [ ] Appliquer la règle des **72 heures**
- [ ] Décider d'**informer** les personnes
- [ ] Citer les **pouvoirs** et **sanctions** de la CNIL
- [ ] Proposer des **mesures correctives**

## I. Sécuriser les données (article 32)

Le responsable de traitement et le sous-traitant doivent mettre en œuvre des mesures **techniques et organisationnelles appropriées** au **risque**, en tenant compte de l'état de l'art, des coûts, de la nature des données et de la gravité des risques pour les personnes.

| Famille | Exemples |
|---|---|
| **Pseudonymisation et chiffrement** | Disques chiffrés, communications chiffrées |
| **Confidentialité** | Gestion des droits, authentification forte, cloisonnement |
| **Intégrité et disponibilité** | Sauvegardes testées, plan de reprise |
| **Résilience** | Mises à jour, supervision, tests réguliers |
| **Organisation** | Charte, sensibilisation, procédures, habilitations (séance 11) |

> [!NOTE]
> Il n'existe pas de liste fermée de mesures : on **adapte au risque** et on **documente** ses choix (principe de responsabilité).

## II. La violation de données

Une **violation de données personnelles** est une atteinte à la **confidentialité**, à l'**intégrité** ou à la **disponibilité** de données, **accidentelle ou illicite** : vol d'ordinateur, rançongiciel, envoi d'un fichier au mauvais destinataire, perte de clé USB, accès abusif d'un salarié.

### Que faire ?

<figure class="graphe diagramme">
<svg viewBox="0.00 0.00 646.10 836.60" style="max-width:861px" role="img" aria-label="Schéma" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<g class="graph" transform="scale(1 1) rotate(0) translate(10.8 825.8)">
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M263,-815C263,-815 112,-815 112,-815 106,-815 100,-809 100,-803 100,-803 100,-790 100,-790 100,-784 106,-778 112,-778 112,-778 263,-778 263,-778 269,-778 275,-784 275,-790 275,-790 275,-803 275,-803 275,-809 269,-815 263,-815"/>
<text text-anchor="start" x="119" y="-793" font-family="Helvetica,sans-Serif" font-size="15.00">Violation détectée</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M286.5,-719C286.5,-719 88.5,-719 88.5,-719 82.5,-719 76.5,-713 76.5,-707 76.5,-707 76.5,-677 76.5,-677 76.5,-671 82.5,-665 88.5,-665 88.5,-665 286.5,-665 286.5,-665 292.5,-665 298.5,-671 298.5,-677 298.5,-677 298.5,-707 298.5,-707 298.5,-713 292.5,-719 286.5,-719"/>
<text text-anchor="start" x="113.5" y="-697" font-family="Helvetica,sans-Serif" font-size="15.00">Contenir et corriger</text>
<text text-anchor="start" x="95.5" y="-680" font-family="Helvetica,sans-Serif" font-size="15.00">isoler, changer les accès</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M187.5,-777.65C187.5,-764.12 187.5,-745.11 187.5,-728.53"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="190.65,-728.11 187.5,-719.11 184.35,-728.11 190.65,-728.11"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M301.5,-606C301.5,-606 73.5,-606 73.5,-606 67.5,-606 61.5,-600 61.5,-594 61.5,-594 61.5,-564 61.5,-564 61.5,-558 67.5,-552 73.5,-552 73.5,-552 301.5,-552 301.5,-552 307.5,-552 313.5,-558 313.5,-564 313.5,-564 313.5,-594 313.5,-594 313.5,-600 307.5,-606 301.5,-606"/>
<text text-anchor="start" x="80.5" y="-584" font-family="Helvetica,sans-Serif" font-size="15.00">Documenter dans le registre</text>
<text text-anchor="start" x="135.5" y="-567" font-family="Helvetica,sans-Serif" font-size="15.00">des violations</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M187.5,-664.98C187.5,-650.19 187.5,-631.48 187.5,-615.37"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="190.65,-615.25 187.5,-606.25 184.35,-615.25 190.65,-615.25"/>
</g>
<g class="node n&#45;diamond">
<polygon fill="none" stroke="black" stroke-width="1.8" points="187.5,-493 33.5,-439 187.5,-385 341.5,-439 187.5,-493"/>
<text text-anchor="start" x="142" y="-444" font-family="Helvetica,sans-Serif" font-size="15.00">Risque pour</text>
<text text-anchor="start" x="129.5" y="-427" font-family="Helvetica,sans-Serif" font-size="15.00">les personnes ?</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M187.5,-551.72C187.5,-537.6 187.5,-519.55 187.5,-502.09"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="190.65,-502.04 187.5,-493.04 184.35,-502.04 190.65,-502.04"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M231,-313C231,-313 12,-313 12,-313 6,-313 0,-307 0,-301 0,-301 0,-271 0,-271 0,-265 6,-259 12,-259 12,-259 231,-259 231,-259 237,-259 243,-265 243,-271 243,-271 243,-301 243,-301 243,-307 237,-313 231,-313"/>
<text text-anchor="start" x="52" y="-291" font-family="Helvetica,sans-Serif" font-size="15.00">Pas de notification</text>
<text text-anchor="start" x="19" y="-274" font-family="Helvetica,sans-Serif" font-size="15.00">mais inscription au registre</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M167.34,-391.87C157.41,-369.16 145.64,-342.24 136.52,-321.36"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="139.4,-320.09 132.91,-313.1 133.63,-322.61 139.4,-320.09"/>
<text text-anchor="start" x="151.5" y="-345.6" font-family="Helvetica,sans-Serif" font-size="13.00">Aucun risque</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M422,-313C422,-313 295,-313 295,-313 289,-313 283,-307 283,-301 283,-301 283,-271 283,-271 283,-265 289,-259 295,-259 295,-259 422,-259 422,-259 428,-259 434,-265 434,-271 434,-271 434,-301 434,-301 434,-307 428,-313 422,-313"/>
<text text-anchor="start" x="302" y="-291" font-family="Helvetica,sans-Serif" font-size="15.00">Notifier la CNIL</text>
<text text-anchor="start" x="322" y="-274" font-family="Helvetica,sans-Serif" font-size="15.00">sous 72 h</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M230.65,-399.9C258.81,-375.03 295.16,-342.93 321.9,-319.32"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="324.16,-321.52 328.82,-313.21 319.99,-316.8 324.16,-321.52"/>
<text text-anchor="start" x="293.5" y="-345.6" font-family="Helvetica,sans-Serif" font-size="13.00">Risque</text>
</g>
<g class="node n&#45;diamond">
<polygon fill="none" stroke="black" stroke-width="1.8" points="358.5,-200 211.5,-163 358.5,-126 505.5,-163 358.5,-200"/>
<text text-anchor="start" x="304" y="-159.5" font-family="Helvetica,sans-Serif" font-size="15.00">Risque élevé ?</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M358.5,-258.74C358.5,-244.32 358.5,-226.02 358.5,-209.35"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="361.65,-209.3 358.5,-200.3 355.35,-209.3 361.65,-209.3"/>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M322,-54C322,-54 115,-54 115,-54 109,-54 103,-48 103,-42 103,-42 103,-12 103,-12 103,-6 109,0 115,0 115,0 322,0 322,0 328,0 334,-6 334,-12 334,-12 334,-42 334,-42 334,-48 328,-54 322,-54"/>
<text text-anchor="start" x="165" y="-32" font-family="Helvetica,sans-Serif" font-size="15.00">Informer aussi</text>
<text text-anchor="start" x="122" y="-15" font-family="Helvetica,sans-Serif" font-size="15.00">les personnes concernées</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M328.47,-133.25C306.24,-111.98 275.92,-82.96 252.75,-60.78"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="254.79,-58.37 246.11,-54.42 250.43,-62.92 254.79,-58.37"/>
<text text-anchor="start" x="288.5" y="-86.6" font-family="Helvetica,sans-Serif" font-size="13.00">Oui</text>
</g>
<g class="node n&#45;rect">
<path fill="none" stroke="black" stroke-width="1.8" d="M612.5,-45.5C612.5,-45.5 386.5,-45.5 386.5,-45.5 380.5,-45.5 374.5,-39.5 374.5,-33.5 374.5,-33.5 374.5,-20.5 374.5,-20.5 374.5,-14.5 380.5,-8.5 386.5,-8.5 386.5,-8.5 612.5,-8.5 612.5,-8.5 618.5,-8.5 624.5,-14.5 624.5,-20.5 624.5,-20.5 624.5,-33.5 624.5,-33.5 624.5,-39.5 618.5,-45.5 612.5,-45.5"/>
<text text-anchor="start" x="393.5" y="-23.5" font-family="Helvetica,sans-Serif" font-size="15.00">Suivi et mesures correctives</text>
</g>
<g class="edge">
<path fill="none" stroke="black" stroke-width="1.8" d="M388.75,-133.25C414.23,-109.04 450.26,-74.79 474.23,-52.02"/>
<polygon fill="black" stroke="black" stroke-width="1.8" points="476.6,-54.11 480.95,-45.63 472.26,-49.54 476.6,-54.11"/>
<text text-anchor="start" x="436.5" y="-86.6" font-family="Helvetica,sans-Serif" font-size="13.00">Non</text>
</g>
</g>
</svg>
</figure>

| Étape | Règle |
|---|---|
| **Notification à la CNIL** | Dans les **72 heures** après en avoir pris **connaissance**, sauf si la violation n'engendre **aucun risque** pour les personnes (articles 33) |
| **Information des personnes** | **Sans retard injustifié** si le risque est **élevé** (article 34), sauf données rendues inintelligibles (chiffrement) |
| **Sous-traitant** | Doit alerter le responsable **dans les meilleurs délais** |
| **Registre des violations** | **Toutes** les violations sont documentées, même non notifiées |

La notification peut être faite **en plusieurs temps** si toutes les informations ne sont pas encore connues : mieux vaut notifier à temps que parfaitement.

### Évaluer la gravité

On croise : **type de données** (sensibles ?), **nombre** de personnes, **facilité d'identification**, **conséquences** (fraude, atteinte à la réputation, discrimination), **mesures de protection** existantes (chiffrement).

## III. L'analyse d'impact (AIPD)

Une **analyse d'impact** (article 35) est requise lorsque le traitement est **susceptible d'engendrer un risque élevé**. La CNIL publie une **liste** de traitements concernés ; des critères reviennent : données **sensibles**, **grande échelle**, **surveillance systématique**, **personnes vulnérables**, croisement de données, nouvelles technologies. En pratique, **deux critères** réunis suffisent souvent à justifier une AIPD.

## IV. La CNIL et les sanctions

### Les pouvoirs de la CNIL

| Pouvoir | Exemples |
|---|---|
| **Conseiller** | Guides, modèles, réponses aux organisations |
| **Contrôler** | Sur place, sur pièces, en ligne, sur convocation |
| **Mettre en demeure** | Demander une mise en conformité dans un délai |
| **Sanctionner** | Avertissement, rappel à l'ordre, limitation ou interdiction du traitement, **amende**, publication |

### Les amendes administratives

| Niveau | Plafond | Exemples de manquements |
|---|---|---|
| **Niveau 1** | **10 M€ ou 2 %** du chiffre d'affaires mondial (le plus élevé) | Défaut de sécurité, de registre, de contrat de sous-traitance, de notification de violation |
| **Niveau 2** | **20 M€ ou 4 %** du chiffre d'affaires mondial | Violation des principes de base, des droits des personnes, des transferts |

La sanction est **proportionnée** : gravité, durée, nombre de personnes, intentionnalité, coopération, mesures prises.

### Autres responsabilités

- **Civile** : réparation du préjudice des personnes (séance 7).
- **Pénale** : le Code pénal punit certains manquements (collecte déloyale, absence de mesures de sécurité, détournement de finalité, accès frauduleux : articles 226-16 et suivants et 323-1 et suivants, à vérifier).
- **Image** : une violation médiatisée coûte parfois plus cher que l'amende.

## V. Le rôle du technicien

L'administrateur ou le technicien est souvent **le premier à voir** une violation : il doit **savoir qui prévenir** (DPO, RSSI, direction), **préserver les preuves** (séance 18) et **ne rien effacer** qui serve à l'enquête.

## Comprendre pas à pas

### Mesures de sécurité : raisonner par scénario

On ne cherche pas « toutes les mesures », mais celles qui répondent au **risque**.

| Scénario | Risque principal | Mesures proportionnées |
|---|---|---|
| Portable d'un commercial avec la liste clients | **Vol, perte** | Chiffrement du disque, verrouillage, effacement à distance |
| Serveur de fichiers RH | **Accès abusif** | Droits limités, authentification forte, journaux d'accès |
| Ancien serveur « oublié » avec des données | **Compromission** | Inventaire, mises à jour, **suppression** des données inutiles |
| Prestataire de maintenance | **Traitement hors instructions** | **Contrat** (article 28), droits limités, traçabilité |

### Violation de données : décider dans l'ordre

Une violation est constatée un **lundi à 10 h**.

1. **Contenir et préserver** les preuves (immédiat).
2. **Évaluer le risque** pour les personnes : données sensibles ? nombre de personnes ? facilité d'identification ?
3. **Notifier la CNIL** si la violation présente un **risque** : au plus tard **72 heures** après la prise de connaissance, soit ici **jeudi à 10 h** (72 = 3 × 24 h).
4. **Informer les personnes** si le risque est **élevé**.
5. **Documenter** la violation, même si elle n'est pas notifiée.

> [!TIP]
> Les 72 heures comptent **les week-ends et jours fériés**. Une violation découverte le vendredi à 10 h se notifie, en principe, avant le lundi à 10 h.

### Exemple guidé : l'amende est proportionnée

Une amende dépend de la **gravité**, de la **durée**, du **nombre de personnes**, de la **nature des données** (santé = très sensible), de la **coopération** et des **mesures prises**. Un petit cabinet qui perd une clé USB chiffrée n'est pas traité comme un éditeur dont une fuite expose des centaines de milliers de dossiers médicaux.

Un cas réel est détaillé dans [Dedalus Biologie](04-cas-reels.md).

## À retenir

- Sécurité **adaptée au risque** (article 32), documentée.
- Violation : **contenir**, **documenter**, **notifier la CNIL sous 72 h** si risque, **informer** les personnes si risque **élevé**.
- Toutes les violations sont inscrites au **registre**.
- **AIPD** pour les traitements à risque élevé.
- Amendes : **10 M€ / 2 %** ou **20 M€ / 4 %**.
