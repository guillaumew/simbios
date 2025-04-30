---
title: "Les enjeux éthiques de l'intelligence artificielle"
description: "Prenons un temps de recul et posons-nous les bonnes questions avant de nous ruer vers l'intelligence artificielle."
tags: ["Numérique Responsable", "Intelligence artificielle", "Souveraineté", "Données", "Société", "Environnement"]
image: /assets/img/posts/2025/Q2/thumb-ai-ethics.jpg
thumb: /assets/img/posts/2025/Q2/thumb-ai-ethics
alt-image: "Un rêve de Google DeepMind"
podcast: null
usages_ia:
  - name: "Total Français "
    data:  [39]
  - name: "18-24 ans"
    data: [74]
  - name: "25-34 ans"
    data: [55]
  - name: "35-44 ans"
    data: [39]
  - name: "45-59 ans"
    data: [35]
  - name: "60-75 ans"
    data: [17]
usage_ia_label: ["Taux d'utilisation de l'IA générative"]
---

## Où en est-on sur les usages de l'intelligence artificielle ?

Une {% include link.html text="étude CESI/Ipsos" link="https://www.ipsos.com/fr-fr/intelligence-artificielle-quels-sont-les-usages-des-francais" %} résume très bien les usages de l'intelligence artificielle en France (février 2025).

{% include bar_chart.html 
  id="usage_ia" 
  data=page.usages_ia
  data-labels=page.usage_ia_label
  max-size=75
  label-label="Impact"
  data-suffixe="%"
  padding-bottom="0px"
  type="column multiple stacked"
  show-data = "show-data"
  spacing = true
%}

On constate une variation extrêmement importante entre un usage massif chez les 18-24 ans alors que les 60-75 ans sont très rares à s'intéresser à l'IA générative.

La même étude montre également que ChatGPT reste de loin l'outil le plus populaire (utilisé par 80 % des personnes ayant recours à l'IA). 

Quand la question des risques a été abordée, l'environnement n'a pas semblé être un sujet de préoccupation des répondants...

## Les impacts environnementaux de l'intelligence artificielle

Pourtant, comme tout service, l'intelligence artificielle possède un impact environnemental. Mais l'essentiel se déroule loin des utilisateurs, donnant une illusion d’immatérialité aux utilisateurs.

### Une chaîne complexe avec un coût environnemental conséquent

Lors d'une conversation avec ChatGPT, nous allons solliciter :
- notre terminal dont la fabrication a probablement été réalisée en Asie et qui fonctionne avec une électricité potentiellement produite à quelques centaines de kilomètres de nous
- notre message (ou prompt) va être transporté par un réseau invisible (sous terre, sous l'eau) pour arriver jusqu'aux États-Unis où étaient hébergés les serveurs de ChatGPT en 2024 ({% include link.html link="https://openai.com/index/introducing-data-residency-in-europe/" text="source" %}) consommant à leur tour une électricité invisible
- les datacenters accueillants les serveurs ChatGPT sont loin. Ils ont besoin d'une électricité importante pour fonctionner, qui plus est une électricité américaine produite avec un mix plus carboné. Ces serveurs nécessitent des composants puissants (le GPU) et peu répandus jusqu'à l’avènement de l'intelligence artificielle. Cela force à mettre à jour le parc des serveurs avec un coût environnemental de fabrication extrêmement important.
- il a également fallu réaliser la conception logicielle de ChatGPT avec des phases d’entraînement nécessitant de nombreuses données et beaucoup de calculs énergivores.

### Beaucoup de ressources exploitées

#### Électricité

Dans le monde, 60 % de l'électricité est d'origine fossile ({% include link.html link="https://www.eia.gov/international/data/world/electricity/electricity-generation" text="source" %}). Les énergies fossiles ont des impacts importants sur le climat et les émissions de particules.

D'autre part, en vue de la réduction de notre empreinte carbone, nous avons tendance à électrifier nos usages (chauffage, transport...). Nos moyens de productions électriques parviendront-ils à satisfaire l'ensemble des besoins de l’humanité dans les années à venir ?

#### Eau

Les datacenters consomment beaucoup d'eau pour refroidir les composants électroniques des serveurs. Rien qu'aux États-Unis les datacenters consomment 1,7 milliards de litres d'eau chaque jour ({% include link.html link="https://www.nature.com/articles/s41545-021-00101-w" text="source" %}).

A l'heure actuelle, nous avons encore beaucoup de difficulté à quantifier la consommation en eau de nos usages numériques. Toutefois, l'université de Californie a évalué qu'une requête à ChatGPT consomme en moyenne 17 ml d'eau ({% include link.html text="source" link="https://arxiv.org/pdf/2304.03271" %})

#### Métaux

Les calculs complexes de l'intelligence artificielle nécessitent des composants particuliers (GPU) qui n'étaient pas courant dans les centres de données avant l'intelligence artificielle.

Les serveurs risquent donc d'être rapidement remplacés par des serveurs compatibles avec l'IA avec ces précieux composants, accélérant ainsi l'obsolescence de serveurs actuels.
Pour être fabriqués les équipements numériques nécessitent de métaux très variés présents en quantités limitées sur Terre. Ces derniers ne se renouvellent pas. L'extraction des métaux nécessite une excavation de quantité astronomique de minerais de la croûte terrestre pour obtenir très peu des métaux rares nécessaires pour le numérique (pour l'or : {% include link.html text="quelques grammes par tonne de minerais excavé" link="https://www.universalis.fr/encyclopedie/minerais/3-les-conditions-de-formation-des-gisements-et-leur-localisation/" %})

