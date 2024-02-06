---
title: "Limitier les ressources externes"
description: Voici un des dix commandements pour diminuer rapidement l'empreinte environnementale d'un site internet.
tags: ["Site", "Eco-conception"]
image: /assets/img/posts/2024/Q1/ecoconception-site.webp
thumb: /assets/img/posts/2024/Q1/ecoconception-site
hidden: true
---

## Le problème 

On a parfois tendance à ajouter des fonctionnalités ou des plugins sans trop considérer leur utilité. Ces dernières peuvent avoir un impact non négligeables.

## Quelques exemples

### Les boutons des réseaux sociaux

Les boutons des réseaux sociaux ne sont clairement pas éco-conçus. Un simple bouton cache généralement une dizaine de requêts et une centaine de Ko transférés.

Il est pourtant très facile de faire des boutons sur mesure avec des URLs du type :

| Réseau social  | URL de partage |
|----------------|----------------|
| Facebook Share | https://www.facebook.com/sharer/sharer.php?u=XXX        |
| Facebook Like  | https://www.facebook.com/plugins/like.php?href=XXX      |
| Twitter        | https://twitter.com/intent/tweet?url=XXX                |
| LinkedIn       | https://www.linkedin.com/sharing/share-offsite/?url=XXX |

Cela permet de maîtriser leur impact environnemental mais aussi de les adapter à votre charte graphique.

### Les vidéos 

#### Vidéos en arrière plan
Il y a depuis quelques années, une mode qui consiste à mettre des vidéos en arrière plan. Cela peut nécessiter des dizaines de Mo de données à transférer et cela consomme pas mal de ressource sur le terminal utilisateur. Pourtant l'intérêt pour les utilisateur.trice.s est faible. Cela peut même perturber la navigation ou nuire au message principal.

#### Vidéos en lecture automatique
De manière générale, il faut laisser l'utilisateur choisir quand il souhaite lancer un contenu vidéo. On peut décider de charger le lecteur à ce moment là également.

### Les outils d'analytics
Connaissez-vous toutes les fonctionnalités d'un outils aussi complet que Google Analytics ? Probablement que non...

Peut-être qu'un outil plus simple sera largement suffisant pour vos besoins :
- Nombre de requêtes calculées côté serveur
- {% include link.html text="Plausible Analytics" link="https://plausible.io/lightweight-web-analytics" %}.
- {% include link.html text="Light Analytics" link="https://liteanalytics.com/" %}.
- {% include link.html text="Data Pulse" link="https://datapulse.app/" %}.
- {% include link.html text="Pirsch Analytics" link="https://pirsch.io/fr" %}.

### Autres

Il y a plein d'exemple de mauvaise pratique avec des ajouts de code inutiles. N'hésitez pas [à proposer les vôtres](contact.html) !

## Ensuite ?

- Voir le commandement suivant : [Les polices standards, tu favoriseras](04-favoriser-polices-standard)
- [Revenir à la liste de commandements](dix-min-pour-reduire-empreinte-environnementale-site.html)