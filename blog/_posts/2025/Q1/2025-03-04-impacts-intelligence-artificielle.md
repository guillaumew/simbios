---
title: "La place de l'intelligence artificielle dans les centres de données mondiaux"
description: "Appuyons-nous sur le rapport GreenIT.fr pour évaluer les impacts environnementaux de l'intelligence artificielle."
tags: ["Intelligence artificielle", "Green IT", "ACV", "Environnement", "Monde"]
image: /assets/img/posts/2025/Q1/thumb-intelligence-artificielle.jpg
thumb: /assets/img/posts/2025/Q1/thumb-intelligence-artificielle
alt-image: "L'image d'un visage ethéré ou artificiel."
podcast: https://sphinx.acast.com/p/open/s/65e06335dd3dcf001643bd06/e/67c9cea322c74795c306c2ca/media.mp3
---

Le rapport GreenIT.fr sur [les impacts environnementaux du numérique dans le monde](/blog/2025/02/06/impacts-numerique-monde) propose un volet sur l'intelligence artificielle. Il s'agit de l'une des rares études qui propose une approche générale en s'appuyant sur une méthodologie sérieuse.

On le sait, l'intelligence artificielle vient principalement solliciter les serveurs des centres de données. En 2023 (année étudiée), les usages sont encore restreints et les flux de données restent minimes comparés aux flux vidéos par exemple. GreenIT.fr a donc pris le parti de se concentrer uniquement sur les impacts de l'intelligence artificielle sur les centres de données.

## Composition des centres de données

Les centres de données regroupent près de 80 millions de serveurs dont environ 2% sont dédiés à l'intelligence artificielle.

{% responsive_image 
  path: "assets/img/posts/2025/Q1/repartition-serveurs-monde.webp"
  alt: "Graphique présentant la répartition des serveurs dans le monde."
  default_type: "png"
%}

On voit qu'à ce stade les serveurs d'intelligence artificielle ne constituent qu'une faible partie de l'ensemble des serveurs, mais ils constituent déjà une part considérable des serveurs de calculs. Si on écarte les serveurs de stockage, les serveurs consacrés à l'intelligence artificielle constituent plus d'un tiers (37%) des serveurs de calculs.

## Consommation électrique des centres de données

Seulement, on le sait, les serveurs dédiés à l'intelligence artificielle sont particulièrement performants et nécessitent donc beaucoup plus d'électricité pour fonctionner.

{% responsive_image 
  path: "assets/img/posts/2025/Q1/consommation-electrique-datacenter.webp"
  alt: "Graphique présentant la consommation électrique des centres de données dans le monde."
  default_type: "png"
%}

Les serveurs de l'intelligence artificielle consomment un part importante de l'électricité des centres de données. En plus des 18,1 % directement consommés par les serveurs, une part de de la consommation des équipements réseau et non-IT doit également être imputée aux usages de l'intelligence artificielle (ces serveurs ayant également besoin d'un accès au réseau et devant être refroidis).

## Impacts environnementaux

Lorsque l'on retranscrit cela en impacts environnementaux on trouve :

| Equipement | Changement climatique (en kg CO<sub>2</sub>eq) | Utilisation de métaux et minéraux (en kg Sb eq) |
|---|---|---|
| High-End                  | 1 282 400 000   | 8 200     |
| Mid-Range                 | 19 419 200 000  | 143 500   |
| Stockage lent             | 79 508 800 000  | 1 340 700 |
| Stockage rapide           | 95 630 400 000  | 635 500   |
| Intelligence artificielle | 72 364 000 000  | 430 500   |
| Equipement réseau         | 10 442 400 000  | 98 400    |
| Equipement non IT         | 138 865 600 000 | 2 578 900 |

On peut mettre ces données en image en les comparant aux limites planétaires proposées par le {% include link.html text="JRC (Joint Research Centre)" link="https://www.sciencedirect.com/science/article/pii/S0301479720306186#tbl3" %}.

{% responsive_image 
  path: "assets/img/posts/2025/Q1/impacts-environnementaux-datacenters.webp"
  alt: "Graphique présentant les impacts environnementaux des centres de données dans le monde."
  default_type: "png"
%}

On se rend compte que les serveurs de l'intelligence artificielle constituaient en 2023 plus de 1 % de la limite planétaire d'émissions de gaz à effet de serre. Cela fait lourd pour un usage encore peu développé. 

Et encore ! Cela n’inclut pas la part des équipements nécessaires à faire fonctionner ces serveurs dans les datacenters (climatisation, réseau, onduleurs, etc.) .Cela n’inclut pas non plus la part des usages de l’intelligence artificielle sur les terminaux utilisateurs et sur les infrastructures réseaux.

## Conclusion

Les centres de données restent majoritairement constitués de serveurs de stockage (d'où leur nom !). Toutefois, les impacts environnementaux de ces derniers proviennent de sources variées. Les serveurs configurés pour l'intelligence artificielle viennent prendre une place importante avec une part de 13 % des émissions de gaz à effets.

En 2023, les serveurs de l'intelligence artificielle constituent à eux seuls 1 % de la limite planétaire climatique. Chiffre qui sera amené à évoluer rapidement dans les années à venir...