La séparation du métal du minerai nécessite beaucoup d'eau , de matière chimique et d'énergie. Les déchets toxiques sont généralement laissés dans des lacs artificiels qui peuvent se répandre et contaminer toutes la vie aux alentours.

#### Gaz à effet de serre

Le manque de transparence des acteurs de l'intelligence artificielle rendent difficiles les évaluations de l'empreinte carbone de l'usage de l'IA. 

On soulignera tout de même l'excellent outil {% include link.html text="Ecologits" link="https://huggingface.co/spaces/genai-impact/ecologits-calculator" %} qui évalue les coûts environnementaux (électricité, climat, métaux...) des différents chatbots.

Selon Ecologits, une conversation avec ChatGPT émet 21,4 g CO<sub>2</sub>eq. Cette donnée n'inclut pas les coûts environnementaux du terminal, du réseau ou de l’entraînement du modèle. Il s'agit uniquement de l'impact des serveurs qui traitent la requête.

Un utilisateur qui utilise donc ChatGPT 15 fois par jour 300 jours an frôle les 100 kg CO<sub>2</sub>eq uniquement sur la sollicitation du serveur pour l'IA. Cela constitue 11,3% de la {% include link.html text="limite planétaire" link="https://www.sciencedirect.com/science/article/pii/S0301479720306186#tbl3" %} individuelle, ce qui ne laisse pas beaucoup de budget carbone pour le reste des usages (alimentation, logement, transport...) 

### Une croissance vertigineuse des impacts

Malgré tous leurs efforts, les grands acteurs du Cloud (Google, Amazon et Microsoft) ne parviennent pas à leurs objectifs de réduction d'émission de gaz à effet de serre ({% include link.html link="https://www.carbone4.com/analyse-empreinte-carbone-du-cloud" text="source" %}). Cela est dû à l'augmentation des usages et notamment à l'explosion de l'intelligence artificielle.

Mais l’expansion ne fait que commencer, {% include link.html link="https://www.deloitte.com/fr/fr/our-thinking/explore/climat-developpement-durable/empreinte-environnementale-de-l-ia-aujourd-hui-et-demain.html" text="Deloitte" %} envisage que les centres de données vont consommer 10 fois plus d'électricité en 2050 qu'en 2023 pour satisfaire les besoins de l'intelligence artificielle.

{% responsive_image 
  path: assets/img/posts/2025/Q2/consommation-d-energie-dans-nos-differents-scenarios.webp 
  alt: "Graphique présentant la consommation des centres de données entre 2016 et 2050 (projections réalisée par Deloitte)"
%}

## Intelligence artificielle et souveraineté

### Souveraineté nationale

Quand on regarde les outils d'IA générative les plus utilisés (toujours l'enquête Ipsos), on se rend compte que les principaux outils sont gérés par OpenAI, Google et Microsoft. Nous avons donc une position ultra dominante des Etats-Unis sur ces technologies.

