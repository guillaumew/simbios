---
title: "La matérialité de l'infrastructure réseau mondiale"
description: "Appuyons-nous sur le rapport GreenIT.fr pour déterminer ce qui pèse le plus sur l'environnement dans l'infrastructure réseau."
tags: ["Réseau", "Fixe", "Mobile", "Green IT", "ACV", "Environnement", "Monde"]
image: /assets/img/posts/2025/Q1/thumb-4G-antenna.jpg
thumb: /assets/img/posts/2025/Q1/thumb-4G-antenna
alt-image: "Une antenne réseau mobile"
podcast: https://sphinx.acast.com/p/open/s/65e06335dd3dcf001643bd06/e/67dbe73813f133b29da5e466/media.mp3
---

Le rapport GreenIT.fr sur [les impacts environnementaux du numérique dans le monde](/blog/2025/02/06/impacts-numerique-monde) propose un volet sur les impacts environnementaux de l'infrastructure réseau. Ce dernier repose en grande partie sur l'étude de l'ADEME {% include link.html link="https://librairie.ademe.fr/industrie-et-production-durable/6789-evaluation-de-l-empreinte-environnementale-de-la-fourniture-d-acces-a-internet-en-france.html" text="Evaluation de l'empreinte environnementale de la fourniture d'accès à internet en France" %} parue en mars 2024.

Je vais m'appuyer sur ces deux rapports pour écrire cet article. Nous aurons ainsi une approche France et Monde.

## L'infrastructure réseau, c'est quoi au juste ?

Quand vous naviguez sur internet, vous accédez généralement à des fichiers ou des données qui n'existent pas sur votre terminal. Votre appareil doit aller télécharger ces derniers sur des serveurs (dans le cas le plus courant). Pour que cela soit possible, il faut créer un pont qui relie le serveur et le terminal. C'est exactement le rôle de l'infrastructure réseau.

Pour cela, on peut soit utiliser un réseau fixe, soit un réseau mobile ou encore un satellitaire (comme StarLink). Ce dernier est de loin le moins utilisé et réservé à des usages particuliers. Il n'a pas été inclus dans les études mentionnées.

De manière générale, la partie la plus importante du réseau est filaire. La seule portion sans fil se résume à la partie entre le terminal et le premier relais de la partie réseau. Ce premier relais sera une antenne 3G-4G-5G pour un réseau mobile ou une box internet pour un réseau fixe.

Tout le reste se fait avec un réseau filaire. Si vous envoyez un mail à un ami aux États-Unis, le message va traverser l'Atlantique dans un câble sous-marin (et non via un satellite comme beaucoup semblent le penser.)

Le premier relais va ensuite être connecté au cœur du réseau (ou backbone) qui va lui-même être connecté aux sites d'hébergement (comme les datacenters).

## Les impacts environnementaux concentrés sur les premiers relais

En France, le réseau fixe constitue l'essentiel des impacts environnementaux du réseau internet français (entre 65 % et 80 % en fonction des indicateurs). Maintenant, pour chacun des modes de connexion (fixe et mobile), regardons comment se répartissent les impacts environnementaux en fonction de la catégorie suivant les critères :
- ADPe : [Utilisation de ressources minéraux et métaux](/blog/2024/05/27/utilisation-des-metaux)
- AP : [Acidification](/blog/2024/03/05/acidification)
- GWP : [Réchauffement climatique](/blog/2024/05/21/changement-climatique)
- IR : [Radiations ionisantes](/blog/2024/12/09/radiations-ionisantes)
- PM : [Émissions de particules](/blog/2024/07/15/particules)
- TPE : Consommation d'énergie primaire (sur l'ensemble des étapes du cycle de vie, y compris énergies renouvelables)

{% responsive_image 
  path: "assets/img/posts/2025/Q1/impacts-reseaufixe-france.webp"
  alt: "Graphique présentant la répartition des impacts environnementaux du réseau internet fixe en France."
  default_type: "png"
%}
*Répartition des impacts du réseau fixe français par catégorie d'équipement, source {% include link.html link="https://librairie.ademe.fr/industrie-et-production-durable/6789-evaluation-de-l-empreinte-environnementale-de-la-fourniture-d-acces-a-internet-en-france.html" text="ADEME" %} (p. 51)*

