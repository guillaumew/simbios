---
title: "Les modes sombres (dark mode/theme)"
description: "Comment économiser jusqu'à 35% de batterie sur un simple paramétrage"
tags: ["Paramétrage", "Electricité", "Eco-geste", "Sombre"]
image: /assets/img/posts/2024/Q2/thumb-darkmode.webp
thumb: /assets/img/posts/2024/Q2/thumb-darkmode
podcast: https://sphinx.acast.com/p/open/s/65e06335dd3dcf001643bd06/e/66744c428fbce3001224ef74/media.mp3
---

## A quoi correspond le mode sombre ?

La plupart des smartphones et des navigateurs proposent un mode de fonctionnement alternatif qui permet de privilégier un affichage blanc sur noir plutôt que noir sur blanc.

Ce mode de fonctionnement s'appelle généralement le mode sombre ou dark mode ou peut porter des noms similaires (dark theme, smart dark).

Les applications ou site internet qui ont fait l'effort de supporter cette fonctionnaltié doivent donc privilégier des fonds sombres voire noirs.

{% responsive_image 
  path: assets/img/posts/2024/Q2/dark-light.webp 
  alt: "La différence visuelle entre le mode sombre et le mode clair sur le site Simbios" 
%}
*Voici le mode classique et le mode sombre sur le blog Simbios*

## A quoi sert le mode sombre ?

### S'adapter à la luminosité ambiante

Le mode sombre permet de limiter la lumière provenant de son écran (un fond d'écran sombre émet moins de lumière qu'un fond blanc). Cela peut s'avérer confortable dans des environnements où il y a peu de lumière ambiante.

### Une lisibilité généralement plus difficile 

Dans certains cas, cela permet même d'améliorer la facilité de lecture. Toutefois, il semble accepté que de manière générale, la lecture noir sur fond blanc (mode positif) est plus efficace. Voici quelques études :

- {% include link.html link="https://www.tandfonline.com/doi/abs/10.1080/00140139.2013.790485" text="Positive display polarity is advantageous for both younger and older adults" %}. 
- {% include link.html link="https://journals.sagepub.com/doi/10.1177/0018720813515509" text="Positive Display Polarity Is Particularly Advantageous for Small Character Sizes: Implications for Display Design" %}. 
- {% include link.html link="https://www.sciencedirect.com/science/article/abs/pii/S0003687016302459?via%3Dihub" text="Effects of ambient illumination, contrast polarity, and letter size on text legibility under glance-like reading" %}. 
- {% include link.html link="https://dl.acm.org/doi/abs/10.1145/3357251.3357584" text="Effects of Dark Mode on Visual Fatigue and Acuity in Optical See-Through Head-Mounted Displays" %} (seule cette étude favorise le mode sombre). 

### Une économie d'énergie

Pour afficher des couleurs sur l'écran, ce dernier doivent envoyer de la lumière, mais pour afficher du noir, il suffit de ne pas envoyer de lumière, ce qui ne consomme donc pas d'énergie. En proposant une interface composée majoritairement de noire, on fait donc des économies d'énergie.

Comme on l'a vu dans [l'article sur l'impact environnemental des messageries](/blog/2024/05/13/ecoconception-services-messagerie), utiliser le mode sombre permet de diminuer jusqu'à 35% la consommation d'énergie de votre smartphone. Cela dépend évidemment des applications utilisées, mais il s'agit là d'un gain significatif.

Si vous n'êtes pas gêné par la lecture en mode sombre, je vous invite donc vivement à utiliser le mode sombre !

## Comment activer le mode sombre ?

Mettre en place le mode sombre sur votre smartphone :

- {% include link.html link="https://support.google.com/android/answer/9730472?hl=fr" text="Passer au mode sombre ou au mode couleur sur votre appareil Android" %}.
- {% include link.html link="https://support.apple.com/fr-fr/108350" text="Utiliser le Mode sombre sur votre iPhone et votre iPad" %}.

Mettre en place le mode sombre sur votre ordinateur :

- {% include link.html link="https://support.microsoft.com/fr-fr/windows/modifier-les-couleurs-dans-windows-d26ef4d6-819a-581c-1581-493cfcc005fe" text="Modifier les couleurs dans Windows (10 et 11)" %}.
- {% include link.html link="https://support.apple.com/fr-fr/guide/mac-help/mchl52e1c2d2/mac" text="Utiliser une apparence claire ou sombre sur votre Mac" %}.

Mettre en place le mode sombre sur votre navigateur web :

- {% include link.html link="https://support.google.com/chrome/answer/9275525?hl=fr-FR" text="Naviguer en mode sombre ou avec le thème sombre sur Chrome" %}.
- {% include link.html link="https://support.mozilla.org/fr/kb/changer-parametres-apparence-sites-web-firefox" text="Changer les paramètres d’apparence des sites web dans Firefox" %}.
- {% include link.html link="https://support.microsoft.com/fr-fr/microsoft-edge/utiliser-le-th%C3%A8me-sombre-dans-microsoft-edge-9b74617b-f542-77ed-033b-1a5cfb17a2df" text="Utiliser le thème sombre dans Microsoft Edge" %}.
- {% include link.html link="https://www.hardreset.info/fr/devices/apps/apps-opera/enable-dark-theme/" text="Comment activer le thème sombre sur Opera" %}.

## Pour les éditeurs de site ou application

Le mode sombre doit être géré au niveau de chaque site ou application. Ce n'est pas le navigateur qui changera les couleurs pour vous.

En HTML, il suffit de charger vos CSS avec
```
@media (prefers-color-scheme: dark) {
  /*
  Votre code CSS pour changer les couleurs d'affichage
  */
}
```

Plus d'information sur la {% include link.html link="https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-color-scheme" text="documentation Mozilla" %}