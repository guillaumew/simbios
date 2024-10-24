---
title: Déclaration d'écoconception
description: Cette déclaration s'applique au site Simbios.fr
layout: markdown
permalink: declaration-ecoconception
published : true
toc: true
---

## Raison d'être de ce service

Le site Simbios.fr a pour vocation de montrer l'ensemble des services proposés par Guillaume Wolf, ainsi que de proposer des articles sur le numérique responsable et sur l'environnement.

Il cible de manière large l'ensemble des personnes souhaitant réduire l'impact environnemental de leurs activités numériques que ces dernières soient personnelles ou professionnelles. Il propose également des ressources utiles à des fins pédagogique pour l'éducation et la formation.

## Stratégie mise en œuvre et objectifs en matière de réduction ou de limitation des impacts environnementaux

Ce site se veut exemplaire par rapport à ce qui peut être réalisé en terme de légerté et de simplicité :
- interface simple pour accéder rapidement à l'information
- il s'agit d'un site statique : aucune base de données et aucun traitement server n'est nécessaire pour afficher les pages
- les pages ne dépassent jamais 150 ko
- les contenus doivent s'adapter à l'écran dès 320 px
- gros effort de compression des images
- limitation de l'usage des animations
- limiter au maximum l'usage de composants externes
- très peu de javascript (analytics et outil de recherche)

## Diagnostic

### EcoIndex

L'ensemble des pages est testé par l'outil EcoIndex. Vous pouvez retrouver les statistiques en bas de page. Toutes les pages possèdent un score d'au moins 80/100. Plus d'informations disponibles sur la page de la [déclaration environnementale](/declaration-environnementale).

### RGESN
Audit à réaliser.

## Configuration minimale requise pour accéder au site

Le site doit pouvoir être consulté sur l'ensemble des terminaux existants. Il existe toutefois une trop grande variété pour réaliser des tests exhaustifs. Le site Simbios est testé sur les configurations suivantes :
- Windows XP Firefox 52
- Lubuntu 24.04, Firefox dernière version
- Android 10, Chrome dernière version
- Lubuntu 24.04, Chromium dernière version
- Windows 7, Edge 109

Les pages lègères entre 10 et 135 ko permettent d'être chargées rapidement dès la 3G. Le site fonctionne correctement en 2G si cette dernière est stable.

Les différentes tailles d'écran sont supportées. Tests réalisé de 320px de large à 2 500 px.

## Améliorations identifiées

- Sur Windows XP, les certificats posent un problèmes. Le site est fonctionnels uniquement sur Firefox.
- Sur certains devices, les icones types "Ouvrir dans un nouvel onglet" s'affichent mal.