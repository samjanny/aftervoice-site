---
layout: page
title: Politique de confidentialité d'Aftervoice
---

Dernière mise à jour : 10 septembre 2026.

Aftervoice est un instrument pour des sessions d'écoute. Cette politique dit ce qu'il advient
des données que l'application produit. Ce qu'elle produit reste sur le téléphone, sauf un
signalement que vous choisissez explicitement d'envoyer.

## En bref

Aftervoice n'a pas de comptes, de publicité ni de statistiques d'usage. Les enregistrements,
la piste microphone, le journal, les notes, les repères et les données des capteurs ne sont
jamais envoyés à nos serveurs. Le réseau sert aux banques vocales gérées par Google Play et,
uniquement à votre demande, à un signalement textuel.

## Ce qui reste sur le téléphone

- **Les réglages** : langue de l'interface, langue de la voix, minuteur, recherche automatique,
  filtre de bruit.
- **Le journal des sessions** : date, durée d'écoute, l'accord utilisé, le titre et les notes
  que vous écrivez, et les repères avec le nom que vous leur donnez.
- **Les enregistrements**, quand vous appuyez sur Enregistrer. Écoute de la pièce sauvegarde
  uniquement le microphone, y compris les voix à proximité, sans émission sonore de
  l’application. Réglage sauvegarde le son de l’application et, avec autorisation, le
  microphone. Celui-ci peut aussi capter le haut-parleur : les pistes ne sont pas isolées
  acoustiquement.

Ce sont des fichiers privés de l'application, dans son propre espace. Aucune autre application
du téléphone ne peut les lire. L'application est exclue de la sauvegarde dans le cloud comme du
transfert vers un nouveau téléphone : si vous changez d'appareil, le journal ne vous suit pas.

## Ce qui reste sur le téléphone

Les enregistrements, le microphone, le journal, les réglages, les notes, les repères et les
données des capteurs restent sur le téléphone. Il n'y a ni analyse, ni collecte de plantages,
ni publicité, ni SDK de suivi. L'application contacte Altrove Labs uniquement lorsque vous
appuyez sur **Envoyer le signalement**.

Les rapports de plantage que l'auteur reçoit viennent de Google Play, agrégés et anonymes, et
décrivent le comportement de l'application, jamais le contenu de vos sessions.

## Signalements et assistance

Si vous touchez **Signaler** sur un enregistrement, vous écrivez le motif dans Aftervoice. Ce
n'est qu'en appuyant sur **Envoyer le signalement** que l'application transmet à Altrove Labs,
par HTTPS, ce texte, la version, la langue de l'interface et des identifiants aléatoires de
session et d'enregistrement. Aucun audio, piste microphone, note, repère, identifiant d'appareil
ou adresse électronique n'est envoyé.

Le serveur voit nécessairement l'adresse IP de la connexion. Il l'utilise uniquement en mémoire
pour limiter les abus à cinq signalements par heure, ne la journalise pas et l'oublie sous une
heure ou au redémarrage. Le signalement est transmis par courrier à
`support@altrovelabs.net` et conservé seulement le temps de l'évaluer. L'application affiche une
référence aléatoire permettant d'en demander la suppression. Le prestataire de messagerie ne le
traite que pour le remettre à Altrove Labs. Les données ne sont pas utilisées à d'autres fins.

## La permission microphone

Aftervoice demande une seule permission, **le microphone**, et s'en sert à deux endroits :

- **Pendant un enregistrement**, pour sauvegarder la pièce seule ou à côté de la piste
  synthétique dans Réglage. Le microphone s’ouvre en appuyant sur Enregistrer et se ferme
  à la fin, y compris lorsque l’application passe en arrière-plan.
- **Dans le sonar**, où le son capté est filtré au-dessus de 17 kHz à l'intérieur de
  l'application avant tout traitement, n'est pas enregistré et n'est pas conservé. Le microphone
  ne reste ouvert que tant que cet écran est ouvert.

Si vous refusez l’autorisation, Écoute de la pièce ne peut pas enregistrer et explique comment
autoriser l’accès. Elle ne lance pas la synthèse en remplacement. Réglage peut enregistrer
uniquement le son de l’application et l’indique explicitement. Le sonar nécessite le microphone.

## Combien de temps les données restent et comment les effacer

Elles restent jusqu'à ce que vous les effaciez. Vous pouvez supprimer un enregistrement précis
ou une session entière depuis les archives, avec confirmation. Désinstaller l'application efface
tout : réglages, journal et enregistrements.

## Les mineurs

Aftervoice ne s'adresse pas aux moins de 13 ans et ne collecte pas délibérément leurs données.

## L'audio que l'application génère

Les sons que produit Aftervoice sont générés par un modèle de voix qui tourne sur le téléphone.
Ce ne sont pas des enregistrements de personnes réelles et ce ne sont la preuve de rien.

L'audio produit par l'application porte une marque lisible par une machine qui le déclare
synthétique, comme l'exige l'article 50 du règlement européen sur l'intelligence artificielle.
La marque est dans le son lui-même, pas dans une étiquette du fichier : elle survit au partage,
à la recompression et à une coupe, et elle est encore là dans un fichier renommé ou réexporté.
N'importe qui peut la vérifier, sans rien nous demander, avec le détecteur décrit dans
[Vérifier la marque](../detector.html).

La marque ne contient rien qui vous concerne : pas d'identifiant du téléphone, ni de la session,
ni de l'installation. Elle dit une seule chose, toujours la même : cet audio a été fait par une
machine. La piste microphone d'un enregistrement n'est pas marquée, parce que ce n'est pas de
l'audio généré — c'est la pièce où vous étiez.

## Contact

Pour toute question sur cette politique : [support@altrovelabs.net](mailto:support@altrovelabs.net).

Responsable du traitement : **Altrove Labs**. Les données du journal et les enregistrements
restent en votre possession et sous votre contrôle, sur votre téléphone. Nous traitons
uniquement les signalements et communications que vous choisissez d'envoyer ; vous pouvez
exercer vos droits RGPD à l'adresse ci-dessus en indiquant, pour un signalement anonyme, sa
référence.

## Modifications

Si cette politique change, la date en haut change avec elle, et la version précédente reste dans
l'historique public du dépôt du site.
