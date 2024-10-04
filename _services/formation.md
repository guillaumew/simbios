---
title: Formation
short_title: Formation
description: Apprendre pour mieux gérer les actions de réductions de l'impact environnemental
layout: service
long_description: Apprendre pour mieux gérer les actions de réductions de l'impact environnemental
order: 4
icon_utf8: 🎓
icon: graduation_hat_icon
grid_sizes: --small:100%; --medium:50%; --large:33%;

---

Voici quelques exemples de formations proposées :

| Nom | Type | Durée | Nombre de participant.e.s |
|-----|------|-------|---------------------------|
{% for formation in site.formations %}| [{{ formation.title }}]({{formation.url}}) | {{formation.type}} | {{ formation.duration}} | {{ formation.effectif }} |
{% endfor %}

N'hésitez pas à nous solliciter pour qu'on créer une formation sur-mesure en fonction de vos besoins.