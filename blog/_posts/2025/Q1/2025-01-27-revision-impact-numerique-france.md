---
title: "Proposition de révision de l'impact environnemental du numérique"
description: "L'ADEME a jeté un pavé dans la mare avec la révision de son rapport sur les impacts environnementaux du numérique français. Voici ma proposition sur le sujet."
tags: ["ADEME", "ACV", "Datacenter", "France"]
image: /assets/img/posts/2025/Q1/thumb-revision-impact-num-france.jpg
thumb: /assets/img/posts/2025/Q1/thumb-revision-impact-num-france
alt-image: "Un centre de données regroupant l'ensemble des symboles de la France."
podcast: null
---

## La mise à jour de l'étude de l'ADEME

Dans [cet article paru mi-janvier](/blog/2025/01/14/impact-environnemental-numerique-france), je parlais de la mise à jour de l'analyse du cycle de vie du numérique en France par l'ADEME. Le rapport montrait notamment un impact beaucoup plus important pour les centres de données.

On passe ainsi de 16% de l'impact carbonne du numérique français dû aux datacenters à 46% avec le nouveau modèle mis à jour. Cela semble étonnant et cela amène à quelques réflexions sur la méthodologie du rapport de l'ADEME. Il y a deux critiques importantes :

- l'absence de revue critique formalisée dans le rapport
- aucun nouvel inventaire n'a été réalisé, les modificications ont été uniquement réalisées sur des modèles projectifs

## Un modèle et une méthodologie criticable

Or le message apporté par ce nouveau rapport qui vient à l'encontre de ce que l'on trouve dans la littérature sur l'impact environnemental du numérique mérite d'être étayé par des arguments plus solides qu'une projection mathématique.

Le modèle utilisé dans la mise à jour prend comme hypothèses principales :

- La France a une répartition Traditionnel/Cloud similaire au modèle monde
- Les datacenters externes utilisés en France sont exclusivement de type Cloud

Je vous invite à lire la méthodologie complète proposée sur {% include link.html text="le site du Hubblo" link="https://hubblo.org/fr/blog/datacenters-imported-impacts/" %}.

Cette approche, quoique sensée et transparente, ne me semble pas être assez robuste pour étayer un changement radical dans les ordres de grandeurs d'impact entre les terminaux et les centres de données. 

## Autre modèle possible

Pour prouver qu'avec des hypothèse sensées, il est possible d'avoir des résultats très différents, je vais adopter une démarche similaire avec une hypothèse de départ tout aussi acceptable que celle de Hubblo :

> Le rapport entre la consommation électrique à l'usage des centres de données et la consommation électrique des terminaux utilisateurs est similaire à l'échelle mondiale et à l'échelle des usages Français.

Pour celles et ceux que cela intéresse, je vous invite à consulter la [méthodologie complète](/blog/2025/01/27/methodologie-revision-impact-numerique-france).

## Résultats

Je vous propose de comparer 4 études qui évaluent l'impact du numérique en France pour l'année 2020 :
- L'{% include link.html text="étude ADEME-ARCEP originale" link="https://www.arcep.fr/uploads/tx_gspublication/etude-numerique-environnement-ademe-arcep-volet02_janv2022.pdf" %} publiée en avril 2022 
- La {% include link.html text="révision des données de cette même étude avec le modèle Masanet" link="https://librairie.ademe.fr/ged/9522/Evaluation-impact-numerique-ADEME-Arcep-2025.pdf" %} publiée en 2025
- La révision de cette étude avec le modèle (Simbios) que j'expose dans cet article
- l'étude Green IT : {% include link.html text="iNUM : impacts environnementaux du numérique en France" link="https://www.greenit.fr/impacts-environnementaux-du-numerique-en-france/" %} publiée en janvier 2021

On va se concentrer sur l'impact climatique.

| Etude                         | Terminaux | Réseaux | Datacenter |
| ----------------------------- | --------- | ------- | ---------- |
| ADEME – ARCEP 2020 (original) | 13,30     | 0,93    | 2,64       |
| ADEME – ARCEP 2020 (Masanet)  | 13,30     | 0,93    | 10,5       |
| ADEME – ARCEP 2020 (Simbios)  | 13,30     | 0,93    | 3,04       |
| iNUM France – GreenIT         | 20,16     | 2,4     | 1,44       |

*Impact climatique du numérique en France suivant différentes études (en Mt CO<sub>2</sub>eq)*

{% responsive_image 
  path: "assets/img/posts/2025/Q1/impact-co2-france-2020.webp"
  alt: "Graphique présentant les données ci-dessus."
  default_type: "png"
%}

## Ce qu'il faut retenir

En tentant de quantifier les mêmes impacts, et pour trois études, en se basant sur les mêmes jeux de données, on peut arriver à des résultats différents. Voire très différents.

Est-ce que le modèle que je défends est plus précis que les autres ? Je le pense, mais je n'en suis pas certain et je ne peux certainement pas le prouver. Par contre, il est cohérent avec l'ensemble de la littérature scientifique sur l'impact environnemental du numérique.

Le message apporté par la mise à jour de l'étude de l'ADEME est trop disruptif pour être annoncé avec un rapport sans revue critique des pairs et sans mise à jour des données.