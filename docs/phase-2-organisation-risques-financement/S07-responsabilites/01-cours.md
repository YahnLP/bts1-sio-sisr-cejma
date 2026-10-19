# Cours – Responsabilités civile, pénale et disciplinaire ; cas de l'administrateur

*BTS SIO SISR 1re année – CEJMA – S07 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S01 (obligations de moyens et de résultat), S04 (contrats, clause limitative)

## À la fin de ce cours tu sauras

- [ ] Distinguer **responsabilités civile, pénale et disciplinaire**
- [ ] Vérifier les **trois conditions** de la responsabilité civile
- [ ] Citer les principales **infractions informatiques** et leurs peines
- [ ] Qualifier une **faute disciplinaire**
- [ ] Décrire comment un **administrateur** se protège

## I. Trois responsabilités, trois sanctions

Quand un incident se produit, on se demande **qui en répond** et **de quoi**. Un même fait peut entraîner **plusieurs** responsabilités à la fois.

| Responsabilité | Question | Qui sanctionne ? | Sanction |
|---|---|---|---|
| **Civile** | Qui **répare** le dommage subi par la victime ? | Le juge civil (ou un accord) | **Dommages-intérêts** |
| **Pénale** | Une **infraction** a-t-elle été commise ? | Le juge pénal | **Peine** : amende, emprisonnement, peines complémentaires |
| **Disciplinaire** | Le salarié a-t-il manqué à ses **obligations** envers son employeur ? | L'employeur (sous contrôle du conseil de prud'hommes) | **Sanction** : avertissement, mise à pied, licenciement |

## II. La responsabilité civile

### Les trois conditions

Pour obtenir réparation, la victime doit prouver :

1. une **faute** (ou un fait générateur : action, négligence, imprudence) ;
2. un **dommage** (financier, matériel, moral) ;
3. un **lien de causalité** entre la faute et le dommage.

