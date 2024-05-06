---
title: "Le numérique responsable pour le jeux olympiques 2024"
description: "Les Jeux Olympiques 2024 de Paris incluent le numérique responsable dans leur organisation !"
tags: ["Environnement", "JO", "Ecoconception", "Numérique responsable"]
image: /assets/img/posts/2024/Q2/thumb-jo.webp
thumb: /assets/img/posts/2024/Q2/thumb-jo
podcast: https://sphinx.acast.com/p/open/s/65e06335dd3dcf001643bd06/e/66227c2435f9560013931306/media.mp3
---

Voilà une belle nouvelle, surtout quand on écoute le {% include link.html link="https://www.rtl.fr/actu/debats-societe/jeux-olympiques-jean-marc-jancovici-retrace-le-bilan-carbone-de-l-evenement-7900336454" text="rapide décryptage de Jean-Marc Jancovici sur RTL" %}, qui souligne le poids très important du numérique dans les conséquences environnementales de l’organisation des jeux.

## Les engagements

La démarche numérique responsable est formalisée dans un {% include link.html text="document de 18 pages" link="https://medias.paris2024.org/uploads/2024/01/Paris2024-231201-SUS-Guide-strategie-numerique.pdf" %} publiquement accessible. Cette dernière semble principalement s’intéresser à l’impact environnemental des jeux. C’est déjà un bon premier pas, mais c’est dommage d’oublier les autres axes (accessibilité, inclusion, éthique…)

On y voit donc 5 engagements clés :

1. Au moins 70 % des équipements seront loués
2. 100 % des équipements achetés auront une seconde vie
3. Eco-conception des applications grand public
4. Sensibilisation des collaborateurs et de l’écosystème de Paris 2024
5. Des critères numérique responsable pour 100 % des appels d’offre technologiques

De manière générale, on voit une démarche très vertueuse. Mais voyons ce que cela donne pour l’éco-conception des services grand public.

## L'éco-conception

On va s'intéresser à la page vitrine la plus visible des jeux, la page d’accueil du site {% include link.html text="paris2024.org" link="https://olympics.com/fr/paris-2024" %} :
- 541 requêtes
- Taille de la page : 21,7 Mo
- DOM : 2394 éléments
- 29 erreurs JS
- EcoIndex : 5,08/100 (G)

Non seulement, on est loin de la perfection… mais surtout c’est une des pages les plus lourdes qu’il m’ait été donné de mesurer.

Pourtant quand on regarde leur {% include link.html text="démarche d’éco-conception" link="https://olympics.com/fr/paris-2024/information/eco-conception" %}, on voit qu’il y a eu un travail effectué. Il semble même y avoir eu un résultat puisque d’après leur scoring interne, la page est passée d’un score de 33/100 à un score de 51/100 en un an. Mais à quoi pouvait ressembler la page en 2022 ?

Concrètement, il suffit de lire les bonnes pratiques mises en place pour se rendre compte qu’ils n’ont pas voulu faire les gestes les plus impactants. 
Chargements asynchrones, redimensionnement d’images, optimisation des polices… Il s’agit là de bonnes pratiques, mais…

### La démarche d’éco-conception ne se limite pas à un travail technique.

Quand on regarde cette page, il est évident qu’il faut travailler sur sa conception. Il faut se demander à quoi elle sert et la concevoir en conséquence.
- Le carousel en haut de page est-il nécessaire ? Le défilement doit-il être automatisé ? Peut-on réduire la taille des images ?
- Le découpage des actualités est-il pertinent ? Faut-il mettre en avant autant de contenu ?
- Est-il nécessaire d’expliquer aux internautes comment acheter un billet de train ?
- La boutique ne doit-elle pas être déportée sur une autre page ?
- La FAQ ne doit-elle pas être déportée sur une autre page ?

Pour faire plus simple : il y a trop de contenus, trop d’images et d’animation. Il est nécessaire de faire un travail de sélection pour améliorer le score environnemental de cette page. Cela permettrait également de mieux guider les visiteur.se.s vers les contenus pertinents.

### Il faut faire le travail technique là où cela pèse le plus

C’est ce qui a été réalisé pour le CSS. 100 ko de CSS pour cette page, cela me semble être tout à fait raisonnable. On aurait peut-être pu réduire le nombre de fichiers, mais c’est déjà du pinaillage.

De même vu le nombre et la taille des images, je trouve que le travail technique à ce niveau est plutôt réussi (8,6 Mo)

Pourquoi la même démarche n’a-t-elle pas réalisée pour le javascript ? 12,2 Mo de javascript pour cette page, c’est beaucoup trop ! Il y a là tout un travail de refonte à réaliser. Je suppose qu’il doit y avoir une réelle dette technique. C’est dommage parce que c’est là qu’il faut faire l’effort.

## Conclusion

Merci beaucoup à l’organisation des jeux de prendre l’impact environnemental du numérique en compte. La démarche est louable et certaines actions semblent réellement permettre de réduire le bilan de ces jeux.
J’aurais toutefois apprécié que la démarche inclut également une sobriété dans les fonctionnalités. La réduction du nombre et de la taille de certains écrans mis à disposition va dans ce sens. La page d’accueil devrait être le symbole de cette sobriété. Cela aurait également permis de créer un précédent avec une page sobre et efficace pour un site à très forte visibilité et affluence… 

En réalité, j’espère qu’un jour on trouvera qu’une page aussi riche que la page d’accueil des JO sera ringarde...
