---
title: "Mettre à jour un vieux smartphone et quitter Google"
description: "Comment donner un coup de neuf sur nos anciens équipements avec des logiciels libres."
tags: ["Logiciel", "Obsolescence", "GAFAM", "Android", "Google", "Open Source"]
image: /assets/img/posts/2025/Q1/thumb-update-phone.jpg
thumb: /assets/img/posts/2025/Q1/thumb-update-phone
alt-image: "Un smartphone en mode recovery"
podcast: https://sphinx.acast.com/p/open/s/65e06335dd3dcf001643bd06/e/677f9939e83bfb002ddfc5ea/media.mp3
---

## Contexte

Comme vous le savez, les plus gros impacts environnementaux du numérique proviennent de la fabrication des terminaux. Il convient donc de savoir comment faire durer nos équipements le plus longtemps possible.
Il y a quelque temps, j'avais écrit ma [démarche pour continuer à utiliser un ordinateur de 12 ans](/blog/2023/10/23/un-ordi-de-12-ans). Il fonctionnait d'ailleurs encore à merveille avant que je me le fasse voler...

Aujourd'hui on va s'intéresser à mon smartphone. Il s'agit d'un OnePlus 5T que j'ai acheté en 2017. Il me convient encore parfaitement, mais OnePlus ne met plus à jour son système d’exploitation OxygenOS. Je suis donc bloqué sur Android 10 dont le support a été définitivement arrêté en mars 2023.

Cela peut poser plusieurs problèmes. 
- Premièrement, il peut y avoir des problèmes sécurité car il peut exister des failles qui ne sont donc plus corrigées. Je n'étais pas plus inquiet que cela à ce sujet puisque je fais attention à mes usages. Mais il vaut toujours mieux être prévenant.
- Je ne bénéficie pas des nouvelles fonctionnalités proposées sur les nouvelles versions d'Android. Autant vous dire que je ne suis pas du tout impacté... en réalité, je ne saurais même pas dire quelles sont ces nouvelles fonctionnalités.
- Les applications vont progressivement arrêter le support des anciennes versions des systèmes d'exploitation. Je vais donc soit devoir rester sur de vieilles versions d'applications, voire même ne pas pouvoir installer certaines applications.

Pour le moment, j'étais relativement épargné par ces problèmes et j'étais pleinement satisfait du fonctionnement de mon smartphone. Ce dont j'étais moins satisfait, c'est l'usage que j'en avais. Comme beaucoup de gens, j'ai tendance à sortir mon téléphone dès que j'ai quelques secondes d'inaction. Incapable de changer cette habitude que je juge pourtant néfaste, j'ai progressivement désinstallé toutes les applications de divertissement. Mais il reste toujours Youtube qui ne peut pas être désinstallé comme les autres applications.

## Objectifs

