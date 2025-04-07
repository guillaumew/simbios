---
title: "Les impacts environnementaux du numérique dans le monde"
description: "GreenIT.fr a mis à jour les données sur l'impact du numérique dans le monde."
tags: ["Green IT", "ACV", "Environnement", "Monde"]
image: /assets/img/posts/2025/Q1/thumb-greenit-acv-monde-2025.jpg
thumb: /assets/img/posts/2025/Q1/thumb-greenit-acv-monde-2025
alt-image: "Un centre de données regroupant l'ensemble des symboles de la France."
podcast: https://sphinx.acast.com/p/open/s/65e06335dd3dcf001643bd06/e/67b841fb86a56284d053d209/media.mp3
---

Jusqu'à présent l'ensemble des acteurs du numérique responsable se basaient sur des études monde qui se concerant l'année 2019. Une mise à jour des données sur l'impact environnemental du numérique à l'échelle mondiale était vivement attendue. GreenIT.fr vient combler ce manque avec une {% include link.html text="analyse du cycle de vie de l'ensemble des activités numériques mondiales" link="https://greenit.eco/nos-etudes-et-essais/impacts-environnementaux-du-numerique-dans-le-monde-2025/" %}.

On peut dire que ce rapport est bien fourni ! L'étude propose vraiment beaucoup d'informations. Je vais faire une présentation générale des résultats dans cet article et je proposerai des approfondissements dans des articles séparés.

Voici les approfondissements prévus ou publiés :
- [Impacts de l'intelligence artificielle](/blog/2025/03/04/impacts-intelligence-artificielle)
- [Modélisation du réseau](/blog/2025/03/14/impacts-infrastructure-reseau)
- [Les équipements utilisateurs](/blog/2025/04/07/terminaux-numeriques-monde)

> Comme l'expliquent les auteurs et autrices de ce rapport, la méthodologie a beaucoup évolué en 5 ans et donc il est dangereux de comparer l'étude sur l'année 2019 et celle de 2023 pour établir une évolution. Nous allons ici faire des comparaisons entre les deux études pour voir **ce qui change au niveau de l'état de l'art des connaissances sur les impacts environnementaux du numérique**.
{: .prompt-info }

## Les impacts globaux

### Émissions de gaz à effet de serre

En 2023, le numérique a été responsable de l'émission de 1 832 milliards de kg CO<sub>2</sub>eq. Cela représente donc 3,4% des émissions mondiales. On reste là sur la même tendance que les données de 2019.

Cela ne veut pas dire que le numérique n'a pas alourdi son impact sur le climat (d'ailleurs pour 2019, il était annoncé 1 400 milliards de kg CO<sub>2</sub>eq), ni même que le numérique a suivi une évolution similaire à celle des autres secteurs. La réalité, c'est que les impacts de 2019 avaient été légèrement sur-évalués.

> **342** kg CO<sub>2</sub>eq, c'est l'empreinte carbone moyenne d'un.e internaute.
{: .prompt-tip }

### Utilisation des métaux et minéraux

Si les émissions de gaz à effet de serre avaient été sur-évaluées, l'utilisation des métaux avait largement été sous-estimée. On passe de 22 millions de kg Sb eq à 41 millions !

> Par internaute, les usages en métaux sont équivalents à **5,9** kg de cuivre par an.
{: .prompt-tip }

### Autres critères

Comme j'ai l'habitude de le faire, nous pouvons comparer les impacts mesurés avec les limites planétaires proposées par le {% include link.html text="JRC (Joint Research Centre)" link="https://www.sciencedirect.com/science/article/pii/S0301479720306186#tbl3" %}.

| Impact environnemental                         | % de la limite planétaire pour le numérique |
|------------------------------------------------|--------|
| [Potentiel de réchauffement climatique](/blog/2024/05/21/changement-climatique)          | 26.9 % |
| [Utilisation des ressources, minéraux et métaux](/blog/2024/05/27/utilisation-des-metaux) | 18.7 % |
| [Émission de particules](/blog/2024/07/10/particules)                         | 15.3 % |
| [Eutrophisation](/blog/2024/01/17/eutrophisation), eau douce                      | 11.6 % |
| [Utilisation des ressources, fossiles](/blog/2024/04/30/epuisement-ressources-fossiles)           | 11.2 % |
| [Écotoxicité, eau douce](/blog/2024/01/30/ecotoxicite-eau)                         |  9.6 % |

*Les activités numériques émettent 26,9% des gaz à effet de serre que la terre peut supporter. Cela laisse peu de marge pour les autres secteurs (alimentation, transport, logement...)*

