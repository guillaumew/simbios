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

L'idéal c'est de n'utiliser de servir avec son propre de domaine l'ensemble des ressources nécessaires.

Il faut donc tout héberger sur son propre service.

## Et les cookies ?

Si vous avez une large utilisation de cookies, il peut être intéressant d'avoir un sous-domaine pour gérer sépareremment les ressrouces externes ne nécessitant pas de cookie.

## Ensuite ?

- Voir le commandement suivant : [Les ajouts inutiles, tu éviteras](03-eviter-ajouts-inutiles.html)
- [Revenir à la liste de commandements](http://127.0.0.1:4000/blog/2024/02/01/dix-min-pour-reduire-empreinte-environnementale-site.html)