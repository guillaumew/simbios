---
title: "Eviter les insertions de contenus"
description: Voici un des dix commandements pour diminuer rapidement l'empreinte environnementale d'un site internet.
tags: ["Site", "Eco-conception", "DOM"]
image: /assets/img/posts/2024/Q1/ecoconception-site.webp
thumb: /assets/img/posts/2024/Q1/ecoconception-site
hidden: true
---

## Le problème 

Nous avons de plus en plus l'habitude de manipuler le DOM de la page pour y insérer du contenu dynamiquement. Les puissants frameworks javascript (VueJS, React, Angular...) nous y insitent pas mal.

C'est indispensable quand le contenu est dynamique (typiquement deux utilisateurs ne voient pas la même chose s'ils se connectent sur Facebook). Mais si tout le monde doit voir le même contenu, c'est totalement inutile. 

Il est beaucoup plus intéressant de livrer la page HTML directement avec tout le contenu.

## Comment faire ?

La première question à se poser est "Est-ce que les internautes voient tous le même contenu sur mon site ?". Si la réponse est affirmative, il ne devrait pas y avoir besoin de faire de manipulation de DOM. (et probablement qu'il n'y a pas besoin de backend non plus)

La question suivante est "Pourquoi j'ai décidé d'insérer mon contenu dynamaiquement ?"
Si c'est par commodité, pour rester sur une technologie que vous maîtrisez, cela peut se comprendre, mais cela peut valoir le coup (coût ?) de se former à d'autres technos plus adaptées.

Si c'est pour avoir une meilleure gestion du contenu, il existe une foule d'outils qui permettent de faire cela sans obliger les navigateurs de chaque internaute qui visite votre page à construire cette dernière. Quelques exemples :
- {% include link.html text="Hugo" link="https://gohugo.io/" %}.
- {% include link.html text="Jekyll" link="https://jekyllrb.com/" %}.
- {% include link.html text="Nunjucks" link="https://mozilla.github.io/nunjucks/" %}.
- {% include link.html text="Eleventy" link="https://www.11ty.dev/" %}.


## Ensuite ?

- Voir le commandement suivant : [Le javascript, les CSS et le HTML, tu minifieras](07-minifier-css-javascript-html.html)
- [Revenir à la liste de commandements](dix-min-pour-reduire-empreinte-environnementale-site.html)