Or, l’intelligence artificielle est amenée à bouleverser le monde économique dans lequel on évolue. Il est donc risqué pour un pays de dépendre à ce point des technologies d'un autre pays. L'actualité récente a d'ailleurs montré que les conditions de collaborations avec les Etats-Unis peuvent changer brusquement (avec les droits de douane notamment, mais d'autres leviers sont possibles). De plus, les sociétés américaines sont toujours soumises aux Partiot Act et Cloud Act qui les obligent à donner accès aux données qu'elles hébergent si le gouvernement les exige.

> La France et l'Europe sont donc en train d'investir massivement dans l'IA avec des plans d'investissements respectifs de 109 milliards et 200 milliards d'euros ({% include link.html text="source" link="https://www.info.gouv.fr/actualite/ia-une-nouvelle-impulsion-pour-la-strategie-nationale" %}).
{: .prompt-info}

Ces investissements ont pour but de permettre aux pays de conserver une relative indépendance dans leur développement économique par rapport aux Etats-Unis. 

### Souveraineté au niveau de l'entreprise

Les entreprises doivent également s'intéresser à leur "souveraineté". On parle parfois du facteur d'autobus (ou bus factor en anglais).

> Combien de personnes clés dans votre équipe peuvent se faire renverser par un autobus avant que votre projet échoue ?

Le but étant de faire en sorte d'éviter que trop peu de personnes soient nécessaires au bon fonctionnement d'un projet ou d'une entreprise.

Mais on peut extrapoler ce mesure du risque aux partenaires. Quelle est la résilience de mon entreprise si tel ou tel partenaire arrête de travailler avec nous. Combien de temps me faudra-t-il pour trouver une solution alternative ?

Si on délègue beaucoup à l’intelligence artificielle on peut en devenir dépendant, voire même dépendant de l'entreprise qui nous fournit le service d'IA.

### Souveraineté personnelle