| Responsabilité | Fondement | Quand ? |
|---|---|---|
| **Contractuelle** | Contrat non respecté (article 1231-1 du Code civil) | Entre les **parties** à un contrat (client et prestataire) |
| **Délictuelle** | Faute causant un dommage à un tiers (articles 1240 et 1241 du Code civil) | Entre personnes **sans contrat** (utilisateur d'un service et tiers) |
| **Du fait d'autrui** | L'employeur répond des fautes de ses **salariés** dans leurs fonctions (article 1242, alinéa 5) | Le salarié a causé le dommage **en travaillant** |

L'**article 1241** vise aussi la **négligence** et l'**imprudence** : pas besoin d'avoir voulu le dommage.

### Le salarié est-il responsable ?

Quand un salarié cause un dommage **dans les limites de sa mission**, c'est l'**employeur** qui en répond vis-à-vis de la victime. Le salarié n'engage pas sa **responsabilité civile personnelle**, sauf s'il a agi **hors de sa mission**, sans autorisation et à des fins étrangères à ses attributions, ou s'il a commis une **infraction intentionnelle**. L'employeur peut sanctionner un salarié fautif (responsabilité disciplinaire), mais ne peut en principe pas lui demander de rembourser un dommage causé par une simple erreur professionnelle.

### Obligation de moyens et obligation de résultat

La **nature de l'obligation** du prestataire (séance 1) décide de **ce que la victime doit prouver**.

| | Obligation de **moyens** | Obligation de **résultat** |
|---|---|---|
| Le prestataire promet | De faire de son mieux | D'atteindre un résultat précis |
| Si le résultat n'est pas atteint | Le client doit prouver une **faute** | La responsabilité est **présumée** ; le prestataire doit prouver une **cause étrangère** (force majeure, faute du client) |

## III. La responsabilité pénale

### Principes

- On ne peut être puni que pour une **infraction prévue par la loi**.
- **Contravention** (peines légères), **délit** (emprisonnement jusqu'à 10 ans, amende), **crime** (réclusion).
- Il faut un **élément matériel** (le fait) et un **élément moral** (l'intention, ou la faute d'imprudence ou de négligence dans certains cas, article 121-3 du Code pénal).
- Les **personnes morales** (entreprises) peuvent être responsables pénalement (article 121-2 du Code pénal), pour des infractions commises pour leur compte par leurs organes ou représentants.
- La **tentative** de délit est punie dans les cas prévus par la loi.

### Les principales infractions en informatique

| Infraction | Texte | Peine |
|---|---|---|
| **Accès ou maintien frauduleux** dans un système de traitement automatisé de données | Article **323-1** | **3 ans** d'emprisonnement et **100 000 €** d'amende ; **5 ans** et **150 000 €** si des données sont supprimées ou modifiées ou si le fonctionnement est altéré |
| **Entrave** au fonctionnement d'un système | Article **323-2** | **5 ans** et **150 000 €** |
| **Atteinte au secret des correspondances** | Article **226-15** | **1 an** et **45 000 €** |
| **Collecte de données personnelles par un moyen frauduleux, déloyal ou illicite** | Article **226-18** | **5 ans** et **300 000 €** |
| **Usurpation d'identité** en ligne | Article **226-4-1** | **1 an** et **15 000 €** |
| **Manquement à la sécurité des données personnelles** | Article **226-17** | **5 ans** et **300 000 €** |

> [!WARNING]
> « J'étais administrateur » ne **protège pas** : avoir un accès **technique** ne donne pas le **droit** de lire ce qui est **privé**. Un administrateur n'a le droit d'accéder aux données que pour **sa mission** (maintenance, sécurité), de façon **proportionnée**.

### Négligence : une infraction est-elle possible ?

Une personne qui, par **imprudence**, **négligence** ou **manquement à une obligation de sécurité**, crée ou ne réduit pas un risque peut être poursuivie dans certains cas ; si le lien avec le dommage est **indirect**, il faut une **faute caractérisée** exposant autrui à un risque d'une particulière gravité qu'elle ne pouvait ignorer (article 121-3). Il y a aussi la **mise en danger délibérée** d'autrui (article 223-1) quand la violation d'une obligation de prudence est **manifestement délibérée**.

## IV. La responsabilité disciplinaire

L'employeur peut sanctionner un salarié qui **manque à ses obligations** (règlement intérieur, charte, contrat).

| Faute | Définition | Conséquence possible |
|---|---|---|
| **Simple** | Manquement ordinaire | Avertissement, mise à pied, licenciement |
| **Grave** | Rend **impossible** le maintien du salarié dans l'entreprise, même pendant le préavis | Licenciement sans préavis ni indemnité de licenciement |
| **Lourde** | Faute grave commise avec **l'intention de nuire** à l'employeur | Licenciement pour faute lourde |

La sanction doit être **proportionnée** et respecter une **procédure** (convocation, entretien).

## V. Le cas particulier de l'administrateur système

| Situation | Risque |
|---|---|
| Un **accès** non nécessaire à des **données privées** | Pénal (226-15), disciplinaire |
| Une **intrusion** que l'administrateur **a facilitée** par négligence répétée malgré des alertes | Disciplinaire ; civil de l'employeur ; pénal dans les cas de faute caractérisée |
| Un **ordre** de l'employeur manifestement **illégal** | L'administrateur doit le **signaler** par écrit et peut **refuser** ; le suivre ne le protège pas |
| Une **alerte** de sécurité ignorée par la hiérarchie | **Garder une trace écrite** de l'alerte et de la réponse |

### Se protéger

1. **Écrire** : alerter la hiérarchie **par écrit** (courriel) et conserver la réponse.
2. Respecter une **procédure** ou la demander : qui peut accéder à quoi, avec quelle justification.
3. Agir **dans la limite de sa mission**.
4. Ne jamais **divulguer** le contenu de données privées rencontrées.
5. Connaître la **charte informatique** de l'entreprise (séance 11).

## À retenir

- **Civile** (réparer), **pénale** (punir une infraction), **disciplinaire** (sanction de l'employeur).
- Civile : **faute, dommage, lien de causalité** ; l'employeur répond de ses salariés dans leurs fonctions.
- **Obligation de résultat** : la responsabilité est présumée ; **de moyens** : la faute doit être prouvée.
- Pénal : **323-1** (accès frauduleux), **323-2** (entrave), **226-15** (secret des correspondances) ; accès technique ≠ droit d'accès.
- Disciplinaire : faute **simple, grave, lourde**.
- L'administrateur se protège par l'**écrit**, la **procédure** et le respect de sa **mission**.
