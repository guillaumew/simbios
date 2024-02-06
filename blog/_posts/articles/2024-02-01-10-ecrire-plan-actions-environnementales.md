---
title: "Ecrire un plan d'actions environnementales"
description: Voici un des dix commandements pour diminuer rapidement l'empreinte environnementale d'un site internet.
tags: ["Site", "Eco-conception", "Produit"]
image: /assets/img/posts/2024/Q1/ecoconception-site.webp
thumb: /assets/img/posts/2024/Q1/ecoconception-site
hidden: true
---

Avec les 9 commandements précédents, on a déjà pu largement baisser la taille de son site. Mais il est toujours possible d'aller plus loin. Cela risque de prendre un peu plus de temps.

Il est important de considérer rapidement les actions possibles, même si on décide de ne pas les planifier imméidatement.

Cela permettra de les inclure dans des travaux ou des réflexions sur des chantiers à venir. 

## Privilégier le sur-mesure aux CMS

Les CMS (Wordpress, Wix...) sont généralement très gourmands en ressources et loin de proposer une solution écologiquement justifiable.

Dans de nombreux cas, il peut être rapidement rentable (environnementalement et économiquement) de faire quelques petits développements pour proposer une solution sur-mesure.

## Choisir les bibliothèques externes légères et adaptées

Depuis de nombreuses années, les outils mis à disposition des développeur.se.s non cesser de croître. On a pris l'habitude d'intégrer de manière quasi-systématique des outils comme JQuery, Bootstrap, FontAwesome ainsi qu'un framework javascript (Angular, VueJS, React...)

Pourtant ces outils ne sont pas toujours adaptés voire utiles. Ils embarquent souvent beaucoup plus de fonctionnalités que ce que nous utilisons.

Il peut être intéressant de :
- choisir une bibliothèque plus adaptée à son besoin (par exemple PureCSS plutôt que Bootstrap)
- retirer le code inutilisé dans la bibliothèque choisie
- écrire le code nécessaire soi-même quand il est d'une difficuluté/taille accessible

## Travailler sur le besoin utilisateur et l'ergonomie

L'essentiel du travail ici a été technique. On s'est intéressé au développement d'un site. Mais il y a beaucoup à optimiser avec une réflexion plus orientée produit.

Je vous propose les pistes proposées par le collectif {% include link.html text="Conception Numérique Responsable" link="https://collectif.greenit.fr/" %} :

### Eliminer les fonctionnalités non essentielles
Plusieurs études (Cast Software et Standish Group, notamment) démontrent que 70 % des fonctionnalités demandées par les utilisateurs ne sont pas essentielles et que 45 % ne sont jamais utilisées. En réduisant la couverture et la profondeur fonctionnelle de l’application, on abaisse son coût de développement initial, sa dette technique et les impacts environnementaux associés.

On diminue ainsi mécaniquement l’infrastructure nécessaire à son exécution. Par ailleurs, à niveau ergonomique constant, plus l’application est pauvre fonctionnellement, plus elle sera simple à utiliser. Il faut donc réduire le plus possible la couverture fonctionnelle de l’application, en la centrant sur le besoin essentiel de l’utilisateur.

Détecter une fonctionnalité non essentielle est possible au moment de l'analyse de l'expression du besoin. La méthode MoSCoW, des ateliers, des wireframes (maquettes fonctionnelles) ou des prototypes avec tests utilisateurs permettent de vérifier l'utilité d’une fonctionnalité en amont de son développement.
### Quantifier le besoin

Les « dimensions » de chaque fonctionnalité doivent être définies précisément et dans leur ensemble. Il peut s’agir d’un taux de compression pour les images de l’interface graphique, du temps de réponse maximum pour une requête HTTP, du nombre d’items affichés dans une liste, etc.

Plus les « dimensions » et exigences associées à chaque fonctionnalité collent au métier, plus on évite la surqualité. La logique doit donc être inversée par rapport aux habitudes actuelles. Si une information n’est pas précisée, c’est le niveau de qualité ou la quantité minimale qui est proposé. Par exemple, en l’absence de précision, le nombre d’items d’une liste est limité à 5 éléments ou au nombre maximal affichable sur le plus petit écran cible de l’application.

Les valeurs par défaut, rarement modifiées par l'utilisateur, doivent être choisies pour répondre au besoin avec un impact minimal.

Gain potentiel : en jouant sur le nombre d’items affichés sur la page de résultats de son moteur de recherche Bing, Microsoft Research a démontré qu’il était possible de réduire jusqu’à 80 % l’infrastructure physique (nombre de serveurs) sous-jacente.

Autre exemple : en utilisant par défaut une résolution de vidéo acceptable (480p) plutôt que maximale, on réduit la bande passante utilisée pour la plupart des utilisateurs (qui ne changeront pas la valeur par défaut), tout en laissant la possibilité aux autres d'augmenter la résolution s'ils en en ont le besoin.

### Optimiser le parcours utilisateur

Optimiser le parcours utilisateur consiste à diminuer le temps passé par l'utilisateur sur ses usages les plus fréquents. Dans un premier temps, cibler les parcours les plus fréquents puis optimiser leur usage : diminuer le nombre d'étapes, diminuer le nombre d'actions, supprimer l'inutile, identifier les cas d'échecs, optimiser les temps de réponse... Un parcours est bien conçu lorsque le programme se comporte exactement comme l'utilisateur l'avait imaginé.

A minima, sonder en observant son entourage utilisant le service est un bon moyen d’identifier les points de friction - situations ou interactions qui contribuent à dégrader l’expérience utilisateur et à ralentir le parcours - des utilisateurs. Les tests utilisateurs permettent d'aller plus en profondeur dans la recherche de ces points de friction.

Le temps passé par l'utilisateur sur son terminal est le deuxième poste en termes d'impacts environnementaux.


*[Revenir à la liste de commandements](dix-min-pour-reduire-empreinte-environnementale-site.html)*