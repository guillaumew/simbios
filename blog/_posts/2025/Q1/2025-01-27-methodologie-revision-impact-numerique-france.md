---
title: "Proposition de révision de l'impact environnemental du numérique"
description: "L'ADEME a jeté un pavé dans la mare avec la révision de son rapport sur les impacts environnementaux du numérique français. Voici ma proposition sur le sujet."
tags: ["ADEME", "ACV", "Datacenter", "France"]
image: /assets/img/posts/2025/Q1/thumb-revision-impact-num-france.jpg
thumb: /assets/img/posts/2025/Q1/thumb-revision-impact-num-france
alt-image: "Un centre de données regroupant l'ensemble des symboles de la France."
podcast: null
hidden: true
---

## Contexte

En 2022, l'ADEME proposait un rapport mesurant l'impact environnemental du numérique. Ce rapport se limite à la consommation électrique des datacenters en France, négligeant le fait que des usages numériques en France sollicitent parfois des datacenters à l'étranger (limitation documentée).

En 2025, l'ADEME s'appuie sur une {% include link.html text="méthologie proposée par Hubblo" link="https://hubblo.org/fr/blog/datacenters-imported-impacts/" %} pour mettre à jour ces chiffres et inclure les usages de datacenters étranger.

## Ratio consommation électrique terminaux vs datacenter

Quand on regarde le ratio entre l'électricité consommée à l'usage par les terminaux et les datacenters, on trouve quelque chose de relativement constant dans différents périmètres :

<table>
  <thead>
    <tr>
      <th>Périmètre</th>
      <th>Ratio</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>{% include link.html link="https://www.greenit.fr/empreinte-environnementale-du-numerique-mondial/" text="Empreinte environnementale du numérique mondial" %}</td>
      <td>50 %</td>
    </tr>
    <tr>
      <td>{% include link.html link="https://www.greenit.fr/le-numerique-en-europe-une-approche-des-impacts-environnementaux-par-lanalyse-du-cycle-de-vie/" text="Le numérique en Europe" %}</td>
      <td>52,4 %</td>
    </tr>
    <tr>
      <td>{% include link.html link="https://www.greenit.fr/impacts-environnementaux-du-numerique-en-france/" text="iNUM : impacts environnementaux du numérique en France" %}</td>
      <td>48,1 %</td>
    </tr>
  </tbody>
</table>

De même, le rapport {% include link.html link="https://www.researchgate.net/publication/275653947_On_Global_Electricity_Usage_of_Communication_Technology_Trends_to_2030" text="On Global Electricity Usage of Communication Technology: Trends to 2030" %} semble montrer un rapport de cet ordre de grandeur pour 2020.

{% responsive_image 
  path: "assets/img/posts/2025/Q1/andrae-edler.webp"
  alt: "Tendances pour la consommation électrique du numérique dans le monde."
%}

Or dans les chiffres de l'ADEME, ce rapport est de 35,1 % dans le rapport initial puis de 74,1 % dans la récente révision.

Les deux rapports de l’ADEME montrent donc un ratio électricité utilisées par les terminaux utilisateur sur électricité utilisée par les centres informatiques assez éloigné du reste de la littérature.

Le premier rapport avait la claire limitation de se contenter de comptabiliser les data centers français, ignorant les usages français sollicitant des data centers étrangers. Mais la correction proposée en 2025 me semble un peu trop sur-estimée.

## Energie utilisée par les datacenters pour les usages français

On va estimer que le ratio d’usage d’énergie des datacenter par rapport aux terminaux est de 50 % (rapport GreenIT, {% include link.html link="https://www.greenit.fr/empreinte-environnementale-du-numerique-mondial/" text="Empreinte environnementale du numérique mondial" %}).

|                                                | Datacenters | Terminaux | Ratio |
|------------------------------------------------|-------------|-----------|-------|
| Données du rapport de l'ADEME 2020 (en %)      | 17.9 %      | 51.0 %    | 35.1 %|
| Données du rapport de l'ADEME 2020 (en Joules) | 14.6 PJ     | 41.7 PJ   | 35.1 %|
| Pour avoir un ratio de 50 %                    | 20.9 PJ     | 41.7 PJ   | 50 %  |

