---
title: "L'éco-conception des services de messagerie"
description: "Whatsapp, Discord, Teams, Slack... Y a-t-il une différence d'impact environnemental ?"
tags: ["Greenspector", "Messagerie", "Environnement"]
image: /assets/img/posts/2024/Q2/messageries.webp
thumb: /assets/img/posts/2024/Q2/messageries
podcast: null
---

Greenspector a récemment publié une étude comparative entre différentes applications de messagerie :
- Whatsapp
- Teams
- Discord 
- Slack

On aurait pu penser que ces différentes applications auraient des résultats similaires puisqu’elles répondent à des besoins très proches. Si on peut clairement dégager une tendance générale, on se rend compte qu’il y a tout de même des différences significatives.

Voici les enseignements clés de cette étude.

## Compression d'image

Quand on regarde la consommation de données des applications, on se rend compte que Whatsapp se démarque. Dans le scénario testé, les trois autres applications sont très proches (entre 7,3 et 7,8 Mo) alors que Whatsapp n'utilise que 0,8 Mo !

Cette différence provient du choix de compresser les images avant de les envoyer. Cela permet de largement baisser la consommation de données pour cet outil. Mais cela a également un coût sur la consommation d'énergie.

## Consommation d'énergie

Lorsque l'on se concentre sur l'envoi d'une image de taille importante, on constate que Whatsapp consomme d'avantage d'énergie que ces concurrents (environ 3 fois plus). Cela est dû au choix de compression d'image mentionné plus haut. 

Cela étant dit, l'application compense en étant plus économe sur les autres aspects, ce qui fait qu'au final, sur l'ensemble du parcours testé, elle se retrouve au même niveau que Teams et Discrod (les trois applications se tiennent entre 10.6 mAh et 11.1 mAh).

Slack en revenche est beaucoup plus consommateur (16 mAh). Cette sur-consommation se retrouve à toutes les étapes.

## Intérêt du mode sombre

Pour l'ensemble des applications, le mode sombre permet d'économiser entre 21% et 35% d'énergie. Cela vient rappeler les faits :
- l'écran est ce qui consomme le plus d'énergie dans un smartphone
- le mode sombre a un impact significatif

Je vous invite donc à tester ce mode proposé sur Android et iOS ainsi que sur tous les navigateurs modernes. D'ailleurs, ce site est compatible avec le mode sombre.

## Rétro-compatibilité

Il s'agit probablement du critère le plus important en éco-conception. Quels sont les terminaux compatibles avec les applications développées ? En n'assurant pas la compatibilité avec un téléphone ancien les éditeurs participent à l'obsolescence des terminaux et donc à leur renouvellement anticipé. Pour rappel, la fabrication des terminaux est ce qui pèse le plus lourd dans la balance écologique du numérique ({% include link.html text="étude ADEME-ARCEP" link="https://librairie.ademe.fr/consommer-autrement/5226-evaluation-de-l-impact-environnemental-du-numerique-en-france-et-analyse-prospective.html" %})

On peut voir un bel effort de Whatsapp et Discord, compatibles avec plus de 97% des smartphones. Par contre, Teams et Slack n'ont pas assuré la rétro-compatibilité avec les téléphones Android.

| Application | Version Android minimum | Pourcentage des smartphones Android compatibles | Version iOS minimum | Pourcentage des smartphones iOS compatibles |
|-----|---------|--------|
| WhatsApp | Android 5.0 | 99,5 | iOS12  | 98,8 |
| Discord | Android 7.0 |  97,1 | iOS12  | 98,8 |
| Slack | Android 10 | 84,3  | iOS15  | 94,2 |
| Teams | Android 11 | 75,4 | iOS15  | 94,2  |

*Pourcentage des smartphones compatibles avec les différentes application de messagerie ({% include link.html text="source" link="https://greenspector.com/en/whatsapp-discord-slack-teams-what-is-the-environmental-impact-of-a-user-journey-on-these-applications/" %})*

## Conclusion

Les enseignements clé :
- des applications similaires peuvent avoir des impacts environnementaux différents
- tous les éditeurs n'ont pas la même stratégie de rétro-compatibilité
- le mode sombre permet une réduction significative de l'énergie utilisée par nos smartphones
- la compression est un élément important pour la sobriété d'une application

## Pour aller plus loin

Je vous invite à consulter l'{% include link.html text="étude complète de Greenspector" link="https://greenspector.com/fr/quel-est-limpact-environnemental-dun-parcours-utilisateur-sur-applications-messagerie/" %}.
Vous y verrez notamment :
- le parcours testé
- les impacts environnementaux pour l'ensemble du parcours pour chacun des services
  - impact carbone
  - consommation en eau
  - utilisation des sols