---
title: "Redimensionner et compresser les images"
description: Voici un des dix commandements pour diminuer rapidement l'empreinte environnementale d'un site internet.
tags: ["Site", "Eco-conception", "Images", "Compression"]
image: /assets/img/posts/2024/Q1/ecoconception-site.webp
thumb: /assets/img/posts/2024/Q1/ecoconception-site
hidden: true
---

## Le problème 
On voit souvent des sites qui utilisent les images telles qu'elles ont été trouvées ou fournies. C'est comme cela qu'on trouve des images d'utlre haute qualité et de taille importante qui sont utilisée comme miniatures par exemple.

Cela demande plus de ressources réseaux pour transférer les images et plus de ressources CPU pour les afficher.

## Comment faire ?

### Choisir le bon format d'image

Il existe de nombreux formats d'images (bmp, jpg, gif, webp, avif...). Pour vérfier quel format est le plus efficace, il n'y a pas trop d'autre solution que de les tester. Pour cela l'outil de Cloudinary donné plus bas est très efficace.

Ceci dit, à part quelques exceptions, les formats les plus récents (webp, avif) seront les plus performants.

Mais ces formats ne sont pas compatibles avec les anciens navigateurs. Or la rétro-compatibilité est ce qu'il y a de plus important d'un point de vue environnemental car c'est la fabrication des terminaux qui pèse le plus lourd. Heureusement, il existe une astuce pour avoir un fallback vers un format plus conventionnel.

```
<picture>
    <source srcset="/assets/img/guillaume-wolf.webp" type="image/webp">
    <source srcset="/assets/img/guillaume-wolf.jpg" type="image/jpg"> 
    <img src="/assets/img/guillaume-wolf.jpg" alt="Photo de Guillaume Wolf" title="Photo de Guillaume Wolf" width="256" height="256" loading="lazy">
</picture>
```
Les navigateur non compatibles non vont lire que la balise **img** parce qu'ils ne comprennent pas les autres. Les navigateurs récents vont comprendre qu'il faut utiliser le format webp s'ils sont compatibles.

Notez également l'apparition de l'attibut **loading="lazy"** qui permet de ne dire au navigateur de ne télécharger cette image qu'à partir du moment où elle est sur le point d'apparaître à l'écran.

### Trouver la (les ?) bonne taille

Si l'image a une taille fixe sur la page (comme par exemple la vignette de cet article), il suffit de la redimensionner à la cette taille.

Si la taille de l'image varie en fonction de la taille de la fenêtre (image responsive). Il y a plusieurs possibilités.
- On trouve une nouvelle manière d'afficher l'image pour qu'elle ait toujours la même taille. C'est ce qui a été fait pour les vignettes des articles de ce blog. Elles apparaissent toujours en 200x200px.
- On choisit une taille d'image par défaut et on accepte le redimensionnement du navigateur. C'est dommage mais cela peut être plus facile et n'avoir que peu d'incidence si la taille de l'image de varie pas trop. A ce moment, on se retrouve face au choix de prendre l'image la plus grande pour qu'elle s'affiche correctement chez tout le monde ou la plus petite pour optimiser la taille du fichier chez tout le monde... ou une position entre les deux...
- Il existe aussi une astuce pour permettre de limiter le redimensionnement de l'image par le navigateur. Par exemple l'image ci-dessous :

{% responsive_image 
  path: assets/img/posts/2024/Q1/resize-image.webp 
  alt: "Une photo d'une photo... mise en abyme..." 
  title: "Cette image s'affiche différemment en fonction de votre taille de fenêtre.
%}

Quand on regarde le code : 
```
<picture>
    <source media="(min-width: 768px)" srcset="image-768x512.webp" type="image/webp" height="512" width="768">
    <source media="(min-width: 480px)" srcset="480x320.webp" type="image/webp" height="320" width="480">
    <source media="(min-width: 320px)" srcset="320x213.webp" type="image/webp" height="213" width="320">
    <img src="/assets/img/posts/2024/Q1/resize-image.jpg" alt="Une photo d'une photo... mise en abyme..." title="Une photo d'une photo... mise en abyme..." loading="lazy">
</picture>
```
On voit qu'il y a 4 images différentes disponibles. Si le navigateur ne peut pas afficher un wepb, il prendre l'image par défaut (un jpg), sinon en fonction de la taille de la fenêtre il va choisir l'image la plus adaptée.

## Les outils

Il existe de nombreux outils pour traiter les images. Je vais en citer quelques uns que j'utilise dans différents contextes :

- {% include link.html link="http://webspeedtest.cloudinary.com" text="Webspeed Test de Cloudinary" %} permet de tester l'URL de votre page. L'outil va montrer quelles images peuvent être optimisées. Mieux vous pouvez directement télécharger l'image parfaite pour votre page !
- Pour retailler les images en lot, j'utilise {% include link.html link="https://converseen.fasterland.net/" text="Converseen" %}. Cet outil est complet et permet de modifier la taille ainsi que de convertir dans un format plus optimal et même de compresser (pour les formats Webp et Jpg).
- Pour automatiser le traitement d'image, l'outil le plus utilisé sur le marché est {% include link.html link="https://imagemagick.org/index.php" text="ImageMagick" %}. Il permet de créer des scripts permettant de faire tous les traitements d'images nécessaires de manière automatisée.
- Pour gérer les images responsives (dont la taille peut varier en fonction de la taille de la fenêtre de l'utilisateur.ice), j'utilie {% include link.html text="jekyll-responsive-image " link="https://github.com/wildlyinaccurate/jekyll-responsive-image" %}. Ca ne vous servira que si vous utilisez Jekyll mais cela permet de tout automatiser.

## Ensuite ?

- Voir le commandement suivant : [les ressources externes, tu limiteras](02-limiter-ressources-externes.html)
- [Revenir à la liste de commandements](dix-min-pour-reduire-empreinte-environnementale-site.html)