Cette même logique s'applique à l’échelle personnelle. Tout ce qu'on est délègué aux technologies entraîne la perte de compétences. Par exemple, quand j'étais enfant je connaissais une bonne dizaine de numéros de téléphone par coeur. Maintenant, j'ai délégué cele à mon application de contacts. Je n'ai mémorisé que mon numéro et je peine à me souvenir de celui de ma femme. On peut voir cela d'un œil positif (une charge mentale en moins à gérer) ou négatif (mais que devient-on quand on n'a plus de batterie dans son smartphone ?).

Avec l'intelligence artificielle, on en arrive également à des pertes de compétences :
- capacité de synthèse
- rédaction
- créativité
- ...

Ce qui est important, c'est de savoir ce qu'on gagne et ce qu'on perd. On peut ensuite faire ses choix en toute conscience de choses.

## Une transformation des compétences métier

On en arrive à l'adaptation du monde professionnel au bouleversement porté par l'intelligence artificielle. Ce nouvel outil va transformer beaucoup de métiers. Il est vraisemblable qu'à l'avenir, il sera parfois plus utile de savoir bien manier les prompts que d'avoir les savoir-faire actuels.

### Augmentation de la fracture numérique

Savoir piloter l'intelligence artificielle va devenir une compétence clé dans les prochaines années. Mais comment intégrer aux mieux l'ensemble de la population à ce nouvel outil ? Quand on sait qu'en France une personne sur six ne peut pas utiliser internet correctement et qu'une personne sur trois manque d'au moins une compétence numérique de base ({% include link.html link="https://www.insee.fr/fr/statistiques/4241397" text="source" %}), peut-on sereinement envisager un virage vers l'intelligence artificielle sans laisser une partie de la population sur le carreau ?

### Enseignement

Dans l'enseignement, quel est l'impact de l'usage de l'intelligence artificielle sur la rédaction ? Sur la réflexion ? Sur la créativité ?
Faut-il interdire l'IA pour favoriser l'apprentissage de ces compétences ? Comment peut-on cadrer l'usage de l'intelligence artificielle pour apprendre à intégrer cet outil sans oublier de solliciter les autres compétences ?

### Gain de productivité

Enfin, il est indéniable que l'intelligence permet de faire des tâches mieux que les humains. Cela fait quelques années que l'IA bat les humains aux échecs et au jeu de go. Le {% include link.html text="prix Nobel de Chimie en 2024" link="https://www.nobelprize.org/prizes/chemistry/2024/press-release/" %} a été décerné à des ingénieurs ayant su intégrer l'IA dans leurs recherches (j'ai hésité à écrire qu'on avait donné le prix à une intelligence artificielle...).

Quelles vont être les conséquences de ces gains de productivité ? Dans le monde libéral actuel, il semble inévitable de se diriger vers une augmentation de la production globale. Est-ce qu'on peut rendre cela compatible avec les limites planétaires ? Peut-on envisager une réduction du temps de travail ?

## Biais et fiabilité des données

### Biais

Les intelligences artificielles s’entraînent sur les données accessibles (livres, web...). Ces données contiennent nos biais de société privilégiant souvent les hommes, les caucasien.nes...

Les exemples où l'intelligence artificielle vient décupler nos biais de société sont pléthores :
- une jeune fille asiatique demandant à professionnaliser sa photo de profil devient caucasienne
- un algorithme de pré-sélection d'une boite tech n'accepte que les hommes blancs
- une intelligence artificielle permet des crédits plus importants aux hommes qu'aux femmes

La modération est donc nécessaire pour éviter d'amplifier les biais. Mais comment réaliser cette modération sans ouvrir la porte aux manipulations ? Imaginez-vous si l'algorithme de sélection des contenus d'un réseau social était géré par un gouvernement hostile à la liberté d'expression...

### Fiabilité

On disait que la capacité à piloter une intelligence artificielle allait devenir une compétence clé. Une autre compétence qu'il va falloir développer c'est le discernement d'une information fausse.

L'intelligence artificielle permet à tout le monde de facilement :
- falsifier un justificatif d'achat
- faire un photo-montage crédible
- cloner une voix ou même créer une vidéo malveillante

De même l'intelligence artificielle peut faire des erreurs et apporter des informations fausses.

> Plus que jamais, il faut rester critiques vis-à-vis des informations que l'on reçoit. 
{: .prompt-tip }

C'est également une bonne idée de mentionner l'usage de l'intelligence artificielle quand vous y avez recours.

### Législation

L'intelligence artificielle est née dans les années 50 ({% include link.html text="source" link="https://fr.wikipedia.org/wiki/Conf%C3%A9rence_de_Dartmouth" %}).

Toutefois, il a fallu attendre 2024 pour que les premières législations apparaissent avec l'{% include link.html text="IA Act" link="https://commission.europa.eu/news/ai-act-enters-force-2024-08-01_fr" %} de l'union européenne.

Cela montre que notre système législatif ne permet pas de cadrer correctement l’avènement des nouvelles technologies qui se développent trop rapidement.

## Conclusion

Pour résumer :
- L'intelligence artificielle a de forts impacts environnementaux
- C'est un support de croissance et donc elle accélère les impacts sur la planète
- Il faut choisir ses usages et ses outils en toute conscience des enjeux éthiques soulevés (environnementaux, souveraineté, biais...)
- Ne pas trop déléguer à l'IA : veiller à garder le contrôle de sur notre développement, nos compétences, notre indépendance
- Rester critique sur les usages et les résultats
- La réflexion éthique reste sous la responsabilité de l'humain


## Pour aller plus loin

- Participer à une [Bataille de l'IA](/services/sensibilisation/bataille_ia)
- Se former pour un [usage responsable de l'intelligence artificielle](/formations/intelligence-artificielle-responsable)
- Le {% include link.html text="MOOC de l'INRIA" link="https://www.fun-mooc.fr/fr/cours/lintelligence-artificielle-avec-intelligence/" %} sur l'intelligence artificielle
- Le {% include link.html text="RIA31" link="https://ref-ia.isit-europe.org/" %}, un référentiel de l'INR pour dévélopper une intelligence artificielle reposnable

## Post-scriptum

Cet article aurait pu être rédigé par l'IA. Dans une moindre mesure, j'aurais pu utiliser l'intelligence artificielle pour réaliser la recherche documentaire ou partir de mon plan détaillé pour tout faire rédiger. Ce n'est évidemment pas le cas !

Au-delà de la réduction de l'impact environnemental, ce qui motive la rédaction de mes articles c'est ma montée en compétence. Je ne manque jamais une occasion d'apprendre même sur des articles de sensibilisation de ce genre. La recherche documentaire et la confrontation à des points de vue différents me permettent d'ouvrir le champ de mes connaissances. La rédaction permet de mieux structurer mes idées

Mon implication intense dans les articles me donne également un sentiment de fierté qui serait moindre si je déléguais tout ou partie à l'IA. J'ai également un degré de confiance plus important dans ce que j'écris, car il n'y a pas d'effet boite noire. D'ailleurs je cite toujours mes sources.

J'espère que cela se ressent à la lecture.