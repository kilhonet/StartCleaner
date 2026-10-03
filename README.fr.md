# StartCleaner

**Un gestionnaire de démarrage gratuit pour Windows : il affiche sur un seul écran les programmes, tâches planifiées et services lancés au démarrage, et les range en toute sécurité en les désactivant plutôt qu'en les supprimant.**

[English](README.md) · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · [Español](README.es.md) · [Português (Brasil)](README.pt-BR.md) · Français

> Ce document est une traduction. En cas de différence, la [version coréenne](README.ko.md) fait foi.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20(64--bit)-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
![Version](https://img.shields.io/badge/version-2.0.0-blue)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/startcleaner?lang=fr)

![Écran de StartCleaner](images/startcleaner-en.webp)

## Présentation

À chaque démarrage du PC, messageries, assistants de mise à jour et toutes sortes de services se lancent en même temps. Chacun est petit, mais ensemble ils ralentissent le démarrage et occupent de la mémoire.

StartCleaner rassemble tout ce qui se lance automatiquement depuis quatre endroits — dossiers de **Démarrage**, **Registre**, **Tâche**s planifiées et **Service**s — et l'affiche dans une seule liste. Sélectionnez un élément inutile et cliquez sur **Désactiver** : dès le prochain démarrage, il ne se lancera plus. Rien n'est supprimé, seulement éteint, donc un clic sur **Activer** le remet exactement comme avant.

Les éléments de base dont Windows a vraiment besoin sont masqués d'avance dans la liste, si bien qu'il y a peu de risque d'éteindre par erreur quelque chose qu'il ne faut pas toucher.

## Fonctionnalités

- **Une seule liste pour tout** — Voyez au même endroit les éléments de lancement automatique répartis entre dossiers de démarrage, registre, Planificateur de tâches et services.
- **Désactiver plutôt que supprimer** — Éteignez-les avec **Désactiver** et récupérez-les à tout moment avec **Activer**.
- **Éléments de base de Windows masqués** — Les composants de Windows qu'il ne faut pas désactiver n'apparaissent pas dans la liste. Avec une connexion Internet, il récupère la liste la plus récente des éléments à masquer.
- **Des noms faciles à reconnaître** — Affiche le nom du produit et l'icône de chaque programme plutôt que le nom du fichier.
- **Suppression définitive** — Les entrées laissées par des programmes que vous n'utilisez plus peuvent être désactivées puis retirées complètement de la liste.
- **Se renseigner** — Double-cliquez sur un élément inconnu pour le rechercher sur le Web.
- **Enregistrer la liste** — Enregistre tous les éléments de démarrage actuels dans un fichier texte.
- **Mode sombre** — Les couleurs suivent le mode d'application de Windows (clair · sombre).
- **9 langues** — Coréen · anglais · japonais · chinois · russe · italien · français · espagnol · arabe.

## Téléchargement / Installation

| Type | Lien |
|---|---|
| Programme d'installation | [Télécharger](https://down.kilho.net/startcleaner?lang=fr) |
| Portable (ZIP) | [Télécharger](https://down.kilho.net/startcleaner?lang=fr&nosetup) |

Le programme d'installation lance StartCleaner dès la fin de l'installation. Pour la version portable, décompressez le ZIP et lancez `StartCleaner.exe`. Les deux versions ont les mêmes fonctionnalités.

Modifier les éléments de lancement automatique nécessite des droits d'administrateur ; Windows affiche donc une demande d'autorisation d'administrateur au lancement. Cliquez sur **Oui**.

## Utilisation

### Premiers pas

1. Lancez StartCleaner et cliquez sur **Oui** dans la demande d'autorisation d'administrateur.
2. Les éléments lancés au démarrage s'affichent dans la liste avec leur **Programme** et leur **Source**.
3. Cliquez une fois sur l'élément à éteindre, puis sur **Désactiver** en bas.
4. La ligne devient grise et le bouton se change en **Activer**. À partir du prochain démarrage de Windows, cet élément ne sera plus exécuté.
5. Pour le rallumer, cliquez sur la même ligne puis sur **Activer**.

Les éléments désactivés ne disparaissent pas tout de suite de la liste : ils restent à leur place, en gris, pour que vous puissiez annuler aussitôt ce que vous venez de faire.

### Organisation de l'écran

| Élément | Rôle |
|---|---|
| **Accueil** | L'écran avec la liste de lancement automatique |
| Logo KILHO.net | Ouvre la page de présentation de StartCleaner |
| Colonne **Programme** | Icône et nom du programme (le nom du produit, s'il en a un) |
| Colonne **Source** | Où l'élément est enregistré — une icône et un nom |
| Ligne grise | Un élément désactivé |
| **Tous les programmes** | Une fois cochée, affiche tout, y compris les éléments désactivés |
| **Désactiver** / **Activer** | Éteint ou allume l'élément sélectionné. Reste grisé tant qu'aucun élément n'est sélectionné |
| Menu du clic droit | **Supprimer** (éléments désactivés uniquement) · **Liste de sauvegarde** (enregistrer la liste) |

**Source** — d'où chaque élément se lance

| Source | Signification |
|---|---|
| **Démarrage** | Raccourcis et programmes du dossier « Démarrage » du menu Démarrer (tous les utilisateurs · utilisateur actuel) |
| **Registre** | Éléments qu'un programme a enregistrés pour « s'exécuter à l'ouverture de session » lors de son installation |
| **Tâche** | Tâches enregistrées dans le Planificateur de tâches qui s'exécutent à des moments définis (vérification des mises à jour, etc.) |
| **Service** | Services d'arrière-plan qui démarrent automatiquement avec Windows |

### Que faire quand…

**Vous voulez savoir ce qui se lance avec le PC**
Il suffit de lancer StartCleaner. Les éléments de lancement automatique répartis en quatre endroits sont réunis dans une liste, et la colonne **Source** indique où chacun est enregistré. Si vous venez d'installer un programme, appuyez sur **F5** pour recharger la liste.

**Vous ne voulez plus qu'une messagerie ou un assistant de mise à jour s'ouvre à chaque ouverture de session**
Cliquez sur ce programme dans la liste, puis sur **Désactiver**. Le programme n'est pas supprimé et fonctionne comme avant ; il ne se lance simplement plus tout seul au démarrage de Windows. Lancez-le vous-même quand vous en avez besoin. Les éléments **Démarrage** et **Registre** apparaissent aussi comme « Désactivé » dans l'onglet **Applications de démarrage** du Gestionnaire des tâches.

**Vous voulez rallumer un élément désactivé**
Cochez **Tous les programmes** : les éléments désactivés auparavant apparaissent en lignes grises. Cliquez sur la ligne puis sur **Activer**, et il se relancera dès le prochain démarrage.

**Vous voulez éteindre des tâches de mise à jour qui tournent en arrière-plan**
Les lignes dont la **Source** est **Tâche** sont des tâches enregistrées dans le Planificateur de tâches. Beaucoup de vérifications de mises à jour de navigateurs et de programmes se trouvent là. Sélectionnez la tâche à arrêter et cliquez sur **Désactiver** : elle ne s'exécutera plus, même à l'heure prévue.

**Vous voulez qu'un service inutile ne démarre plus avec le PC**
Cliquer sur **Désactiver** sur une ligne **Service** empêche ce service de démarrer avec Windows — et les autres programmes ne peuvent pas non plus le lancer. Cliquer sur **Activer** le fait démarrer automatiquement avec Windows. Mieux vaut vérifier à quel programme appartient un service avant de l'éteindre — renseignez-vous d'abord sur tout service inconnu, comme expliqué ci-dessous.

**Vous ne savez pas ce qu'est un élément**
Double-cliquez sur la ligne : le navigateur s'ouvre avec des informations sur cet élément. Utile pour vérifier ce que fait un programme avant de l'éteindre.

**Il reste des entrées de démarrage d'un programme désinstallé**
Si le programme a disparu mais que son nom est toujours dans la liste, passez d'abord la ligne en **Désactiver**, puis clic droit → **Supprimer**. Cliquez sur **Oui** dans la confirmation, et l'élément est retiré complètement de la liste. Un élément supprimé ne peut pas être restauré ; ne supprimez donc que ce dont vous êtes sûr de ne pas avoir besoin. Le menu **Supprimer** n'apparaît pas pour les éléments encore actifs — le plus sûr est de désactiver d'abord, d'utiliser le PC quelques jours, puis de supprimer.

**Vous voulez supprimer complètement un service**
Seuls les services passés en **Désactiver** peuvent être supprimés avec **Supprimer**. Un service en cours d'exécution est arrêté avant d'être supprimé. Ensuite, un message indique « Un service en cours d'exécution est entièrement supprimé après un redémarrage » : redémarrez le PC une fois et tout est propre.

**Services grisés dans Tous les programmes**
**Tous les programmes** affiche aussi, en lignes grises, les services réglés pour ne démarrer qu'en cas de besoin. Cliquer sur **Activer** sur l'un d'eux le fait démarrer automatiquement à chaque démarrage de Windows ; laissez-les donc tels quels, sauf si c'est vous qui les avez désactivés.

**Vous voulez garder une trace de l'état actuel avant le nettoyage**
Clic droit sur la liste → **Liste de sauvegarde**, puis choisissez l'emplacement. Tous les éléments de lancement automatique — y compris les éléments de base de Windows masqués dans la liste — sont enregistrés dans un fichier texte. Pratique pour comparer l'avant et l'après, ou pour comparer avec un autre PC.

**Pourquoi les éléments de base de Windows ne sont pas dans la liste**
Les services et tâches indispensables au fonctionnement de Windows — audio, réseau, sécurité, etc. — sont masqués dès le départ. Les désactiver pourrait empêcher Windows de fonctionner correctement ; StartCleaner ne vous laisse donc pas y toucher du tout. Ils restent masqués même lorsque **Tous les programmes** est cochée.

**Parcourir la liste au clavier**
Utilisez **↑** · **↓** pour passer d'une ligne à l'autre ; la liste défile pour que la ligne sélectionnée reste toujours visible. **F5** recharge la liste.

**Des noms coupés parce que trop longs**
Faites glisser le bord de la fenêtre pour l'élargir : la colonne **Programme** s'élargit avec elle. Vous pouvez aussi faire glisser la limite entre les en-têtes de colonnes pour régler la largeur vous-même.

**Vous le relancez alors qu'il est déjà ouvert**
Un seul StartCleaner s'exécute à la fois. Le relancer alors que la fenêtre est ouverte n'ouvre pas de nouvelle copie : la fenêtre déjà ouverte passe au premier plan (et se restaure si elle était réduite).

## Configuration

Il n'y a rien à régler. StartCleaner suit de lui-même ce qui suit :

| Élément | Suit |
|---|---|
| Langue | Les paramètres régionaux de Windows (anglais si la langue n'est pas prise en charge) |
| Couleurs | Le mode d'application de Windows (clair · sombre) — les changements s'appliquent aussitôt, même quand StartCleaner est ouvert |

## Configuration requise

- Windows 10 · Windows 11 (64 bits)
- Droits d'administrateur — nécessaires pour modifier les éléments de lancement automatique. Une demande de confirmation s'affiche au lancement.
- Aucun autre composant à installer.
- La connexion Internet ne sert qu'aux annonces de nouvelles versions et à la récupération de la liste des éléments de base de Windows à masquer. Sans connexion, il fonctionne normalement avec sa liste intégrée.

## Mises à jour

StartCleaner ne se met **pas** à jour tout seul. Au lancement, il vérifie s'il existe une nouvelle version et affiche un avis ; cliquer sur **[Oui]** ouvre la page de téléchargement et ferme le programme. Les nouvelles versions sont publiées manuellement après vérification interne et annoncées sur la [page de StartCleaner](https://kilho.net/startcleaner). Consultez l'[avis sur la politique de mise à jour](https://en.kilho.net/archives/notice/2940).

## Licence

StartCleaner est un **freeware**. Utilisez-le gratuitement et sans restriction partout — au bureau, à la maison, dans les administrations ou à l'école — et redistribuez-le librement.

## Liens

- Site web : <https://kilho.net/startcleaner>
- Forum : <https://kilho.top/forum/qna>
- X (Twitter) : <https://www.twitter.com/kilhonet>

© KILHO.NET
