---
title: Actions de réduction de l'empreinte environnementale
short_title: Réduction
description: Des opération effectives avec une prise de recul pour mesurer l'impact réel
layout: service
long_description: Application du plan d'actions. Formation des équipes. Pilotage et suivi des tâches. Mesure de l'amélioration effective.
order: 4
icon_utf8: 🚧
icon: people_icon
grid_sizes: --medium:33%; --large:20%;

---

## Plan d'actions en main

Après une [Analyse du Cycle de vie](/services/analyse_cycle_vie.html), nous avons établi un [plan d'actions](/services/strategie_reduction.md) pour réduire l'empreinte environnementale. Nous assurons le suivi de ce plan d'action, mais nous pouvons également intervenir directement sur plusieurs points.

## Formations

Voici quelques formations proposées :

| Nom | Type | Durée | Nombre de participant.e.s |
|-----|------|-------|---------------------------|
{% for formation in site.formations %}| [{{ formation.title }}]({{formation.url}}) | {{formation.type}} | {{ formation.duration}} | {{ formation.effectif }} |
{% endfor %}

N'hésitez pas à nous solliciter pour qu'on créer une formation sur-mesure en fonction de vos besoins.

## Eco-conception des services

Dans la création de votre service ou de votre produit, il est important de penser à l'impact environnemental. 
Nous pouvons vous accompagner dans la démarche d'éco-conception que ce soit à la création du service ou pour un produit utilisé par des millions d'utilisateurs.
Nous suivrons les bonnes pratiques référencées :
- {% include link.html text="Référentiel général d'écoconception de services numériques (RGESN)" link="https://ecoresponsable.numerique.gouv.fr/publications/referentiel-general-ecoconception/" external=true %} proposée par la mission interministérielle "Numérique écoresponsable"
- {% include link.html link="https://collectif.greenit.fr/ecoconception-web/115-bonnes-pratiques-eco-conception_web.html" text="Les 115 bonnes pratiques pour une conecption responsables des services numérique" external=true %} du collectif GreenIT

Pour garantir que votre service propose le meilleur sans user l'environnement.

## Optimisation de site vitrine

Avoir un site internet pour promouvoir ses services et produit, c'est primordial. Mais souvent ces sites sont réalisés sans réfléchir à leur impact environnemental.

Vous ne savez pas où se situe votre site ? Je vous invite à faire le test par vous-même directement sur le site {% include link.html text="Eco-Index de GreenIT" link="https://www.ecoindex.fr/" external=true %}.

Un site vitrine devrait pouvoir atteindre l'Eco-Index A. Si vous êtes en dessous, n'hésitez pas à nous [contacter](/contact.html) pour en discuter.

## Réduction des usages cloud

On touche un point intéressant ou la démarche environnementale peut permettre des économies financières. En effet, quelques paramétrages bien pensés peuvent permettre de réduire la facture en même temps que l'impact environnemental :
- mise en place d'autoscaling
- ajustement de la taille des serveurs à la demande effective
- coupure des environnements non production la nuit
- changement de localisation
- révision de la politique de sauvegarde

## Coaching agile

Pour améliorer l'efficacité des équipes techniques, nous pouvons organiser du coaching agile. L'idée est de guider les équipes à travers les méthodologies agiles telles que le Scrum, Kanban ou encore SAFe.

- stimuler la collaboration
- accroitre l'efficacité opérationnelle
- favoriser la culture d'amélioration continue

## Chef de projet

Le rôle d'un chef de projet est crucial pour intégrer les principes de durabilité et de respect de l'environnement dans le processus de développement d'un produit ou d'un service.

Il est responsable de la planification, de la coordination et de la mise en œuvre des projets en veillant à ce que les meilleures pratiques d'éco-conception soient appliquées à chaque étape. Pour créer des solutions durables qui répondent aux besoins tout en préservant l'environnement.

---
# Intéressé.e ? Prenons contact !
{% include contact_form.html %}