Quitte à devoir faire des opérations avancées sur mon téléphone pour pouvoir retirer Youtube (que je suis a priori incapable de m’empêcher d'ouvrir), je vais en profiter pour mettre à jour Android.

Il existe pas mal d'initiatives comme {% include link.html link="https://grapheneos.org/" text="GrapheneOS" %}, {% include link.html  link="https://calyxos.org/" text="CalyxOS" %} ou {% include link.html  link="https://www.ubuntu-touch.io/" text="Ubuntu Touch" %}. Mais ces OS ne fonctionnent  que sur une poignée de terminaux. Seuls {% include link.html  text="/e/OS" link="https://e.foundation/e-os/" %} et {% include link.html  text="LineageOS" link="https://lineageos.org/" %} proposent un support étendu (qui inclut mon OnePlus 5T).

J'ai opté pour Lineage parce qu'il m'a été recommandé, mais honnêtement je n'avais pas vraiment d'argument pour aller dans un sens ou dans l'autre. Cependant, je me suis également rendu compte qu'il était possible d'utiliser ces OS pour "déGoogliser" mon smartphone. Je me dis que c'est une bonne occasion pour tester un monde sans Google.

## Installer LineageOS

Je ne vais pas tenter d'expliquer ici comment faire pour installer LineageOS ou /e/OS. Je renvoie directement à leurs documentations. Je tiens toutefois à souligner qu'il s'agit d'une opération à réserver aux utilisateurs et utilisatrices avancé.es.

Au final, cet OS est très similaire à n'importe quelle surcouche Android. Je n'ai aucun mal à m'adapter, pourtant cela fait 7 ans que j'utilise OxygenOS...

## Réinstaller les applications

Une fois le nouvel OS installé, il faut donc rétablir les applications ou tout du moins choisir les services que je souhaite conserver. Rendez-vous donc sur le Play Store pour... ah bah non... Je n'ai pas installé les services Google, donc il n'y a pas Google Play Store...

### Gestionnaire d'applications

C'est donc parti pour installer un nouveau catalogue d'applications. Après quelques tentatives je décide d'installer {% include link.html link="https://f-droid.org/fr/" text="F-Droid" %} pour avoir accès à des applications open source. Mais j'ai également dû installer {% include link.html link="https://gitlab.com/AuroraOSS/AuroraStore" text="Aurora Store" %} pour installer les applications d'éditeurs dont je ne peux pas me passer (Whatsapp, Slack, Discord...)

### Navigateur

Pour surfer sur le web, je me sépare donc de Chrome sur mobile. J'ai beaucoup hésité entre utiliser Mozilla Firefox ou Brave Browser. Je voulais contribuer à la vision d'un Internet libre que je partage avec la fondation Mozilla, mais au final, la navigation par défaut sans publicité de Brave m'a fait basculé.

Par commodité, je vais également utiliser le moteur de recherche de Brave. Cela permettra à la société qui gère le navigateur d'avoir une rétribution pour la mise à disposition du logiciel.

### Client mail

Aujourd'hui la plupart des services mails viennent avec leur solution applicative. C'est le cas pour mon Gmail perso mais également pour mon adresse pro (Infomaniak). Pour remplacer Gmail, je me suis créé une adresse mail avec un de mes domaines perso. Cela permettra de migrer toute la famille si l'essai est concluant. Je vais donc remplacer Gmail par un client mail IMAP classique. Que ce soit sur PC ou sur smartphone, j'ai décidé de faire confiance à Mozilla avec Thunderbird et K9-mail.

Je n'ai donc pas (encore) supprimé mon adresse Gmail... Cela viendra peut-être dans le futur, mais pas avant une année. Ce n'est pas si simple de se séparer d'une adresse mail qui a été utilisée pendant plus de 15 ans ! Je vais progressivement rediriger mes contacts vers la nouvelle adresse. Mon Gmail sera supprimé quand il ne sera plus utilisé.

### Agenda et contacts

Tous mes rendez-vous et contacts sont gérés par Google. Je décide de tout basculer sur {% include link.html text="Nextcloud" link="https://nextcloud.com/fr/" %}. Deux petits exports côté Google, deux imports côté Nextcloud et le tour est joué, j'ai tout mon historique sur mon téléphone et en ligne (sans Google).

Bonus, Nextcloud pourra également gérer le partage de notes et de fichiers.

### GPS

Au revoir Google Maps. Inutile également d'envisager Waze qui a été racheté par Google il y a quelque temps déjà.

Je vais tester Magic Earth et Organic Maps. J'aime bien l'idée d'Organic Maps qui a un fonctionnement 100% offline. Il faut bien penser à télécharger les cartes en amont et il n'y a pas d'information sur le trafic, mais c'est bien plus sobre en termes de fonctionnement. Et puis, à vélo, il n'y a pas de bouchon !

### Les photos et vidéos

Jusqu'à présent j'ai remplacé l'ensemble des services Google par des solutions très proches qui ne vont quasiment pas me demander de changer mes usages.

Pour les photos, en revanche, je vais opter pour un stockage 100% local. J'aurais pu choisir de payer un espace pour pouvoir les stocker sur Nextcloud par exemple et conserver le fonctionnement actuel de Google Photos.

Mais, pour réduire les impacts de mes photos on ne va rien mettre dans le cloud. Mes photos iront directement de mon téléphone vers mon ordinateur avec une sauvegarde automatique.

Concrètement, cela signifie que périodiquement, je vais connecter mon téléphone à mon ordinateur pour charger les photos. J'en profiterai pour faire un tri et éviter de sauvegarder ce qui n'a pas vocation à être conservé. Ce sera aussi l'occasion de vider les photos présentes sur mon téléphone.

Le seul désavantage que j'y vois, c'est que je ne pourrai montrer mes anciennes photos que depuis mon domicile. Mais bon cela m'arrive tellement peu souvent...

Le tri que j'opérerai me permettra d avoir moins de fichiers et de revoir avec plus de plaisir mes vieilles photos.

### La musique

Au revoir Youtube Music, Amazon music, Spotify ou même Deezer. Pour la musique, on va revenir aux bons vieux MP3 directement téléchargés sur mon téléphone. Bon, ça fonctionne pour moi puisque j'écoute souvent la même chose.

Mais j'aime aussi les découvertes donc je bascule sur {% include link.html text="Jamendo" link="https://www.jamendo.com/" %} pour découvrir des artistes indépendants.

Pour les podcasts, ce sera {% include link.html link="https://antennapod.org/fr/" text="AntennaPod" %}.

### Les autres applications

J'ai profité de cette mise à jour pour installer le strict minimum. Les applications de divertissement ont entièrement disparu de mon téléphone ce qui inclut les jeux, les réseaux sociaux et les vidéos (peut-être que je réinstallerai LinkedIn pour la veille).

A cela, j'ai ajouté des applications qui me sont nécessaires comme les outils de communication (Whatsapp, Slack, Teams, Discord...) et des applications qui sont utiles pour faire fonctionner des objets dans la maison (majoritairement de la domotique)

## Pourquoi déGoogliser mes activités ?

Maintenant que j'ai trouvé une alternative pour l'ensemble des services Google, je prends la pleine mesure de ma dépendance au géant américain. Je me reposais sur les services de Google pour beaucoup de choses. 

Cela me rend vulnérable aux divers choix que pourrait réaliser la direction de Google. Par exemple, la fin de service de Google Play m'avait forcé à changer ma manière d'écouter de la musique et pour être honnête cela m'a pas mal restreint dans mon écoute. Bon, pour la musique ce n'est pas très important... mais si les règles d'usages changent pour l'utilisation de Gmail ou de l'agenda ou des contacts ? Cela pourrait être dramatique.

C'est d'ailleurs ce qui m'avait initialement poussé à changer le système d'exploitation. Google ne maintient plus Android 10, OnePlus ne met plus à jour OxygenOS pour mon appareil... je dois donc me tourner vers l'open source !

Dans mon cas, la dépendance à une seule entreprise qui me fournit un service gratuit me fait un peu peur. C'est pour cela que la grande majorité des applications que j'ai présentées sont open sources. Cela me permet de ne pas subir les choix d'un éditeur, car le code peut être repris par une communauté (voire est géré par une communauté). 

A cela s'ajoute également l'usage des données réalisé par Google. L'ensemble des outils offerts par Google a un coût qui se nomme les données personnelles. La simplicité d'usage des outils Google me laisse à penser que l'échange est équitable. D'un côté Google me met à disposition des outils simples et performants, de l'autre j'autorise le géant à collecter et utiliser mes données à des fins publicitaires. Mais je sais que tout le monde n'est pas de cet avis.

> Si vous ne payez pas un service, c'est que vous êtes le produit

Je vois aussi cette démarche comme un test. Comment vais-je vivre ma séparation des outils Google ? On en reparle dans 6-12 mois ? 

### Ai-je vraiment coupé toutes mes dépendances aux GAFAM ?

Bien sûr que non...

- Lineage OS est basé sur Android qui est supporté par Google.
- Brave Browser est un navigateur basé sur Chromium qui est développé par Google
- Whatsapp est édité par Facebook 
- J'utilise encore Teams (Microsoft), LinkedIn et Slack

Nous vivons dans un monde complexe où nous nous appuyons sans cesse sur le travail des autres (cf l'[article sur la galette des rois maison](/blog/2024/01/10/galette-des-rois-et-complexite-economique)). Avec la taille des géants du numérique comme les GAFAM (Google, Amazon, Facebook, Apple et Microsoft), il parait utopique que l'on puisse avoir une vie numérique sans qu'ils ne soient sollicités.

Mais on peut au moins limiter notre dépendance et surtout la rendre moins directe...

Surtout que des alternatives existent et qu'elles ont l'air d'être tout aussi efficaces que les services des géants américains. Promis, je vous fais un retour d'expérience dans quelques mois !