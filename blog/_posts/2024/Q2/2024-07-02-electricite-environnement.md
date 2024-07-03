---
title: "L'impact environnemental de la production d'électricité"
description: "Comparons l'impact environnemental de la production d'électricité de différents pays"
tags: ["Electricité", "ACV", "Environnement", "Nucléaire", "Eolien", "Hydro", "Fossile"]
image: /assets/img/posts/2024/Q3/electricity.webp
thumb: /assets/img/posts/2024/Q3/electricity
podcast: https://sphinx.acast.com/p/open/s/65e06335dd3dcf001643bd06/e/6685169a04b201dd34273f5f/media.mp3
---

L'électricité, c'est bien pratique dans notre vie... mais dès lors que l'on parle de sa production, il semble qu'aucun moyen de production ne soit satisfaisant.

Voici généralement les reproches que l'on peut entendre

- Les [énergies fossiles](/blog/2024/04/30/epuisement-ressources-fossiles) sont responsables du [dérèglement climatique](/blog/2024/05/21/changement-climatique)
- Le nucléaire produit des déchets dangereux et emet des radiations nocives
- L'éolien est responsable de la mort de nombreux oiseaux et chauve-souris et cela pollue l'espace visuel.
- Le solaire est produit à partir de panneaux photovoltaïques chinois

Et j'en passe !

Je vous propose cet article pour s'y retrouver un peu. L'objectif ici est de donner des ordres de grandeurs quantitatifs sur les impacts environnementaux. On ne traitera donc pas des aspects financiers, esthétiques ou du confort sonore.

Je ne m'intéresse pas non plus ici aux contraintes techniques, notamment au fait qu'il faut que la production soit toujours égale à la consommation d'électricité. Il s'agit pourtant d'une prouesse réalisée par les gestionnaires de réseaux (RTE en France) qui oblige parfois à prendre des décisions contre-intuitives.

## France vs Allemagne

Pour commencer, je vous propose de comparer les stratégies mises en place par deux pays assez similaires (population équivalente, ressources naturelles similaires, PIB proches) : la France et l'Allemagne.

### Le mix électrique

La France a beaucoup développé sa filière nucléaire pour produire son électricité. L’Allemagne a décidé d'abandonner le nucléaire pour développer les énergies renouvelables (éolien, solaire, biomasse) et produit le reste en priorité avec le [charbon qu'ils extraient localement](/blog/2023/12/12/demesure-des-besoins-humains)

{% responsive_image 
  path: assets/img/posts/2024/Q3/france-allemagne-mix-elec.webp 
  alt: "Le mix électrique de la France et de l’Allemagne : beaucoup de nucléaire en France, et une part important pour l'éolien et le charbon en Allemagne." 
%}
*Le mix électrique de la France et de l’Allemagne (source : {% include link.html text="Electricitymaps" link="https://app.electricitymaps.com/map" %})*

### Moins d'énergies fossiles, moins d'émissions de gaz à effet de serre

On constate que la France utilise bien moins d'énergies fossiles. Du coup, ce n'est pas une surprise quand on regarde l'impact sur le climat d'1 kWh d'électricité, la France est bien en dessous de l'Allemagne.

| Pays      | CO<sub>2</sub>eq par kWh d'électricité produite |
|-----------|-------------------------------------------------|
| France    | 80 g                                          |
| Allemagne | 650 g                                           |

*Impact climatique de l'électricité allemande et française (source {% include link.html link="https://base-empreinte.ademe.fr/donnees/jeu-donnees" text="Base empreinte" %} de l'ADEME)*

### La contrepartie du nucléaire

En effet, cependant le nucléaire émet des {% include link.html text="radiations ionisantes" link="https://www.who.int/fr/news-room/fact-sheets/detail/ionizing-radiation-and-health-effects" %} qui peuvent avoir des effets néfastes sur la santé.

| Pays      | Radiations ionisantes par kWh d'électricité produite |
|-----------|------------------------------------------------------|
| France    | 3 230 Bq U<sub>235</sub>eq                           |
| Allemagne | 958 Bq U<sub>235</sub>eq                             |

*Impact ionisant de l'électricité allemande et française (source {% include link.html link="https://base-empreinte.ademe.fr/donnees/jeu-donnees" text="Base empreinte" %} de l'ADEME)*

### Comment comparer ?

Nous voilà bien embêtés... On pourrait s'arrêter là et conclure : "Les stratégies de l'Allemagne et de la France comportent des avantages et des inconvénients".

On ne peut pas comparer des becquerels et des grammes... Mais il existe des limites planétaires pour ces deux impacts environnementaux. C'est le JRC (Joint Research Centre) de la Commission Européenne qui les propose. 

| Critère environnemental | Limite plantéaire              | Limite par habitant          | 
|-------------------------|--------------------------------|------------------------------|
| Changement climatique   | 6,81E+12 g CO<sub>2</sub>eq    | 973 kg CO<sub>2</sub>eq      |
| Radiations ionisantes   | 5,27E+14 kBq U<sub>235</sub>eq | 75 300 kBq U<sub>235</sub>eq |

