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

Il cible de manière large l'ensemble des personnes souhaitant réduire l'impact environnemental de leurs activités numériques que ces dernières soient personnelles ou professionnelles. Il propose également des ressources utiles à des fins pédagogiques pour l'éducation et la formation.

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

> Simbios obtient la note **88 / 100**.
{: .prompt-tip }

### RGESN

Un diagnostic de ce site avec le {% include link.html text="RGESN" link="https://ecoresponsable.numerique.gouv.fr/publications/referentiel-general-ecoconception/" %} a été réalisé en février 2025. Il s'agit d'une auto-évaluation. 

> Simbios obtient le score de **95 %**.
{: .prompt-tip }

| Thématique      | Score |
|-----------------|-------|
| Statégie        | 100 % |
| Spécifications  |  89 % |
| Architecture    |  86 % |
| UI / UX         |  94 % |
| Contenus        |  88 % |
| Frontend        | 100 % |
| Hébergement     | 100 % |
| Algorithmie     | 100 % |

Le rapport est disponible [ici](/assets/img/declarations/rgesn_2025_simbios.pdf){:target="new-page"}

## Configuration minimale requise pour accéder au site

Le site doit pouvoir être consulté sur l'ensemble des terminaux existants. Il existe toutefois une trop grande variété pour réaliser des tests exhaustifs. Le site Simbios est testé sur les configurations suivantes :
- Windows XP Firefox 52
- Lubuntu 24.04, Firefox dernière version
- Android 10, Chrome dernière version
- Lubuntu 24.04, Chromium dernière version
- Windows 7, Edge 109

Les pages lègères (entre 10 et 135 ko) permettent d'être chargées rapidement dès la 3G. Le site fonctionne correctement en 2G si cette dernière est stable.

Les différentes tailles d'écran sont supportées. Tests réalisé de 320px de large à 2 500 px.

## Améliorations identifiées

Engagements à réaliser :

- formaliser une stratégie de maintenance et de décommissionnement
- optimiser les transferts lors des mises à jour du site
- mettre une validation côté client pour le formulaire de contact
- écrire une stratégie d'archivage et de suppression des contenus

Anomalies à corriger :
- Sur Windows XP, les certificats posent un problèmes. Le site est fonctionnels uniquement sur Firefox.
- Sur certains devices, les icones types "Ouvrir dans un nouvel onglet" s'affichent mal.