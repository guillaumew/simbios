---
title: "Les terminaux numériques dans le monde"
description: "Quels sont les impacts des outils numériques que nous utilisons ?"
tags: ["Terminaux", "Ordinateurs", "Smartphones", "Green IT", "ACV", "Environnement", "Monde"]
image: /assets/img/posts/2025/Q2/thumb-terminaux.jpg
thumb: /assets/img/posts/2025/Q2/thumb-terminaux
alt-image: "Quelques exemples d'objets connectés"
podcast: https://sphinx.acast.com/p/open/s/65e06335dd3dcf001643bd06/e/67f3ccf6e8676925926c3478/media.mp3
data1:
  - name: "Emissions de gaz à effet de serre "
    data:  [54]
  - name: "Utilisation de métaux et minéraux"
    data: [72]
  - name: "Utilisation de ressources énergétiques"
    data: [53]
  - name: "Emissions de particules"
    data: [52]
datalabels1: ["Part des terminaux dans les impacts du numérique"]
data2:
  - name: "Ordinateurs fixes"
    data: [ 05.8]
  - name: "Ordinateurs portables"
    data: [05.8]
  - name: "Tablettes"
    data: [01.9]
  - name: "Téléphones fixes"
    data: [01.9]  
  - name: "Smartphones"
    data: [09.6]
  - name: "Moniteurs"
    data: [01.9] 
  - name: "Téléviseurs"
    data: [25]
  - name: "Imprimantes"
    data: [07.7]
  - name: "Consoles de jeu"
    data: [01.9]  
  - name: "Vidéoprojecteurs"
    data: [09.6]
  - name: "Box TV"
    data: [05.8]
  - name: "Enceintes connectées"
    data: [01.9] 
  - name: "Objets connectés"
    data: [21.3] 
datalabels2: ["Part de l'empreinte carbone des terminaux"]
data3:
  - name: "Empreinte carbone"
    data: [27.8, 1.4, 70.4, 0.5]
  - name: "Utilisation de métaux"
    data: [86.1, 0.7, 12.5, 0.7]
datalabels3: ["Fabrication","Transport","Utilisation","Fin de vie"]
---

Comment sommes-nous équipés pour le numérique ? Et quels sont les impacts environnementaux de ces équipements ? Nous allons nous baser sur le rapport GreenIT.fr sur [les impacts environnementaux du numérique dans le monde](/blog/2025/02/06/impacts-numerique-monde) pour répondre à ces questions.

Les équipements utilisateurs génèrent la majorité des impacts environnementaux liés aux activités numériques. Le reste provient des serveurs et du réseau. Les impacts environnementaux des équipements ont lieu soit lors de leur fabrication, soit à cause de l'électricité qu'ils consomment. Le reste des étapes du cycle de vie étant relativement anecdotique.

{% include bar_chart.html 
  id="chart1" 
  data=page.data1
  data-labels=page.datalabels1
  max-size=72
  label-label="Impact"
  data-suffixe="%"
  padding-bottom="40px"
  type="column multiple stacked"
  show-data = "show-data"
  spacing = true
%}

## Equipements considérés

### Inventaire des équipements dans le monde

Voici l'ensemble des équipements utilisés ainsi que les données clés d'utilisation.

| Equipement   | Unités dans le monde (en millions) | Durée d'utilisation quotidienne | Consommation électrique par équipement et par an | Durée de vie moyenne |
|-----------------------|--------|--------------|-------------|--------|
| Smartphones           | 4 600  | 4 h 37 min   | 3.9 kWh     | 3 ans  |
| Feature phones        | 951    |              | 0.6 kWh     | 4 ans  |
| Téléphones fixes      | 1 700  |              | 18 kWh      | 8 ans  |
| Tablettes             | 460    | 3 h 15 min   | 19.4 kWh    | 3 ans  |
| Ordinateurs portables | 1 050  | 3 h 15 min   | 27.6 kWh    | 5 ans  |
| Ordinateurs fixes     | 465    | 3 h 15 min   | 95.8 kWh    | 6 ans  |
| Ecrans                | 907    | 3 h 15 min   | 25 - 50 kWh (en fonction de la taille) | 7 ans  |
| Téléviseurs           | 1 475  | 3 h 20 min   | 179 kWh     | 7 ans  |
| Box TV                | 773    |              | 73 kWh      | 5 ans  |
| Vidéoprojecteurs      | 567    | 30 min à 3 h | 200 kWh     | 5 ans  |
| Imprimantes           | 585    |              | 133 kWh     | 6 ans  |
| Enceintes connectées  | 718    |              | 43.8 kWh    | 5 ans  |
| Consoles de jeu       | 294    | 1 h 2 min    | 5 (portable) - 56  (salon) kWh  | 6.5 ans|
| Objets connectés      | 15 706 |              | 1.3 kWh     |5 - 12 ans |

*Equipements utilisateurs à travers le monde (source GreenIT.fr)*

Cela constitue un total d'un peu plus de 30 milliards d'équipements utilisateurs.

### Taux d'équipement 

