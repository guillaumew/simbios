---
title: Déclaration d'accessibilité
description: Cette déclaration s'applique au site Simbios.fr
layout: markdown
permalink: accessibilite
published : true
toc: true
---

## État de conformité

La conformité avec le référentiel {% include link.html text="RGAA" link="https://accessibilite.numerique.gouv.fr/" %} n'a pas encore pu être vérifiée. Ce sera un audit intéressant à mener mais qui semble un peu hors d'atteinte pour un site comme celui de Simbios.

Toutefois l'accessibilité de Simbios est testée avec des outils qui automatisent les différentes vérifications :
- Extention Firefox {% include link.html text="Tanaguru" link="https://www.tanaguru.com/" %} ;
- {% include link.html text="Wave" link="https://wave.webaim.org/" %}.

## Résultats des tests

Voici la liste des problèmes remontés.

### Incohérence entre le titre d'un lien et l'intitulé visible

Dans la timeline, on peut voir que l'avant projet possède un lien dont le titre est cadrage et financement. L'outil pense qu'il s'agit d'une incohéhence, mais l'avant-projet chez moi correspond au cadrage et au financement du projet.

Il s'agit donc à mon sens d'un faux positif.

### Incohérence entre le nom accessible et l'intitulé visible

Le logo en haut à gauche comporte un lien qui permet de revenir sur la page d'accueil. Il s'agit d'une pratique courante qui à mon sens ne nécessite pas d'être explicitée.

En revanche, j'ai mentionné explicitement ce fonctionnement dans le nom accessible du lien ("retour à la page d'accueil"). L'outil y voit une incohérence, mais je pense qu'il s'agit encore d'un faux positif.


## Établissement de cette déclaration d’accessibilité

- Cette déclaration a été établie en juillet 2024.
- Elle a été mise à jour en octobre 2024 (correction d'un problème)


## Technologies utilisées pour la réalisation du site

- Jekyll
- Sass ;
- HTML 5 ;
- CSS 3 ;
- Javascript.

## Environnement de test

Les vérifications de restitution de contenus ont été réalisées sur la base d’une combinaison fournie par la base de référence du RGAA, avec les versions suivantes :
- Orca
- Firefox

## Pages du site ayant fait l’objet de la vérification de conformité

Pour le moment seuls les tests de certaines pages ont été formalisés. L'idée est, à terme, de tester une page par structure de page existante.

- [https://simbios.fr](/)
- [https://simbios.fr/blog/](/blog/)
- [https://simbios.fr/contact](/contact)

## Retour d’information et contact

Si vous constatez un défaut d’accessibilité vous empêchant d’accéder à un contenu ou une fonctionnalité du site, merci de bien vouloir le signaler en utilisant [le formulaire de contact](/contact).