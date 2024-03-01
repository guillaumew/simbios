---
title: "Limitier les ressources externes"
description: Voici un des dix commandements pour diminuer rapidement l'empreinte environnementale d'un site internet.
tags: ["Site", "Eco-conception", "cookie", "http"]
image: /assets/img/posts/2024/Q1/ecoconception-site.webp
thumb: /assets/img/posts/2024/Q1/ecoconception-site
hidden: true
---

## Le problème 

Lorsque vous avez besoin de ressources externes (images, CSS...), on peut être tenté de laisser des sites externes les héberger pour nous.

Mais cela force le navigateur à ouvrir un nouvelle connexion HTTP pour chaque domaine ce qui est moins performant.

## Comment faire ?

L'idéal c'est de servir les fichiers avec son propre de domaine l'ensemble des ressources nécessaires.

Il faut donc tout héberger sur son propre service.

### Et le cache multi-site ?

Depuis de nombreuses années, {% include link.html text="les navigateurs n'autorisent plus l'emploi partagé du cache entre plusieurs site" link="https://www.stefanjudis.com/notes/say-goodbye-to-resource-caching-across-sites-and-domains/" %}.

Cela pouvait être pratique vu que tout le monde utilise les mêmes bibliothèque, mais cela posait des problèmes de sécurité / confidentialité des données.

### Et les cookies ?

Si vous avez une large utilisation de cookies, il peut être intéressant d'avoir un sous-domaine pour gérer sépareremment les ressources externes ne nécessitant pas de cookie.

## Ensuite ?

- Voir le commandement suivant : [Les ajouts inutiles, tu éviteras](03-eviter-ajouts-inutiles.html)
- [Revenir à la liste de commandements](dix-min-pour-reduire-empreinte-environnementale-site.html)