# Cours – Droit des réseaux : hébergeurs, FAI et neutralité du net

*BTS SIO SISR 1re année – CEJMA – S12 – à lire avant l'[étude de cas](02-etude-de-cas.md)*

> [!NOTE] Ce que tu dois savoir déjà
> - **Prérequis :** S07 (responsabilités), S11

## À la fin de ce cours tu sauras

- [ ] Distinguer **éditeur**, **hébergeur**, **FAI**
- [ ] Expliquer le **retrait après notification**
- [ ] Citer la **conservation** des données d'identification
- [ ] Expliquer la **neutralité du net**
- [ ] Rédiger une **procédure de signalement**

## I. Qui est qui sur Internet ?

| Acteur | Rôle | Exemples |
|---|---|---|
| **Fournisseur d'accès à Internet (FAI)** | Donne l'accès au réseau | Opérateurs fixes et mobiles |
| **Hébergeur** | Stocke des contenus ou des services pour des tiers | Hébergement web, cloud, plateformes |
| **Éditeur de contenu** | Choisit et publie les contenus | Site d'entreprise, média, blog |
| **Plateforme en ligne** | Met en relation et diffuse des contenus d'utilisateurs | Réseaux sociaux, places de marché |
| **Utilisateur** | Consomme et publie | Salarié, client |

Le droit applicable dépend du **rôle réellement joué** : un même acteur peut être éditeur pour certains contenus et hébergeur pour d'autres.

## II. Le régime de responsabilité

Le cadre français est la **loi pour la confiance dans l'économie numérique (LCEN) du 21 juin 2004**, complétée par le **règlement européen sur les services numériques (DSA, règlement (UE) 2022/2065)**, applicable à toutes les plateformes depuis le **17 février 2024**.

| Acteur | Principe | Exception |
|---|---|---|
| **Éditeur** | **Responsable** des contenus qu'il publie | — |
| **Hébergeur** | **Non responsable a priori** des contenus stockés | Responsable s'il a **connaissance** d'un contenu **manifestement illicite** et ne le retire pas **promptement** |
| **FAI** | **Pas d'obligation générale de surveillance** | Peut devoir **bloquer** un accès sur **décision d'un juge** ou d'une autorité |

Le principe est celui du **retrait après notification** : toute personne peut signaler un contenu illicite à l'hébergeur par une notification motivée (identité, contenu, motifs, base légale).

> [!WARNING]
> Un hébergeur n'a **pas** à surveiller tout ce que stockent ses clients, mais il doit **agir** quand on lui signale un contenu manifestement illicite. Ne pas réagir engage sa responsabilité.

## III. Conservation des données d'identification

Les hébergeurs et les FAI doivent **conserver** certaines données permettant d'identifier l'auteur d'un contenu (identifiant de connexion, adresse IP, horodatage…) pour répondre à une **demande de l'autorité judiciaire**. La durée est d'**un an** (décret du 25 février 2011, à vérifier). Ces données sont des **données personnelles** : leur accès est strictement encadré (séance 13).

Les **journaux** d'une entreprise qui fournit un accès Wi-Fi ou une messagerie sont soumis à des obligations proches : savoir **qui a fait quoi** en cas de plainte.

## IV. Neutralité du net

La **neutralité du net** impose aux FAI de traiter le trafic de manière **égale**, sans **discrimination** selon l'émetteur, le destinataire, le contenu ou l'application. Elle est posée par le **règlement (UE) 2015/2120**, et son respect est contrôlé en France par l'**ARCEP**.

| Autorisé | Interdit en principe |
|---|---|
| Gestion de trafic **raisonnable, transparente et non discriminatoire** | Bloquer ou ralentir un service concurrent |
| Mesures contre la **cybersécurité** (attaques) | Favoriser un service payant au détriment des autres |
| **Services spécialisés** à qualité garantie (sous conditions) | Faire payer un site pour atteindre les abonnés plus vite |

## V. Contenus illicites et obligations de l'entreprise

Une entreprise qui héberge des contenus de tiers (forum, espace client) doit : prévoir un **dispositif de signalement**, **retirer promptement** les contenus manifestement illicites signalés, **conserver** les données d'identification, désigner un **point de contact**, et **informer** ses utilisateurs par des conditions d'utilisation et des mentions légales.

Les **mentions légales** d'un site (identité de l'éditeur, de l'hébergeur, du directeur de publication) sont **obligatoires**.

## Comprendre pas à pas

### Éditeur, hébergeur, FAI : trois questions pour trancher

| Question | Si la réponse est… | … alors plutôt |
|---|---|---|
| **Qui choisit et met en ligne le contenu ?** | L'entreprise | **Éditeur** (responsable) |
| **Qui se contente de stocker pour un tiers ?** | Le prestataire | **Hébergeur** (responsable après notification) |
| **Qui donne seulement l'accès au réseau ?** | L'opérateur | **FAI** (pas d'obligation générale de surveillance) |

> [!NOTE]
> Un même acteur peut jouer **deux rôles** : par exemple, il édite sa page d'accueil (éditeur) et héberge les commentaires de ses clients (hébergeur).

### Que se passe-t-il quand on signale un contenu ?

1. **Notification** : la personne décrit le contenu, explique pourquoi il est illicite et s'identifie.
2. **Examen** : l'hébergeur vérifie si le contenu est **manifestement illicite**.
3. **Réaction** : s'il l'est, il le **retire promptement** ; sinon, il peut demander l'avis d'un juge.
4. **Traçabilité** : il garde la notification, la décision et les **données d'identification** de l'auteur du contenu (voir partie III).

### Exemple guidé : le commentaire injurieux

Un commentaire visant un salarié est publié sur le forum d'une entreprise. Personne ne le signale pendant trois semaines. L'hébergeur est-il responsable ? **Pas a priori** : il n'a pas à surveiller tout ce qui est publié. Une fois **averti**, en revanche, il doit agir vite. Si le forum est hébergé en interne, l'**entreprise** est elle-même hébergeur : c'est donc **à elle** de réagir, et le technicien doit savoir **qui prévenir**.

Pour une décision de justice qui illustre le critère du « rôle réel », voir [Dailymotion et Tiscali](04-cas-reels.md).

## À retenir

- Éditeur **responsable** ; hébergeur responsable **seulement s'il ne réagit pas** à un contenu manifestement illicite ; FAI sans obligation générale de surveillance.
- Cadre : **LCEN 2004** et **DSA** (applicable depuis le 17 février 2024).
- Conservation des données d'identification : **un an** (à vérifier).
- **Neutralité du net** : égalité de traitement, contrôlée par l'**ARCEP**.
- Les **mentions légales** d'un site sont obligatoires.
