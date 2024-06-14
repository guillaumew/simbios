---
title: "Le numérique, les yeux fermés"
description: "Mettons-nous dans la peau d'une personne avec un handicap qui la force à utiliser un lecteur d'écran."
tags: ["Numérique responsable", "Cécité", "Clavier", "Accessibilité"]
image: /assets/img/posts/2024/Q2/guillaume-blind-folded.webp
thumb: /assets/img/posts/2024/Q2/guillaume-blind-folded
podcast: https://sphinx.acast.com/p/open/s/65e06335dd3dcf001643bd06/e/665eccf36e20900012d28694/media.mp3
---

Dans un [article précédent](/blog/2023/09/27/numerique_et_handicap), nous avions déjà parlé des différents handicaps qui pouvaient nuire à l'usage d'outils numériques. Je vous y avais alors invité à faire l'expérience d'une navigation web avec handicap sur une {% include link.html link="https://www.atalan.fr/agissons/fr/" text="interface qui simule plusieurs handicaps" %}.

J'ai eu la chance d'aller un cran plus loin grâce à un atelier immersif proposé par l'{% include link.html link="https://aciah-linux.org/" text="ACIAH" %}. L'ACIAH (Accessibilité, Communication, Information, Accompagnement du Handicap) est une association qui a pour objectif d'aider les personnes à accéder aux outils numériques.

Nous allons donc réaliser des opérations très simples avec des contraintes :
- d'abord sans la souris (difficile à utiliser avec certains handicaps moteurs comme la maladie de Parkison)
- puis les yeux fermés (indice : sans la vue, la souris reste inutilisable)

Les opérations simples consistent :
- à lire un mail
- écrire un mail
- rédiger et enregistrer un document
- consulter une page web

Pour faciliter la navigation au clavier, nous allons utiliser un lecteur d'écran ({% include link.html text="Orca" link="https://help.gnome.org/users/orca/stable/index.html.fr" %} dans notre cas). L'ACIAH nous a également proposé sa version de Linux avec des outils permettant de pouvoir utiliser l'ordinateur plus facilement sans écran et sans souris.

Voici quelques-une de mes impressions :

## Où en suis-je ?

Quand on se lance dans une opération, aussi simple soit-elle, il faut toujours garder en tête où nous en sommes. Impossible de se laisser distraire par une conversation ou autre puis de reprendre la tâche là où on l'a laissée. Dans la quasi-totalité des cas, si on perd le fil, il faut recommencer au début.

Et perdre le fil, c'est quelque chose qui arrive assez souvent. Il arrive qu'on se trompe de touche sur le clavier et qu'on lance une mauvaise opération, il arrive qu'on se trompe régulièrement lorsqu'on tape un texte au clavier et qu'on perde ainsi le fil de sa phrase.

## Prendre son temps

Nous sommes habitué.e.s à parcourir un document en diagonale en scrollant frénétiquement pour aller chercher l'information qui nous intéresse. Quand on fonctionne avec uniquement le lecteur d'écran, il faut prendre le temps de parcourir l'ensemble du document avec la voix robotique. Cela prend beaucoup de temps et c'est quelque chose qui m'a souvent frustré.

On comprend d'ailleurs ici l'importance d'avoir une page bien structurée avec des titres de niveau 1,2,3... qui suivent la hiérarchie des informations.

## L'importance de l'agencement du clavier

Sur tout clavier physique vous noterez que les touches **F** et **J** possèdent un petit relief qui permet de les identifier plus facilement. Ce sont les touches sur lesquelles nous sommes censés poser nos index lorsque nous écrivons. C'est subtil pour un voyant, mais c'est indispensable pour un non-voyant ! Le pavé alpha-numérique est très large et il est facile d'y perdre ses repères quand on ne le voit pas.

Les claviers externes ont généralement les touches regroupées en petits pavés. Le pavé des flèches, le pavé numérique, la ligne des boutons fonctions, les 6 touches au-dessus des flèches. Cet agencement permet de plus facilement retrouver les touches que lorsque toutes les touches sont serrées les unes à côtés des autres (comme c'est souvent le cas sur les claviers des ordinateurs portables).

{% responsive_image 
  path: assets/img/posts/2024/Q2/clavier.webp 
  alt: "Un clavier externe classique avec des reliefs sur les touches J et F, ainsi qu'un agencemenet par paquets de touches." 
%}

## Les détails d'interface qui cassent tout

Sur la quasi-totalité des sites internets, la première chose à faire avant de pouvoir les utiliser est d'accepter les cookies. C'est souvent irritant pour l'internaute moyen. Mais lorsqu'on ne peut pas utiliser la souris, cela peut devenir un enfer !

Par exemple, sur un grand site media français, il faut parcourir toute la page pour parvenir enfin aux boutons qui gèrent les cookies. Et la page d'accueil est très longue ! Tant que les cookies ne sont pas acceptés, impossible d'accéder au contenu.

C'est un exemple parmi d'autre, mais on se rend compte qu'on peut avoir fait un gros effort d'accessibilité, parfois une simple petite imprécision peut rendre une interface inutilisable pour une partie des utilisateur.ice.s.

## Les efforts d'accessibilité peuvent servir à tous

Si un site est bien structuré pour être accessible, cela devrait également le rendre plus compréhensible pour l'ensemble des utilisateurs.

D'ailleurs quelques innovations sont nées de volontés de rendre des services plus accessibles comme par exemple le SMS qui a été inventé pour permettre aux personnes mal-entendantes d'utiliser le téléphone ({% include link.html text="source" link="https://fr.wikipedia.org/wiki/Short_Message_Service" %}).

## Pour aller plus loin

Je vous invite vivement à faire l'expérience d'une navigation à l'aveugle à l'aide d'un lecteur d'écran comme {% include link.html text="Orca" link="https://help.gnome.org/users/orca/stable/index.html.fr" %}. Cela permettra de mieux appréhender les barrières rencontrées par certaines personnes.

Sinon, vous pouvez également consulter {% include link.html link="https://www.eig.numerique.gouv.fr/blog/demonstrations-accessibilite-numerique/" text="ces témoignages de personnes en situation de handicap" %} sur leur utilisation de services numériques.

Pour rendre les interfaces plus accessibles, vous avez :
- le {% include link.html text="Référentiel Général d'amélioration de l'accessibilité (RGAA)" link="https://accessibilite.numerique.gouv.fr/" %} qui est obligatoire pour les services publics et grandes entreprises (malheureusement ces organisations préfèrent généralement payer l'amende).
- des outils d'analyse automatiques {% include link.html link="https://www.webaccessibility.com/" text="Web Acessibility" %} ou {% include link.html text="WAVE" link="https://wave.webaim.org/" %}.

Dans un registre "IT for human", je souhaite aussi vous proposer l'application {% include link.html link="https://www.bemyeyes.com/language/french" text="Be My Eyes" %} qui propose à des aveugles de poser des questions à des voyants pour les aider dans la vie de tous les jours.