{% responsive_image 
  path: "assets/img/posts/2025/Q1/impacts-reseaumobile-france.webp"
  alt: "Graphique présentant la répartition des impacts environnementaux du réseau internet mobile en France."
  default_type: "png"
%}
*Répartition des impacts du réseau mobile français par catégorie d'équipement, source {% include link.html link="https://librairie.ademe.fr/industrie-et-production-durable/6789-evaluation-de-l-empreinte-environnementale-de-la-fourniture-d-acces-a-internet-en-france.html" text="ADEME" %} (p. 52)*

Dans les deux cas, on voit que 82% à 94% des impacts sont dus au premier relais (accès opérateur pour le réseau fixe et réseau d'accès radio pour le réseau mobile). La part du cœur de réseau (backbone) et sa connexion avec les serveurs comptent pour une part minime des impacts.

## La réelle différence entre le réseau fixe et le réseau mobile

Lorsque l'on s'intéresse aux étapes du cycle de vie nécessaires pour le fonctionnement de l'infrastructure réseau. On note une différence importante entre le réseau mobile et le réseau fixe.

| Etape du cycle de vie | Réseau Fixe | Réseau mobile |
|-----------------------|-------------|---------------|
| Fabrication           | 72.1 %      | 22.4 %        |
| Distribution          | 0.4 %       | 0.4 %         |
| Installation          | 2.9 %       | 17.2 %        |
| Utilisation           | 21.4 %      | 43.8 %        |
| Maintenance           | 2.7 %       | 16.0 %        |
| Recontionnement       | 0.3 %       | 0.0 %         |
| Fin de vie            | 0.2 %       | 0.3 %         |

*Tableau des contributions des différentes étapes du cycle de vie à l'empreinte carbone du réseau français, source {% include link.html link="https://librairie.ademe.fr/industrie-et-production-durable/6789-evaluation-de-l-empreinte-environnementale-de-la-fourniture-d-acces-a-internet-en-france.html" text="ADEME" %} (p. 82-83)*

On peut voir que les étapes de fabrication (fabrication, distribution et installation) sont largement majoritaires pour le réseau fixe alors que pour le réseau mobile, la partie utilisation (utilisation + maintenance) est majoritaire.

## Modélisation par abonné.e et par quantité de données

La méthode propose une composition des impacts environnementaux par abonnement et par quantité de données consommées. Ainsi, nous avons une partie fixe avec le nombre d'abonnements et une partie variable avec la quantité de données consommées.

Ainsi en France, un abonnement possède un coût environnemental annuel. Pour le réchauffement climatique :
- 50,1 kg CO<sub>2</sub> eq pour un abonnement fixe
- 5,7 kg CO<sub>2</sub> eq pour un abonnement mobile

On voit ainsi que la mutualisation des infrastructures (antennes 3G-4G-5G) permet au réseau mobile d'avoir une empreinte carbone plus faible par abonnement que les box et leur raccordement au cœur du réseau des abonnements fixes.

Mais il existe également une composante variable pour chaque abonnement en fonction de la quantité de données consommées :
- 1,75 g CO<sub>2</sub> eq pour 1 Go consommé via une connexion fixe
- 12,3 g CO<sub>2</sub> eq pour 1 Go consommé via une connexion mobile

Comme l'abonné fixe moyen consomme 2 290 Go et l'abonné mobile moyen 141 Go, cela donne un total de :
- 54,1 kg CO<sub>2</sub> eq pour un abonnement fixe moyen
- 7,5 kg CO<sub>2</sub> eq pour un abonnement mobile moyen

> Chose étonnante, il semble donc qu'il soit intéressant d'un point de vue environnemental de délaisser totalement notre réseau fixe pour tout faire fonctionner sur le réseau mobile.
{: .prompt-tip }

En effet, un abonnement mobile avec une consommation fixe (2 290 Go) possède une empreinte carbone de 33,9 kg CO<sub>2</sub> eq ce qui est moins que l'abonnement fixe moyen.

Cependant, les auteurs de l'étude avertissent que la part abonnement du réseau fixe peut être gonflée par des travaux de sur-dimensionnement du réseau pour anticiper les futurs abonnements et usages.

## Dans le monde

### Par abonnement

Pour le moment, nous nous sommes concentrés sur le rapport de l'ADEME sur le réseau français. Les autrices et auteurs du rapport GreenIT.fr sur les impacts mondiaux se sont basés sur ce rapport mais en extrapolant les résultats, notamment pour s'adapter au mix électrique mondial.

Ainsi pour l'empreinte carbone du réseau à l'échelle mondiale :

| | Réseau Fixe | Réseau mobile |
|---|---|---|
| Empreinte carbone fixe d'un abonnement (en kg CO<sub>2</sub> eq) | 94,3 | 18,4 |
| Impact par Go consommé (en g CO<sub>2</sub> eq ) | 5,6 | 87,8 |
| Données moyennes consommées par abonnement (en Go) | 3 002 | 214 |
| Empreinte moyenne d'un abonnement (en kg CO<sub>2</sub> eq) | 111 | 34 |

Sans surprise le mix électrique français permet d'avoir un impact moindre. Par contre, je suis étonné de voir la moyenne mondiale de données consommée supérieure à la moyenne française.

Ce poids plus lourd de l'utilisation et donc du Go consommé vient changer la donne par rapport à la France. Par exemple, un abonnement mobile avec une consommation identique à la consommation fixe aurait un impact supérieur à un abonnement fixe (282 kg CO<sub>2</sub> eq).

### Au total

Au total dans le monde, le réseau a une empreinte carbone  de 428 millions de tonnes de CO<sub>2</sub> eq dont 39 % sont issus du réseau fixe et 61 % du réseau mobile (tendance inversée par rapport à la France)

Cela constitue :
- 23 % de l'impact du numérique mondial
- 6,3 % de la limite planétaire

Par contre, le réseau possède un impact plus limité sur les ressources minérales et métaux :
- 15 % de l'impact du numérique mondial
- 2,9 % de la limite planétaire

## Les bons réflexes

### Choix de la box internet

On constate que l’essentiel de l'impact environnemental du réseau fixe se situe au nombre de raccordements. Il convient donc de questionner l'intérêt de relier son logement au réseau. Dans beaucoup de cas, il semble qu'une box 4G-5G soit plus intéressante d'un point de vue environnemental.

L'ensemble des opérateurs proposent ce service avec un débit pouvant dépasser 1 Gb/s (la fibre varie en 0.6 et 8 Gb/s). Un abonnement box 5G coûte entre 40€ et 50€ / mois ce qui est un peu plus cher qu'un abonnement fibre classique.

Attention, la box 5G n'a de sens que si votre logement n'est pas encore raccordé au cœur du réseau !

### Privilégier le réseau fixe 

Ensuite, il convient d'avoir les bons réflexes pour limiter sa consommation de données mobiles. Lorsque vous avez le choix, il est important de passer par un réseau fixe (qui inclut le Wifi). La consommation d'un Go via une connexion fixe a une empreinte carbone 7 fois inférieure par rapport à une connexion mobile. Tous les téléchargements qui peuvent être faits de manière asynchrone doivent passer par le réseau fixe :
- Mises à jour d'applications
- Sauvegardes
- Téléchargements de vidéo (avant un trajet en train par exemple)

En parlant de train, lorsque vous êtes dans le train, même si vous vous connectez au réseau wifi proposé, vous êtes bien sur un réseau mobile (un peu comme avec une box 5G)

### Questionner ses usages

Enfin, il y a aussi la possibilité de remettre en question ses usages. En transport, un bon livre permet de s'évader avec un impact environnemental limité. 

Quitte à passer à la médiathèque pour choisir votre livre, vous y trouverez probablement une belle offre de films en DVD (qui ne nécessitent pas de réseau internet pour fonctionner).