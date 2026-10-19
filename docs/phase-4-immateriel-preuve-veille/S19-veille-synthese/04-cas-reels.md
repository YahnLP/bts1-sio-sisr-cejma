# Cas réel – Log4Shell : une veille qui se joue en heures

*BTS SIO SISR 1re année – CEJMA – S19*

> [!NOTE]
> **Comment travailler.** Lis chaque cas réel et ses sources, réponds par écrit aux questions, puis ouvre « Voir la réponse attendue ». Les faits viennent des sources citées en fin de page ; en cas de doute, **retourne à la source**. Ces cas complètent l'étude de cas fictive de la séance.

## Le dossier

**Les faits.** En décembre 2021, une faille critique est découverte dans **Log4j**, une bibliothèque Java très répandue qui sert à **écrire des journaux**. Elle porte l'identifiant **CVE-2021-44228** et le surnom **Log4Shell**. Un attaquant qui peut influencer un message journalisé peut **faire exécuter du code** à distance sur le serveur.

**Chronologie (voir les sources pour la précision des dates).**

| Date | Événement |
|---|---|
| 9 décembre 2021 | Divulgation publique ; un code d'exploitation circule, des attaques commencent en quelques heures |
| 10 décembre 2021 | Fiche **CVE publiée** dans la base américaine NVD ; la faille est ajoutée au catalogue des vulnérabilités exploitées de la **CISA** ; l'éditeur (fondation Apache) publie la version **2.15.0** |
| Jours suivants | Nouvelles versions correctives (2.16.0, puis 2.17.0 et 2.17.1) |
| 17 décembre 2021 | La CISA impose aux agences fédérales américaines de corriger ou contourner rapidement la faille |
| 24 décembre 2021 | Date limite de correction fixée par la CISA |

**Gravité.** Score **CVSS 10,0 sur 10** : attaque par le **réseau**, **complexité faible**, **aucun privilège**, **aucune interaction** de l'utilisateur, impact **élevé** sur la confidentialité, l'intégrité et la disponibilité.

**Ce qui rend la veille difficile.** Log4j est souvent **embarquée** dans d'autres logiciels : beaucoup d'organisations ne savaient pas **si et où** elles l'utilisaient.

## Pourquoi ce cas est utile

Il montre qu'une veille utile répond à trois questions : **suis-je concerné ?** (inventaire), **à quelle vitesse dois-je agir ?** (gravité, exploitation en cours), **que dois-je faire ?** (correction ou contournement). Sans inventaire, la meilleure veille ne sert à rien.

## Questions

**1.** Pourquoi une organisation qui n'a **pas d'inventaire** de ses logiciels était-elle en difficulté ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Parce qu'elle ne pouvait pas répondre à « **suis-je concerné ?** ». Log4j étant **intégrée dans d'autres logiciels**, il fallait savoir **quels produits** l'embarquaient. L'inventaire (voir S17 et le cours de veille) est le **préalable** de l'action.
</details>

**2.** Rédige la **fiche de veille** de ce cas en quatre lignes : source, information, impact, action.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

**Source** : fiche CVE-2021-44228 (NVD) et alerte de l'éditeur, sources **primaires**. **Information** : faille d'exécution de code à distance dans Log4j2, score 10,0, exploitée. **Impact** : tout service Java qui journalise des données externes avec une version vulnérable est exposé. **Action** : inventorier les produits concernés, passer à une version corrigée, appliquer les contournements indiqués, surveiller les journaux.
</details>

**3.** Classe ces sources de la plus fiable à la moins fiable pour ce cas : (a) la fiche NVD, (b) un message de réseau social annonçant « la faille est partout », (c) un article d'un site spécialisé citant la fiche NVD.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(a) **NVD** (source **primaire**, officielle) > (c) **article spécialisé** (source **secondaire** qui cite la primaire) > (b) **réseau social** (non vérifié, à recouper). Une information importante se **recoupe** avec au moins une autre source indépendante.
</details>

## Sources

- [NVD – CVE-2021-44228](https://nvd.nist.gov/vuln/detail/CVE-2021-44228) : date de publication (10 décembre 2021), score CVSS 3.1 de 10,0, versions affectées, ajout au catalogue CISA le 10 décembre 2021 avec échéance au 24 décembre 2021.
- [Security Scientist – When Was Log4Shell Disclosed](https://answers.securityscientist.net/q/20881/when-was-log4shell-disclosed-and-what-was-the-initial-response) : chronologie de la divulgation, des versions correctives et de la directive de la CISA.

> [!NOTE]
> **À valider :** la date de divulgation du 9 décembre, les dates des versions 2.16.0 à 2.17.1 et la date du 17 décembre viennent d'une source secondaire ; à confirmer sur le site de la fondation Apache et celui de la CISA. L'alerte du CERT-FR n'a pas pu être consultée pour cette page.