Avec plus de 30 milliards d'équipements numériques, en moyenne chaque personne sur Terre possède près de 4 terminaux. En France, en 2020, nous étions plutôt à 10 équipements par personne (selon l'étude Evalutation de l'impact environnemental du numérique en France de l'ADEME).

> 4 terminaux par personne dans le monde. En France, nous en sommes à 10.
{: .prompt-info }

| Equipements | Unité par personne dans le monde | Unité par personne en France | Part des équipements professionnels en France |
|-------------|----------------------------------|------------------------------|------------------------------------|
| Smartphones           | 0,58                                  | 1,0                                | 14 %               |
| Feature phones        | 0,12                                  | 0,2                                | 14 %               |
| Téléphones fixes      | 0,21                                  | 0,6                                | 30 %               |
| Tablettes             | 0,06                                  | 0,5                                | 31 %               |
| Ordinateurs portables | 0,13                                  | 0,9                                | 45 %               |
| Ordinateurs fixes     | 0,06                                  | 0,6                                | 53 %               |
| Ecrans                | 0,11                                  | 0,7                                | 58 %               |
| Téléviseurs           | 0,18                                  | 0,9                                | 30 %               |
| Box TV                | 0,10                                  | 0,4                                | 30 %               |
| Imprimantes           | 0,07                                  | 0,3                                | 73 %               |
| Enceintes connectées  | 0,09                                  | 0,04                               | 0 %                |
| Consoles de jeu       | 0,04                                  | 0,3                                | 0 %                |
| Objets connectés      | 1,96                                  | 3,6                                | 23 %               |
|-----------------------|---------------------------------------|------------------------------------|--------------------|
| **Total**             | 3,78                                  | 10,0                               | 31 %               |

### Quelques précisions

- Un feature phone est un téléphone portable qui n'est pas un smartphone
- On parle de box TV, la box internet est considérée dans la partie réseau
- Les enceintes connectées incluent les assistants vocaux, les enceintes wifi et bluetooth
- Les objets connectés incluent les équipements de sécurité et de domotique, tout comme certains capteurs, mais excluent la RFID.

Faute de données fiables, les équipements suivants ont été exclus :
- Périphériques (souris, claviers, station d'accueil...)
- Montres connectées
- Imprimantes 3D
- Terminaux de paiement
- Distributeurs de billets
- Caméra de sécurité

## Impacts environnementaux 

### Impacts totaux

Les équipements utilisateurs émettent au total 989 millions de tonnes CO<sub>2</sub> eq. Cela constitue 54 % de l'empreinte carbone du numérique soit 14,5 % de la limite planétaire proposée par le JRC.
Ces équipements concomment 29,5 millions de kg Sb eq soit 72% des métaux nécessaires pour faire fonctionner le numérique mondial. Ils consomment ainsi 13,5 % du budget métaux proposé par le JRC. 

### Par catégorie d'équipement

Voici l'empreinte carbone des différents équipements utilisateurs. Cette empreinte carbone inclut la fabrication et l'utilisation du terminal, mais exclut la sollicitation du réseau et des centres de données.

{% include bar_chart.html 
  id="chart2" 
  data=page.data2
  data-labels=page.datalabels2
  max-size=30
  label-label="Impact"
  data-suffixe=" %"
  type="column"
  padding-bottom="125px"
  show-data = "hide-data"
%}

On constate que les téléviseurs et les objets connectés ont le plus grand impact. Pour les objets connectés, cela est dû à leur nombre. En effet, ils constituent plus de la moitié des équipements utilisateurs. Pour les téléviseurs, c'est leur impact individuel qui est important (grosse consommation et coût de fabrication important).

Viennent ensuite les smartphones (notamment à cause de leur faible durée de vie) et les vidéoprojecteurs qui ont un impact individuel proche des téléviseurs mais qui sont moins nombreux.

### Fabrication vs utilisation

A l'échelle mondiale, l'essentiel des impacts environnementaux se déroule au niveau de l'utilisation. Cela étant dû à une électricité mondiale qui dépend encore largement des énergies fossiles (61% d'après le rapport {% include link.html text="Global Electricity Review" link="https://www.connaissancedesenergies.org/sites/connaissancedesenergies.org/files/pdf-actualites/Global%20Electricity%20Review%202023.pdf" %} d'Ember).

En revanche, la fabrication nécessite énormément de métaux ce qui constitue également un impact environnemental majeur.

*Répartition des impacts environnementaux des terminaux numériques dans le monde en fonction de l'étape du cycle de vie*
{% include bar_chart.html 
  id="chart3" 
  data=page.data3
  data-labels=page.datalabels3
  max-size=110
  label-label="Impact"
  data-suffixe=" %"
  type="column multiple stacked"
  show-data = "show-data"
  spacing = true
  padding-bottom="10px"
%}

## Conclusion

Les équipements utilisateurs sont la principale cause d'impacts environnementaux. Cela est dû principalement à leur nombre dépassant les 30 milliards de terminaux ainsi qu'à leur faible durée de vie.

> Pour limiter leurs impacts, il est nécessaire de ne pas se suréquiper et de faire notre possible pour allonger leur durée de vie au maximum.
{: .prompt-tip }