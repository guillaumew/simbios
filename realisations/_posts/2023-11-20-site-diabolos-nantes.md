---
title: Diminution de l'empreinte du site des Diabolos Nantes
description: Application des outils d'éco-conception aux conditions réelles d'un site statique
tags: ["Ecoconception", "Réécriture", "Site"]
image: /assets/img/posts/2023/Q4/thumb_diabolos_nantes.webp
---

En 2018, j’avais créé un site pour ma troupe de théâtre d’improvisation. Ce site doit permettre de communiquer sur nos spectacles à venir. Mon objectif était alors de proposer une page statique qu’il était raisonnablement facile de mettre à jour. La raison principale de cette mise à jour du site était de faire un site qui s’affiche correctement sur les mobiles (en mode responsive donc).

![Logo de la troupe des Diabolos Nantes](/assets/img/posts/2023/Q4/thumb_diabolos_nantes.webp){:loading="lazy"}

Dans le but d’aller vite, j’ai pris un joli template que j’ai adapté aux couleurs de la troupe. J’ai installé Angular JS et j’ai géré la liste des spectacles dans un fichier JSON. Ce n’est pas ce qu’il y a de plus facile pour la mise à jour des spectacles mais bon je ne voulais pas passer trop de temps sur ce sujet.

A ce moment, je n’avais que très peu de considération de sobriété, à part le fait que le page devait s’afficher dans un délai raisonnable. 5 ans plus tard, je ne peux pas ignorer un site qui ne respecte pas mes valeurs. Il est temps d'agir.

## Etat des lieux

Vous pouvez retrouver le site tel qu’il existait avant {% include link.html text="sur cette adresse (temporaire)" link="https://diabolos-nantes-sept-2023.netlify.app/" external=true %}.

On va commencer par regarder l’ecoindex de la page. On constate qu’on s’en tire pas trop mal. Le score est de B : 75,98/100
Cela implique une estimation de 2,22 cl de consommation d’eau pour un bilan carbone de 1,48gCO2eq pour chaque visite.

| Nombre de requêtes | Taille de la page | Taille du DOM |
|--------------------|-------------------|---------------|
| 33                 | 2,4 Mo            | 109           |

Au niveau de la taille du DOM on est bien. Il faudra rester sur cet ordre de grandeur avec une centaine d’éléments.

Je constate qu’une dizaine de requêtes proviennent du plugin Facebook. Voici un module qui coûte beaucoup, pour peu d’utilité. On va donc le supprimer.
On a aussi 6 requêtes javascript pour un site complètement statique c’est bien dommage.
Le gros de la taille provient sans surprise des images. On devrait pouvoir optimiser cela.

## Objectifs

On va catégoriser l'ensemble des requêtes réalisées par le site ainsi que leur taille totale. Pour chaque catégorie on va estimer les gains possibles.

|    Catégorie    | Nb requêtes | Poids  |                                                                                                Commentaire                                                                                                | Objectif requêtes | Objectif poids |
|:---------------:|:-----------:|:------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------:|:--------------:|
| Index.html      | 1           | 2,9 ko | Il n’y a pas grand chose à gagner ici.                                                                                                                                                                    | 1                 | 1,5 ko         |
| CSS             | 8           | 33 ko  | On va remplacer bootstrap par pure.css. On va agréger l’ensemble des CSS dans un seul fichier.                                                                                   | 2                 | 10 ko          |
| Font            | 4           | 152 ko | On va rester sur les fonts système. Je ne vais importer que les icônes utiles de font awesome. On devrait donc arriver à une seule requête de quelques ko.                                                | 1                 | 3 ko           |
| Javascript      | 6           | 112 ko | On va enlever l’ensemble du javascript sur le site statique. La page devra être générée automatiquement à partir d’informations extérieures.                                                              | 0                 | 0 ko           |
| Plugin Facebook | 9           | 150 ko | On va retirer ce plugin pour simplement garder un lien vers notre page.                                                                                                                                     | 0                 | 0 ko           |
| Images          | 5           | 2 Mo   | On va garder les 5 images mais on devrait pouvoir largement diminuer la taille. Il faudra mettre un outil d’optimisation d’image automatique. | 5                 | 500 ko         |
| TOTAL           | 33          | 2,4 Mo |                                                                                                                                                                                                           | 9                 | 505 ko         |

Si on réalise tous les objectifs on devrait donc arriver à une page avec un très bon ecodindex avec seulement 9 requêtes et 505ko. De quoi nous garantir une note de A, avec une consommation d’eau de l’ordre de 1.8 cl et un bilan carbone de 1,2 gCO2eq par visite.

## Plan d'actions

|                               Action                              |      Gain     | Difficulté | Priorité |
|:-----------------------------------------------------------------:|:-------------:|:----------:|:--------:|
| Retirer le plugin Facebook                                        | 9 req 150 ko  | 1/5        | 1        |
| Retirer les fonts                                                 | 3 req         | 1/5        | 2        |
| Optimiser les images statiques                                    | 700 ko        | 2/5        | 3        |
| Passer par icomoon pour les icônes                                | 100 ko        | 2/5        | 4        |
| Retirer l’ensemble du javascript hors angular                     | 5 req         | 2/5        | 5        |
| Remplacer bootstrap par pure CSS                                  | 100 ko        | 4/5        | 6        |
| Retirer Angular JS                                                | 100 ko        | 4/5        | 6        |
| Rassembler et minifier l’ensemble de CSS                          | 7 req         | 1/5        | 7        |
| Mettre en place un outil pour optimiser les images des spectacles | 800 ko        | 5/5        | 8        |
| Remplacer angular par une solution type Hugo ou Jeykill           | 100ko         | 5/5        | 9       |

