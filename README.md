# Simbios

## Enpreinte environnementale du site
Conformément à la vision de Simbios, ce site est conçu pour avoir une empreinte environnemental réduite.
A l'heure de l'écriture du ce read me, la home page possède un [écoindex A](https://www.ecoindex.fr/resultat/?id=8278ca23-a84d-4fb9-afc7-f06f397b1b77) (91/100) :
 - 30 ko (15 ko compressé)
 - 139 éléments dans le DOM
 - 6 requêtes
 
Soit une consommation estimée à 1,8 cl d'eau et 1,2 gCO2e par visite.

## Mise en place

Pour le CSS, il s'agit d'une solution complètement custom inspirée de [Pure.css](https://purecss.io/). Petite fantaisie pour les grilles, les tailles sont directement indiquées en variables CSS dans le HTML.

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

ou

``` JEKYLL_ENV=production bundle exec jekyll serve ```

Cela doit créer un site temporaire qui va se mettre à jour à chaque modification de fichier.


## Déploiment

Lorsque le site est prêt, il suffit de faire un 
``` rake site:publish ```
pour publier. 

Attention, cela fonctionne à partir de n'importe quelle branche et ça publie directement en production. A ce stade, il n'y a pas d'environnement tests en dehors de l'environnement local.

Ne pas oublier de publier les modifications sur master (la publication avec rake ne suffit pas)

## Structure du projet
J'ai suivi les conventions indiquées dans le tutoriel de Jekyll. Je vous laisse le consulter.
https://jekyllrb.com/docs/step-by-step/01-setup/