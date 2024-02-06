---
title: "Compresser les fichiers"
description: Voici un des dix commandements pour diminuer rapidement l'empreinte environnementale d'un site internet.
tags: ["Site", "Eco-conception", "NGINX", "Apache", "gzip", "Brotli"]
image: /assets/img/posts/2024/Q1/ecoconception-site.webp
thumb: /assets/img/posts/2024/Q1/ecoconception-site
hidden: true
---

Dans le commandement précédent, on a vu comment [minifier les ressources](07-minifier-css-javascript-html.html). A cela s'ajoute également la possibilité de les compresser !

## Le problème 

La compression des fichiers (GZip, Brotli...) permet de diminuer la taille de ces derniers pour qu'ils utilisent moins de ressources réseau. 

La compression peut nécessiter un peu de ressources côté serveur quand elle est très optimisée, mais elle n'est à faire qu'une seule fois alors qu'elle servira à chaque visite.
Côté navigateur, la décompression utilise des ressources négligeables.

## Comment faire ?

Les serveurs Apache et NGINX savent tous les deux compresser les fichiers. C'est même par défaut pour les fichiers HTML sur NGINX. Mais il faut tout de même ajouter quelques paramètres pour que l'ensemble des fichiers soient compresser.

- {% include link.html link="https://www.digitalocean.com/community/tutorials/how-to-improve-website-performance-using-gzip-and-nginx-on-ubuntu-20-04" text="Suivre le tutoriel sur NGINX" %}.
- {% include link.html link="https://ali-dev.medium.com/how-to-setup-caching-gzip-compression-in-apache-web-server-with-htaccess-292a0f689553" text="Suivre le tutoriel sur Apache" %}.
- Sur Wordpress, il existe des extensions pour gérer cela. {% include link.html link="https://www.codeur.com/tuto/wordpress/activer-compression-gzip-wordpress/" text="Voir le tutoriel" %}.

## Ensuite ?

- Voir le commandement suivant : [Le cache, tu géreras](09-gerer-cache.html)
- [Revenir à la liste de commandements](dix-min-pour-reduire-empreinte-environnementale-site.html)