# Cas réels – GitLab (2017) et CrowdStrike (2024) : deux incidents majeurs

*BTS SIO SISR 1re année – CEJMA – S09*

> [!NOTE]
> **Comment travailler.** Lis le cas réel et ses sources, réponds par écrit aux questions, puis ouvre « Voir la réponse attendue ». Les faits viennent des sources citées en fin de page ; en cas de doute, **retourne à la source**. Ce cas complète l'étude de cas fictive de la séance.

## Cas 1 – GitLab : une suppression, cinq sauvegardes défaillantes

**Les faits.** Dans la nuit du **31 janvier au 1er février 2017**, lors d'une opération sur la **base de données** de GitLab.com, un administrateur exécute par erreur une commande de **suppression** sur le **mauvais serveur**. Environ **300 Go** de données de production sont visés ; il interrompt la commande alors qu'il n'en reste que **4,5 Go**.

**Les sauvegardes.** GitLab liste ses défaillances :

| Dispositif | Problème |
|---|---|
| Sauvegardes régulières (toutes les 24 h) | Emplacement non confirmé, fichiers de quelques octets |
| Exports de base (`pg_dump`) | Échec probable **silencieux** (mauvaise version du logiciel) |
| Instantanés de disque | Activés sur un serveur, **pas** sur les bases |
| Stockage S3 | Seau de sauvegarde **vide** |
| Réplication | Procédure **fragile**, mal documentée |

**Le bilan.** La dernière sauvegarde exploitable avait environ **six heures**. GitLab a admis qu'**aucune** de ses cinq techniques de sauvegarde ou de réplication ne fonctionnait de façon fiable. Il a **communiqué publiquement** pendant la reprise (source consultée : article de la presse spécialisée écrit **pendant** la restauration, sans bilan final).

### Questions

**1.** Quelle est la **leçon principale** sur les sauvegardes ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Une sauvegarde qui **n'a jamais été restaurée** n'est pas une garantie : il faut **tester la restauration** et **surveiller** l'exécution des sauvegardes (alerte si le fichier est vide ou trop petit).
</details>

**2.** Cite **deux mesures** qui auraient réduit le risque d'erreur humaine lors de l'opération.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Par exemple : une **procédure écrite** et relue avant l'opération, une **double vérification** du serveur visé (nom affiché dans l'invite), un **compte aux droits limités**, un **environnement de test** pour répéter, un **plan de retour arrière**.
</details>

## Cas 2 – CrowdStrike : 8,5 millions d'ordinateurs en panne

**Les faits.** Le **vendredi 19 juillet 2024**, une **mise à jour défectueuse** du logiciel de sécurité de CrowdStrike plante les ordinateurs **Windows** : écran bleu, puis **boucle de redémarrage**. Microsoft a estimé à **plus de 8,5 millions** le nombre de machines touchées, soit environ **1 %** de son parc mondial. La mise à jour est restée en ligne environ **70 minutes** avant d'être retirée. Ce n'était **pas une cyberattaque**, selon le dirigeant de CrowdStrike.

**Les conséquences.** Environ **4 %** des vols mondiaux annulés d'après la source ; services d'urgence indisponibles dans trois États américains ; hôpitaux perturbés aux Pays-Bas, au Royaume-Uni et en Allemagne ; système d'accréditation des Jeux de Paris 2024 temporairement indisponible. En France, les services, dont les aéroports parisiens, sont revenus à la normale dans l'**après-midi**.

**Le contournement.** Démarrer en **mode sans échec** et supprimer le fichier fautif : **impossible à grande échelle** machine par machine ; une clé USB a ensuite été diffusée. Des **escroqueries** proposant de faux correctifs ont circulé.

### Questions

**3.** Pourquoi le contournement manuel était-il si lent ?

<details markdown="1">
<summary>Voir la réponse attendue</summary>

Parce qu'il fallait **intervenir physiquement ou à distance sur chaque machine**, **en mode sans échec**, alors qu'elles ne démarraient plus normalement. Plus le **parc** est grand, plus la correction **manuelle** est longue : c'est un argument pour les **mises à jour progressives** (déploiement par vagues).
</details>

**4.** Tu es technicien : cite **quatre actions** pendant un **incident majeur** de ce type.

<details markdown="1">
<summary>Voir la réponse attendue</summary>

(1) **Qualifier** l'incident (majeur, périmètre, cause probable) ; (2) **déclencher** la cellule de crise et **informer** utilisateurs et direction à heure fixe ; (3) **appliquer** le contournement validé, en priorisant les **services critiques** ; (4) **se méfier** des faux correctifs et ne suivre que les **sources officielles** ; puis **clôturer** avec un **retour d'expérience**.
</details>

## Sources

- [The Register – GitLab.com data loss](https://www.theregister.com/2017/02/01/gitlab_data_loss/) : faits, 300 Go, 4,5 Go, liste des défaillances, six heures.
- [Blog du Modérateur – Panne mondiale : pourquoi 8,5 millions d'ordinateurs Microsoft ont planté](https://www.blogdumoderateur.com/panne-mondiale-pourquoi-ordinateurs-microsoft-plante/) : CrowdStrike, 19 juillet 2024, 70 minutes, conséquences, contournement.

> [!NOTE]
> **À valider :** le récit GitLab vient d'un article écrit **pendant** l'incident (le bilan final n'y figure pas) ; les chiffres de CrowdStrike (4 % des vols, 1 % du parc) sont ceux de la presse. Les rapports officiels des deux sociétés font foi.
