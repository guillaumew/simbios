---
title: "L'impact environnemental du numérique en France"
description: "L'ADEME propose une mise à jour de l'impact environnemental des usages numériques en France."
tags: ["ACV", "ADEME", "France", "Environnement", "Datacenter"]
image: /assets/img/posts/2025/Q1/thumb-impact-num-france.jpg
thumb: /assets/img/posts/2025/Q1/thumb-impact-num-france
alt-image: "Les usages numériques français compte pour 4,4% de l'empreinte carbone du pays en 2022"
podcast: https://sphinx.acast.com/p/open/s/65e06335dd3dcf001643bd06/e/67877a8a21ed2db9f73b8ed8/media.mp3
---

Début 2025, l'ADEME propose une mise à jour de son étude sur les impacts environnementaux du numérique. La précédente étude était sortie en 2022 sur l'année 2020. Cette étude porte sur l'année 2022.

## Changement méthodologique

Cette étude contient un changement méthodologique majeur en ce qui concerne les datacenters. On oublie la simplification précédente qui ne mesurait que les usages des centres de données français. Cette fois-ci on va chercher à modéliser l'ensemble des centres de données utilisés lors des usages en France. Ces centres de données peuvent se trouver à l'étranger.

**Cela a un impact majeur sur les données finales.**

Par exemple, en 2022, l'ADEME communiquait sur des émissions de gaz à effet de serre totales pour le numérique français de 17 Mt CO<sub>2</sub>eq en 2020. Pour cette même année, avec cette mise à jour méthodologique, on passe à 25 Mt CO<sub>2</sub>eq. Soit près de 50% de plus !!!

## Chiffres clés

### Une augmentation importante des gaz à effet de serre

En 2022, le numérique contribuait donc pour 4,4% des émissions de gaz à effet de serre du pays soit 29.5 Mt CO<sub>2</sub>eq. Cela représente 429 kg CO<sub>2</sub>eq par habitant. 

Il s'agit également d'une augmentation des émissions de gaz à effet de serre de 18% en 2 ans.

A ce rythme, l'impact du numérique pourrait tripler d'ici à 2050. Cela signifie que la limite planétaire climatique d'un français moyen sera atteinte rien qu'avec ses activités numériques !

### Le rôle important des datacenters

Jusqu'à présent le message des impacts environnementaux du numérique était clair. "L'impact environnemental du numérique provient principalement des terminaux utilisateurs". C'était d'autant plus le cas en France dont l'électricité décarbonée faisait encore plus pencher la balance sur la fabrication des terminaux utilisateurs. Ces derniers représentant 79% de l'empreinte carbone du numérique en France.

{% responsive_image 
  path: assets/img/posts/2025/Q1/methodologie-dc-vs-terminaux.webp 
  alt: "Avec la nouvelle méthodologie les datacenters pèsent presque autant que les terminaux."
%}
*La prise en compte de l'usage de centres de données étrangers dans les usages numériques français change la donne.*

Avec cette nouvelle méthodologie, les datacenters ont une empreinte carbone presque équivalente aux terminaux utilisateurs. De plus, la part des datacenters augmente, notamment avec la démocratisation de l'intelligence artificielle.

Il est d'ailleurs important de préciser qu'en 2022 l'intelligence artificielle n'était pas aussi populaire qu'elle l'est aujourd'hui. Il faut donc s'attendre à une augmentation d'autant plus importante des datacenters à l'avenir.

## Vue panoramique de l'étude

Les impacts environnementaux ne se limitent pas au climat. L'étude de l'ADEME inclut des données sur :

- L'utilisation des métaux ([Késako ?](/blog/2024/05/27/utilisation-des-metaux))
- Utilisation d’énergies fossiles et nuclaires ([Késako ?](/blog/2024/04/30/epuisement-ressources-fossiles))
- Changement climatique ([Késako ?](/blog/2024/05/21/changement-climatique))
- Radiations ionisantes ([Késako ?](/blog/2024/12/09/radiations-ionisantes))
- Émissions particules fines ([Késako ?](/blog/2024/07/10/particules))
- Écotoxicité ([Késako ?](/blog/2024/01/30/ecotoxicite-eau))
- Acidification ([Késako ?](/blog/2024/03/05/acidification))
- Formation ozone photochimique ([Késako ?](/blog/2024/07/30/formation-ozone-photochimique))

Pour pouvoir les afficher sur un même graphique, je vais utiliser une unité de mesure commune qu'on appelle le "Planet Boundary per capita". Le {% include link.html text="Joint Research Centre" link="https://www.sciencedirect.com/science/article/pii/S0301479720306186#tbl3" %} propose une limite planétaire pour chacun des impacts cités. J'ai ensuite ramené cette limite planétaire à la France. Je vais donc exprimer les impacts en pourcentage de la limite planétaire viable selon le JRC.

{% responsive_image 
  path: assets/img/posts/2025/Q1/impact-num-france-2024.webp 
  alt: "Graphique présentant les impacts environnementaux du numérique en France"
  default_type: "png"
%}

*Les impacts environnementaux du numérique français en PBPC*

Il faut lire ce graphique ainsi : Le numérique en France atteint 50% de la limite planétaire pour le changement climatique. A cela il faudrait également ajouter les contributions des autres secteurs (transport, alimentation, logement...). Sur ces 50%, 21 points sont dus à la fabrication, distribution et fin de vie des terminaux et 4 pts sont dûs à l'utilisation des terminaux.

On constate que les terminaux utilisateurs restent la principale cause d'épuisement des ressources non énergétiques (métaux). Ces derniers nécessitent beaucoup d'électricité pour fonctionner (utilisation d'énergies fossiles et nucléaire) mais leur utilisation n'a pas beaucoup d'impact sur le climat, car l'électricité française est relativement décarbonée.

Pour une totale transparence, vous trouverez les données ayant permis d'arriver à ce résultat sur {% include link.html text="cette feuille de calcul partagée" link="https://kdrive.infomaniak.com/app/share/894812/abfd2705-6c52-4fc0-ace9-d37c7a1ff13b" %}.

## Conséquences

Cette étude risque de bouleverser le monde du Green IT en France.

Elle met en relief la part importante des centres de données dans l'empreinte environnementale du numérique en France, alors qu'il s'agissait d'une idée reçue qu'on devait désamorcer lors des formations.

Cela montre également l'importance de bien faire attention aux hypothèses réalisées. Ces dernières peuvent avoir des effets importants sur les résultats finaux.

D'ailleurs l'ADEME est transparente sur les limites de cette nouvelle étude :

- pas de prise en compte des réseaux télécoms hors de France
- pas d’actualisation détaillée des data centers en France
- pas de prise en compte du développement de l’IA générative
- pas de données sur l'empreinte eau
- les hypothèses donnent un intervalle de sécurité large (entre 50% et 185% de l'impact annoncé )

## Pour aller plus loin

- {% include link.html link="https://infos.ademe.fr/magazine-janvier-2025/numerique-quel-impact-environnemental-en-2022/" text="Résumé de l'étude" %} par l'ADEME
- {% include link.html link="https://librairie.ademe.fr/ged/9522/Evaluation-impact-numerique-ADEME-Arcep-2025.pdf" text="Rapport complet" %} par l'ADEME