*Les {% include link.html text="limites planétaires" link="https://www.sciencedirect.com/science/article/pii/S0301479720306186#tbl3" %} proposées par le JRC*

On a envie de faire une simple division

*<math><mfrac><msup>Impact d'un kWh</msup><mn>Limite planétaire de cet impact</mn></mfrac></math>*

Cela permettra de savoir à quel point chaque kWh participe aux impacts environnementaux et en particulier à leurs limites planétaires. Mais je trouve qu'un kWh n'est pas très parlant. Je préfère donc multiplier le tout par l'{% include link.html text="électricité consommée par personne en France" link="https://www.data.gouv.fr/fr/reuses/consommation-par-habitant-et-par-ville-delectricite-en-france/" %} :

*<math><mfrac><msup>(Energie consommée par personne en France en kWh) * (Impact d'un kWh)</msup><mn>Limite planétaire de cet impact</mn></mfrac></math>*

Nous allons appeler le résultat le PBPC (Planet Boundary per Capita). L'idée, c'est que cela permet de ramener tous les indicateurs environnementaux (pour le moment on en a parlé de deux, mais on va pouvoir élargir ensuite) à la limite planétaire.

| Pays      | PBPC - Changement Climatique | PBPC - Radiation ionnisantes | 
|-----------|------------------------------|------------------------------|
| France    | 18.30 %                      | 9.54 %                       |
| Allemagne | 148.53%                      | 2.83 %                       |

*Comparaison de deux critères environnementaux pour la production d'électricité par rapport à la limite planétaire*

Ainsi la consommation d'électricité d'un.e Français.e moyen.ne contribue à 18.3 % de la limite planétaire pour les émissions de gaz à effet de serre. Si nous avions adopté la stratégie allemande on dépasserait la limite planétaire. Il faut bien garder en tête qu'il ne s'agit là uniquement de la production d'électricité. A cela, il faut également ajouter les autres secteurs (transport, alimentation...)

Ainsi, on se rend compte que les radiations ionisantes produites par l'électricité française sont plus acceptables que la participation aux émissions de gaz à effet de serre de l'électricité allemande.

### Et les autres indicateurs environnementaux ?

On l'a vu, il [existe beaucoup de crises environnementales](/blog/2024/01/16/crises-environnementales). Dans les Analyses du Cycle de Vie, nous en suivons 16.

La {% include link.html link="https://base-empreinte.ademe.fr/donnees/jeu-donnees" text="Base empreinte" %} de l'ADEME permet de suivre 9 de ces 16 indicateurs :

| Impact environnemental | France | Allemagne |
|---|---|---|
| [Changement climatique](blog/2024/05/21/changement-climatique) | 18,30 % | 148,53 % |
| [Acidification](blog/2024/03/05/acidification) | 0,33 % | 2,74 % |
| [Appauvrissement de la couche d'ozone](blog/2024/06/25/depletion-ozone-stratospherique) | 0,00 % | 0,00 % |
| [Eutrophisation eaux douces](blog/2024/01/17/eutrophisation) | 0,01 % | 0,01 % |
| [Eutrophisation marine](blog/2024/01/17/eutrophisation) | 0,59 % | 2,05 % |
| [Eutrophisation terrestre](blog/2024/01/17/eutrophisation)	| 0,13 % | 0,50 % |
| Formation d'ozone photochimique	| 0,81 % | 2,88 % |
| Particules	| 12,45 % | 31,06 % |
| Radiations ionisantes	| 9,54 % | 2,83 % |
| [Utilisation de ressources fossiles](blog/2024/04/30/epuisement-ressources-fossiles)	| 64,68 % | 60,79 % |
| [Utilisation de ressources minérales et métalliques](blog/2024/05/27/utilisation-des-metaux) | 0,35 % | 0,62 % |

*Participation aux limites planétaires pour l'équivalent de la consommation d'un habitant en France pour les différents impacts environnementaux (source {% include link.html link="https://base-empreinte.ademe.fr/donnees/jeu-donnees" text="Base empreinte" %} de l'ADEME)*

On peut constater par exemple, que l'Allemagne a besoin de presque deux fois plus de métaux pour son parc électrique que la France (je suppose que cela est dû à la fabrication des éoliennes). Mais qu'il s'agit d'un non sujet puisque cette consommation reste très basse et acceptable (= je suis prêt à mettre 1% de mon budget métaux dans la production d'électricité).

Une autre remarque importante, même si l'électricité française est décarbonée (seulement 6% d'énergies fossiles), nous avons encore besoin de beaucoup de ressources fossiles (plus même que l'Allemagne !). Cela peut s'expliquer par le fait que les ressources fossiles sont nécessaires pour l'extraction et le transport de l'uranium par exemple ou encore pour la fabrication des différentes centrales.

Là, vous vous demandez sûrement comment il est possible qu'il y ait une telle différence entre les émissions de gaz a effet de serre (rapport fois huit) alors que l'utilisation en ressources fossiles est environ égale. Cela peut s'expliquer par :
- l'usage de ressources fossiles en tant que matière première (et donc peu de participation au changement climatique)
- l'usage de différents combustibles fossiles. Typiquement, le gaz naturel émet moins de gaz à effet de serre que le charbon pour une production énergétique équivalente.
- le fait qu’il peut y avoir d’autres émissions de gaz à effet de serre que par la combustion d’énergie fossile (comme la déforestation par exemple, ou encore les émissions de méthane d’une zone inondée suite à la construction d’un barrage) 

### Vers un indicateur unique ?

Si on estime que toutes les catégories d'impacts environnementaux sont d'égales importances, il est possible de sommer ces impacts pour avoir un indicateur unique. Cette somme n'a plus trop de sens physique et l'hypothèse est fortement contestable. Mais cela permet de se faire une idée rapide de ce qui a l'impact environnemental le plus fort ou le plus faible. 

On verra que c'est presque indispensable si on veut comparer de nombreux pays.

{% responsive_image 
  path: assets/img/posts/2024/Q3/france-allemagne-impacts-elec.webp 
  alt: "Comparaison des impacts environnementaux de la production d'électricité en Allemagne et en France." 
%}

## Et les autres pays ?

Voilà maintenant que la méthodolgie est présentée, on peut tenter l’impossible et tenter de comparer l’impact environnemental de la production d’électricité de 12 pays. La Base Empreinte en propose beaucoup plus mais je me suis dit qu’il valait mieux sélectionner.

Mon choix s'est porté sur les pays qui avaient les données les plus robustes, qui étaient proches de la France et dont les stratégies de production d'électricité étaient différentes.

{% responsive_image 
  path: assets/img/posts/2024/Q3/12pays-impacts-elec.webp 
  alt: "Comparaison des impacts environnementaux de la production d'électricité de 12 pays." 
%}
*Comparaison des impacts environnementaux de la production d'électricité de 12 pays (source {% include link.html link="https://base-empreinte.ademe.fr/donnees/jeu-donnees" text="Base empreinte" %} de l'ADEME)*

Un petit coup d’œil suffit pour se rendre compte que l'Islande et la Norvège se démarquent avec une électricité avec très peu d'impacts environnementaux. A l'inverse, l'électricité polonaise semble la plus mauvaise pour l'environnement.

Essayons de comprendre ce qui se passe, en consultant par quels moyens ces pays produisent leur électricité.

{% responsive_image 
  path: assets/img/posts/2024/Q3/12pays-mix-elec.webp 
  alt: "Comparaison des mix de production d'électricité de 12 pays." 
%}

*Mix électriques des douze pays (source : {% include link.html text="Electricitymaps" link="https://app.electricitymaps.com/map" %})*

### Les bons élèves : la Norvège et l'Islande

Quand on regarde l'origine de leur production électrique, on se rend compte que ces deux pays se basent en grande part sur l'hydro-électricité. On peut clairement affirmer qu'il s'agit d'une stratégie de production qui préserve au mieux l'environnement, mais tous les pays ne possèdent pas la géographie permettant d'arriver à ce niveau (typiquement, en France, il me semble que nous exploitons l'hydro-électricité au maximum de ce que nous pouvons).

On notera également que ces deux pays ont complété leur production avec d'autres modes de productions renouvelables (géothermie pour l'Islande et éolien pour la Norvège).

### France, Belgique et Suisse : au dessus-de la moyenne

Le point commun de ses trois pays est d'avoir réussi à remplacer une grande partie de leur production électrique basée sur des ressources fossiles par le nucléaire.

Le problème des ressources fossiles, c'est que [leur épuisement](blog/2024/04/30/epuisement-ressources-fossiles) constitue une catégorie d'impact à part entière, qu'elles [impactent aussi fortement le climat](blog/2024/05/21/changement-climatique), mais elles ont également un rôle important sur les émissions de particules ainsi qu'un rôle non négligeable sur l'[acidification](blog/2024/03/05/acidification).

Malgré leur utilisation du nucléaire, la Grande-Bretagne et les États-Unis ne sont pas mieux que les autres puisqu’ils utilisent encore largement les énergies fossiles.

### Dernier de classe : la Pologne

Avec une électricité produite pour près de deux tiers avec du charbon (la pire des énergies fossiles), la Pologne possède l'électricité la plus nocive pour la planète du groupe testé.

## Pour finir

### Limites

Comme évoqué en introduction, seuls les critères environnementaux ont été pris en compte. Il existe des contraintes physiques, techniques, financières et sociales qui n'ont pas été évaluées.

Seuls 9 des 16 critères environnementaux ont été évalués. Il manque à minima l'utilisation de l'eau ainsi que le changement des sols afin de pouvoir être assertif sur les résultats.

### Conclusion

L'enseignement général derrière cette étude, c'est que les énergies fossiles sont tellement nocives pour la planète qu'elles viennent complètement masquer les différences qui peuvent exister entre les différents moyens de production d'électricité alternatifs.

Le débat n’est aujourd’hui pas de savoir quelles filières il faut développer. Tout ce qui peut réduire la part du charbon, du pétrole et du gaz est bon à prendre.