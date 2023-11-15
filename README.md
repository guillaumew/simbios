# Simbios

## Enpreinte environnementale du site
Conformément à la vision de Simbios, ce site est conçu pour avoir une empreinte environnemental réduite.
A l'heure de l'écriture du ce read me, il possède un [écoindex A](https://www.ecoindex.fr/resultat/?id=8278ca23-a84d-4fb9-afc7-f06f397b1b77) (91/100) :
 - 54.8 ko (23.0 ko compressé)
 - 108 éléments dans le DOM
 - 8 requêtes
 
Soit une consommation estimée à 1,78 cl d'eau et 1,19 gCO2e par visite.

## Mise en place
Pour le moment, il n'y a pas de javascript. J'espère pouvoir rester cette dynamique.
Pour le CSS, j'ai utilisé [Pure.css](https://purecss.io/). Pour aller un cran plus loin, je pourrai décider de passer sur une solution complètement custom.
Les images doivent être ajoutées au format webp et optimisée manuellement pour le moment (je n'ai pas encore trouvé de solution compatible avec Github page)
Les icônes sont gérées directement en svg dans le CSS.
Les feuillets CSS sont listés dans `/assets/css/`. Ils sont générés à partir des fichiers dans `/_sass/`

## Installation
Il faut avoir Ruby, RubyGems, GCC et Make sur son ordinateur. Voir [le guide d'installation](https://jekyllrb.com/docs/installation/).
Puis il suffit de faire un
```bundle install```

## Lancement
Faire
``` bundle exec jekyll serve ```

Cela doit créer un site temporaire qui va se mettre à jour à chaque modification de fichier.

## Structure du projet
J'ai suivi le tutoriel de Jekyll. Je vous laisse le consulter.
https://jekyllrb.com/docs/step-by-step/01-setup/