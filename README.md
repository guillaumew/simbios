# Simbios

## Enpreinte environnementale du site
Conformément à la vision de Simbios, ce site est conçu pour avoir une empreinte environnemental réduite.
A l'heure de l'écriture du ce read me, la home page possède un [écoindex A](https://www.ecoindex.fr/resultat/?id=8278ca23-a84d-4fb9-afc7-f06f397b1b77) (90/100) :
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

## Mise à jour des Ecoindex

Lancer le calcul de l'éco-index avec le [eco-index-cli](https://github.com/cnumr/ecoindex_python_fullstack/blob/main/projects/ecoindex_cli/README.md).

Lancer Docker
Dans un terminal (pas de VS code) :

``` ecoindex-cli analyze --url https://simbios.fr --recursive --export-format json ```

Répondre Oui (Y) deux fois.

La réponse ressemblera à 

```
You are about to perform a recursive website scraping. This can take a long time. Are you sure to want to proceed? [Y/n]: Y
⏲ Crawling root url https://simbios.fr -> Wait a minute!
-2024-02-20 09:58:17 [scrapy.utils.log] INFO: Scrapy 2.11.0 started (bot: scrapybot)
2024-02-20 09:58:17 [scrapy.utils.log] INFO: Versions: lxml 4.9.3.0, libxml2 2.10.3, cssselect 1.2.0, parsel 1.8.1, w3lib 2.1.2, Twisted 22.10.0, Python 3.12.0 (main, Nov 29 2023, 03:23:09) [GCC 12.2.0], pyOpenSSL 23.3.0 (OpenSSL 3.1.4 24 Oct 2023), cryptography 41.0.7, Platform Linux-6.5.11-linuxkit-x86_64-with-glibc2.36
📁 Urls recorded in file `/tmp/ecoindex-cli/input/simbios.fr.csv`
There are 53 url(s), do you want to process? [Y/n]: Y
53 urls for 1 window size with 4 maximum workers
100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 53/53 • 0:02:00 • 0:00:00
┏━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┓
┃ Total analysis ┃ Success ┃ Failed ┃
┡━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━┩
│ 53             │ 53      │ 0      │
└────────────────┴─────────┴────────┘
🙌 File /tmp/ecoindex-cli/output/simbios.fr/2024-02-20_100037/results.json written !
```

Il faut noter le répertoire dans lequel se trouve les résultats, ici : `2024-02-20_100037`

Ensuite il faut faire (dans vs code, dans le dossier Simbios) :
``` rake site:ecoindex 2024-02-20_100037 ```

Cela va mettre à jour le fichier `_data/ecoindex.yml`
Ce fichier sera utilisé dans les builds pour écrire les scores sur chaque page.

## Déploiment

Lorsque le site est prêt, il suffit de faire un 
``` rake site:publish ```
pour publier. 

Cela va mettre à jour la branche `gh-pages` avec le build du site.

Attention, cela fonctionne à partir de n'importe quelle branche et ça publie directement en production. A ce stade, il n'y a pas d'environnement tests en dehors de l'environnement local.

Ne pas oublier de publier les modifications sur master (la publication avec rake ne suffit pas)

## Structure du projet
J'ai suivi les conventions indiquées dans le tutoriel de Jekyll. Je vous laisse le consulter.
https://jekyllrb.com/docs/step-by-step/01-setup/