## Mise en oeuvre

### Quick wins

Dans un premier temps, les 5 premiers points par ordre de priorité ont été traités. Il s'agit de petites améliorations efficaces et très rapides à faire. On est loin d'une réelle réécriture avec une heure de travail effectif. Mais les améliorations sont déjà notables.

Vous pouvez voir le résultat {% include link.html text=" des quick-wins sur cette adresse (temporaire)" link="https://diabolos-nantes-octobre-2023.netlify.app/" external=true %}.

On passe de
- 33 à 13 requêtes, malgré l’ajout d’un outil d’analytics (+2 requêtes).
- 2.4 Mo à 1.2 Mo, alors qu’une seule image a été améliorée.
- 109 à 94 éléments dans le DOM. Même si ce n’était pas un objectif, le DOM a été légèrement simplifié.

Nous avons déjà atteint un ecoindex A (83.98/100)

Il est à noter, qu'on perd quelques effets de style :
- la barre header reste rose (pas d’animation avec changement de couleur)
- j’ai retiré le menu qui nécessitait du javascript pour une utilité peu évidente.
- les fonts sont plus classiques
- la seule icône a été remplacée par du texte
- le plugin Facebook est remplacé par un lien

J’estime ces effets secondaires par rapport aux gains. On peut même les considérer bénéfiques dans le sens où ces artifices ne viennent pas parasiter le contenu.

Dans les prochaines étapes, certains points nécessitent une réécriture. C’est une démarche bien plus lourde qui s’annonce pour un gain moins important. Il reste encore pas mal de gain à prendre au niveau des images, on peut largement diviser par deux la taille de la page.
On va aller au bout de la démarche, mais à ce stade, il serait légitime de ne se concentrer que sur l’optimisation des images (action avec la priorité 8).

### Réécriture

Les tâches restantes demandent un effort important. Au point qu'il me semble plus rapide de me lancer dans une réécriture complète. Il me faudra une petite journée de travail effectif.

Vous pouvez voir le résultat {% include link.html text=" de la réécriture sur cette adresse (temporaire)" link="https://diabolos-nantes-novembre-2023.netlify.app/" external=true %}.

Tout n’a pas été conservé dans l’état original, le plus souvent par choix. Mais on reste fidèle à la version précédente. Nous avons également décidé d'ajouter un outil pour suivre la fréquentation du site.

Avant, avec angularJS, la page était construite par le navigateur à chaque visite. Maintenant avec Jekyll, la page est construite seulement quand le contenu est modifié.

On passe de :
- 16 à 10 requêtes mais surtout on passe de 4 domaines à 2 domaines (tout est hébergé sauf l’outil d’analytics…)
- 1149 ko à 166 ko (dû à l’utilisation de librairies plus légères et à la compression des images des spectacles).
- 103 éléments dans e DOM à 74. Encore une fois ce n’était pas le but recherché mais on continue à aller dans la bonne direction. 

L’écoindex est A (90.6 /100)

Cette réécriture améliore pas mal de points de notre site : 
- Les spectacles sont plus lisibles avec des cartes plus grandes
- On peut consulter le détail d’un spectacle
- La mise en ligne de contenu a été largement simplifiée (on passe de la mise à jour d’un fichier JSON à du Markdown)

Je suis assez déçu de ne pas avoir pu mettre en place l’optimisation des images automatiques. Surtout que j’y arrive en local, mais Github ne semble pas prendre en compte le plugin que j’avais mis en place… Il va donc falloir redimensionner les images manuellement à chaque mise à jour…

## Conclusion

On va se projeter à périmètre constant, donc je retire les requêtes liées à l’analytics. Si je reprends le tableau des objectifs : 

|                 |   Avant  |        | Objectif |        | Résultats |        |
|-----------------|:--------:|:------:|:--------:|:------:|:---------:|:------:|
|    Catégorie    | Requêtes | Poids  | Requêtes | Poids  |  Requêtes | Poids  |
| Index.html      | 1        | 2,9 ko | 1        | 1,5 ko | 1         | 2.5 ko |
| CSS             | 8        | 33 ko  | 2        | 10 ko  | 1         | 7.1 ko |
| Font            | 4        | 152 ko | 1        | 3 ko   | 0         | 0 ko   |
| Javascript      | 6        | 112 ko | 0        | 0 ko   | 0         | 0 ko   |
| Plugin Facebook | 9        | 150 ko | 0        | 0 ko   | 0         | 0 ko   |
| Images          | 5        | 2 Mo   | 5        | 500 ko | 5         | 153 ko |
| TOTAL           | 33       | 2,4 Mo | 9        | 505 ko | 7         | 163 ko |

On a donc largement atteint les objectifs pour un site qui garde une apparence très proche. La page est maintenant 7 fois plus légère et nécessite 5 fois moins de requêtes.

![Graphique présentant la diminutaion de la taille de la page d'accueil du site des Diabolos Nantes](/assets/img/posts/2023/Q4/optimisation_DN.webp){:loading="lazy"}

On voit aussi que le travail technique s’arrête là. Maintenant, les images pèsent presque la totalité du poids de la page. Pour alléger, il faut diminuer la taille ou le nombre d'images.

Il faut toutefois nuancer les résultats. Il s’agit ici d’un exercice à but de sensibilisation et de formation. Mais la faible affluence sur le site de ma troupe d’improvisation ne justifie pas le travail d’optimisation effectué. Il faudra plusieurs années pour que la consommation de mon ordinateur et des services utilisés pendant cette réécriture soit rentabilisée.