Les datacenters français consomment 14.6 PJ, on estime qu'ils répondent uniquement à des usages français.

Il manque donc 6,3 PJ à la consommation électrique dans le rapport de l'ADEME, si on estime que les datacenters consomment la même énergie à usage électrique des terminaux constant. Il s'agit donc de la consommation des datacenters étrangers sollicités par des usages français.

Pour la suite, nous allons considérer que l’ensemble des impacts environnementaux des datacenters sont proportionnels à l’électricité consommée à l’usage (fabrication, fin de vie…). Hypothèse simpliste, mais qui permet d’avoir des ordres de grandeurs.

L’étude {% include link.html link="https://www.greenit.fr/empreinte-environnementale-du-numerique-mondial/" text="Green IT monde" %} montre que le numérique mondial consomme 6 800 TWh d’énergie primaire soit 24 480 PJ. 15 % de cette énergie va dans l’usage des datacenters soit 3 672 PJ. Les usages numériques français sollicitant des datacenters étranger utilisent donc 0,17 % des datacenters mondiaux.

On peut donc appliquer ce rapport directement dans les impacts environnementaux des datacenters monde de l'étude GreenIT.

| Bilan GES | Fabrication | Utilisation |
| ---|---|---|
| Ensemble des datacenters dans le monde | 14 Mt CO<sub>2</sub>eq | 196 Mt CO<sub>2</sub>eq | 
| Part des datacenters étrangers sollicités par des usages français | 0.024 Mt CO<sub>2</sub>eq | 0.33 Mt CO<sub>2</sub>eq |

## Révision de la répartation de l'impact carbone du numérique en France

| Bilan GES            | Terminaux – Fabrication | Terminaux - Usages | Datacenters - Fabrication | Datacenter - Usages | Réseau - Fabrication | Réseau – Usages |
| -------------------- | ----------------------- | ------------------ | ------------------------- | ---------------------- | ----------------------- | --------------- |
| ADEME original (%)       | 65,50 %                 | 13,20 %            | 11,00 %                   | 4,90 %                 | 2,60 %                  | 2,90 %          |
| ADEME original (Mt CO<sub>2</sub> eq)      | 11,0695                 | 2,2308             | 1,859                     | 0,8281                 | 0,4394                  | 0,4901          |
| Révision             | 11,0695                 | 2,2308             | 1,883                     | 1,1581                 | 0,4394                  | 0,4901          |
| Différence           | 0,00 %                  | 0,00 %             | 1,29 %                    | 39,85 %                | 0,00 %                  | 0,00 %          |
| Pourcentages révisés | 64,09 %                 | 12,92 %            | 10,90 %                   | 6,71 %                 | 2,54 %                  | 2,84 %          |

On peut voir que cette révision a impact fort sur l'usage des datacenters avec une augmentation d'environ 40 % de son impact sur le climat. Toute fois cela ne vient pas chambouler les ordres de grandeurs généraux. L'usage des datacenters passent de 4,9 % à 6,7 % de l'impact climatique général du numérique.

## Conclusion

J'estime que mon estimation est un peu naïve et ne reflète probablement pas la réalité. Elle s'appuie sur de nombreuses hypothèses simplistes. Toutefois, je suis plus confiant dans mon modèle que dans le modèle Masanet utilisé par l'ADEME, pour la bonne raison qu'il reste cohérent avec le reste de la littérature.

L'enseignement à retenir, c'est qu'avec des hypothèses simplificatrices (même sensées), on peut arriver à des résultats radicalement différents. Il est donc hasardeux de s'appuyer sur ce type de raisonnement. Rien ne remplace un inventaire factuel.

[Revenir à l'article principal pour une conclusion plus complète](/blog/2025/01/27/revision-impact-numerique-france#résultats)