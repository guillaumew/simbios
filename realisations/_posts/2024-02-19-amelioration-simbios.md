---
title: Amélioration du site Simbios.fr
description: Aller un cran plus loin dans la sobriété avec le site vitrine Simbios.
tags: ["Ecoconception", "Optimisation", "Site"]
image: /assets/img/posts/2023/Q4/thumb-simbios.webp
thumb: /assets/img/posts/2023/Q4/thumb-simbios
---

## Contexte

J'avais détaillé dans un [article l'année dernière](/realisations/2023/11/14/simbios.html) comment le site simbios.fr avait été créé.

J'y avais noté des idées d'améliorations :
- Intégrer le logo en CSS
- Passer à du CSS natif
- Remplacer l’analytics par des statistiques côté hébergement
- Mieux gérer les images dans la partie blog

## Améliorations 

J'ai finalement décidé de conserver mon outils d'analytics qui me donne des informations extrêmement précieuses (par exemple, une grosse partie des visiteur.se.s utilisent un iPhone, il font donc que je sois attentif à ce que mon site fonctionne sur ces appareils que je ne possède pas).

Par contre, j'ai bien réalisé toutes les autres optimisations. 
- Le logo (qu'on retrouve dans le menu, le footer et sur la page d'accueil) est bien chargé dans le CSS
- J'ai retiré le framework PureCSS. Je n'ai conservé que Normalize pour éviter les incohérences entre les navigateurs. Tout le reste est géré en CSS fait sur mesure. Il n'y a donc plus de code non utilisé.
- J'ai maintenant 3 tailles d'images dans la partie blog. En fonction de votre taille d'écran, vous aurez une image plus ou moins grande.

A ces optimisations s'ajoutent certaines fonctionnalités nouvelles comme la gestion du mode sombre, l'ajout des statistiques de la page dans le footer, la gestion d'un menu dynamique (nécessaire sur petits écrans).

## Résultats

Malgré ces derniers ajouts, la taille de la page d'accueil a encore bien réduit.

| Statistique | Novembre 2023 | Février 2024 |
|-------------|---------------|--------------|
| DOM         | 102           | 139          |
| Requêtes    | 8             | 6            |
| Transferts  | 22.9 ko       | 17.7 ko      |
| Taille      | 51.3 ko       | 31.0 ko      |

Le DOM a augmenté puisque du contenu a été ajouté, mais sinon tous les indicateurs sont en baisse et avec une taille de la page qui diminue de 40% !

Comme l'ensemble du code est utile, on peut maintenant regarder quelles sont les parties qui pèsent le plus lourd. Voici les catégories :
- **Aspect général** : apparence des éléments, organisation de la page, couleurs, le logo...
- **Menu** : le menu noir en haut de page
- **Splash** : le haut de page en bleu avec le logo et le titre
- **Services** : la présentation des services en 5 étapes
- **Présentation Guillaume** : la partie avec me photo et description
- **Contact** : la partie en bas de page avec la possibilité d'envoyer un message et de me suivre de manière variée
- **Footer** : la partie en bleu tout en bas de page avec les mentions légales et les stats de la page.
- **Analytics** : l'outil qui permet d'avoir des statistiques de fréquentation sur le site
- **SEO** : l'ensemble des données pour que les moteurs de recherches ou réseaux sociaux puissent répertorier le site.
- **Darkmode** : le CSS pour accepter le mode sombre si l'option est choisie sur le navigateur.

{% responsive_image 
  path: assets/img/posts/2024/Q1/simbios-fr-breakdown.webp
  default_type: png 
  alt: "Les gros de la taille vient de l'aspect général. Les icones et la photos pèsent également pour les services et la présentation" 
  title: "Répartition de la taille de la page d'accueil simbios.fr par fonctionnalité"
%}

Si l'aspect général est toujours ce qui pèse le plus lourd, on voit maintenant que le contenu texte est maintenant clairement visible avec par exemple la partie contact qui malgrés l'absence d'image et icône approche les 10% de la page.

Les icônes de la partie services et ma photo de profil font de ces sections les sections les plus importantes. On voit également que la partie SEO n'est pas négligeable avec 7% de la taille totale de la page.

## La suite ?

On ne peut maintenant plus réellement envisager de réduction de la taille de la page sans retirer du contenu ou des fonctionnalités. Je pourrais décider de gagner quelques kilos en retirant les icônes de la partie service pour mettre de chiffres par exemple, ou décider de sortir la partie contact et d'imposer de cliquer sur le lien proposé dans le menu.

A l'heure actuelle, je ne pense pas faire ces choix. Je pense au contraire que la page d'accueil va s'étoffer davantage de contenus. Je pense qu'elle est arrivée à son point le plus bas en terme de taille.

Il me reste encore à bien vérifier la compatibilité avec l'ensemble des appareils ainsi qu'à travailler sur l'accessibilité. Ce seront mes prochains chantiers. J'ai dors et déjà vu que faire fonctionner un site sur Windows XP ou Vista relevait du quasi-impossible. On verra ce que l'on peut faire.