Les autres indicateurs se situent sous 1,5 % (par ordre décroissant d'importance) :
- [Formation d’ozone photochimique](/blog/2024/07/30/formation-ozone-photochimique)
- [Acidification](/blog/2024/03/05/acidification)
- [Eutrophisation](/blog/2024/01/17/eutrophisation), marine 
- Toxicité humaine, non cancéreuse 
- [Eutrophisation](/blog/2024/01/17/eutrophisation), terrestre
- Toxicité humaine, cancéreuse 
- [Radiations ionisantes](/blog/2024/12/09/radiations-ionisantes)
- [Appauvrissement de la couche d’ozone](/blog/2024/06/25/depletion-ozone-stratospherique)

On notera que la [consommation en eau](/blog/2024/01/22/utilisation-eau) et le [changement d'usage des sols](/blog/2024/09/30/changement-affectaction-sols) n'ont pas pu être inclus. En effet, les données sur ces deux impacts ne sont pas encore suffisamment fiables pour donner une estimation robuste.

## Répartition des impacts par origine

On a l'habitude de former trois catégories de matériels faisant fonctionner le numérique : les terminaux utilisateurs, les centres de données et les infrastructures réseaux. Pour ces trois catégories, on regarde les impacts de leur fabrication, de leur distribution, de leur utilisation et de leur fin de vie.

Les impacts étant largement concentrés dans la fabrication et l'utilisation, distribution et fin de vie ont été regroupées. L'ensemble des impacts est exprimé en pourcentage de la limite planétaire.

{% responsive_image 
  path: "assets/img/posts/2025/Q1/impacts-num-monde-2023.webp"
  alt: "Graphique présentant les impacts du numérique mondial par origine."
  default_type: "png"
%}
*Résumé des impacts environnementaux du numérique mondial (en % de la limite planétaire)*

La répartition terminaux / réseau / datacenters est relativement cohérente avec les études précédentes. Il y a toutefois, une différence très importante sur la répartition entre fabrication (en clair) et utilisation (plus foncé).

Sur ce graphique, cela ne saute pas aux yeux, mais pour l'ensemble des facteurs (sauf l'utilisation des métaux), la grande majorité des impacts se concentre sur l'utilisation. La fabrication a un impact moindre. Cela constitue une différence importante avec l'étude précédente.

Comparons les émissions de gaz à effet de serre des deux études :

{% responsive_image 
  path: "assets/img/posts/2025/Q1/ges-num-monde-2019-2023.webp"
  alt: "Comparaison de l'origine des émissions de GES entre les deux études GreenIT monde"
  default_type: "png"
%}
*Evolution de l'état de l'art des émissions de gza à effet de serre du numérique entre 2019 et 2025*

Sur la partie extérieure du graphique, on voit les données de l'étude 2019, la partie fabrication est responsable de 44 % des émissions. Sur la partie intérieure, on voit les données de l'étude 2025 où la fabrication n'est responsable que de 18 % des émissions. Cette tendance se retrouve sur presque tous les indicateurs.

Cela s'explique par une sur-évaluation qui avait été réalisée en 2019 car les connaissances n'étaient pas aussi structurées qu'elles ne le sont aujourd'hui. D'autre part, il y a aussi une modélisation du réseau qui a changé en cours de route. J'en parlerai dans un article dédié. Enfin, l'émergence de l'intelligence artificielle vient également augmenter la consommation électrique des centres de données et donc leurs impacts dans la phase utilisation.

## Limites de l'étude

Comme toujours, il est impossible de tout prendre en compte parfaitement. Il est à noter que GreenIT.fr a fait un effort considérable de transparence sur la méthodologie utilisée ce qui permet de vraiment savoir quel est le périmètre étudié.

Les quelques limites significatives relevées :

- les données réseau sont issues d'une étude France extrapolée au réseau mondial
- quelques équipements numériques ne sont pas inclus (imprimantes 3D, terminaux de paiement...)
- les satellites ne sont pas inclus dans la partie infrastructure réseau
- dans la phase utilisation, seule la consommation électrique a été prise en compte. La maintenance des appareils n'a pas pu être modélisée (réparation, changement de composant...)
- non prise en compte de la seconde vie des appareils (reconditionnement, recyclage)

Dans tous les cas, c'est l'absence de données fiables qui justifie ces limites. Il semble que ces limites devraient garder un impact relativement faible sur les tendances générales. Par exemple à l'échelle mondiale, les équipements électroniques sont rarement collectés pour recyclage. 

Toutefois, il faut rester prudent avec ces certitudes tant qu'on n'a rien chiffré.

## Conclusions

Ce rapport vient donner un coup de fraîcheur sur les impacts envirionnementaux du numérique. Avec une méthodologie bien formalisée et respectant les principes généraux d'une analyse du cycle de vie, les résultats semblent aussi fiables que l'état de l'art du moment le permet.

L'essentiel des impacts environnementaux se déroulant pendant la phase utilisation, il convient de modérer nos usages. En France, même si nos équipements fonctionnent avec une électricité bas-carbone, lors de notre utilisation il est possible voire probable que nous sollicitions des centres de données et du réseau d'autres pays et dont l'électricité aura des impacts suppérieurs.

Plus que jamais, il faut questionner nos usages pour en maitriser la croissance. Par exemple, en 2023, les serveurs portant l'intelligence artificielle produisent à eux seuls entre 15 % et 20 % des gaz à effet de serre des centres de données.

Pour creuser le sujet, je vous invite à lire le document complet (92 pages) :

<p class="is-center">{% include link.html text="Voir l'étude complète" link="https://greenit.eco/nos-etudes-et-essais/impacts-environnementaux-du-numerique-dans-le-monde-2025/" class="button" %}</p>
