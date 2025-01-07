---
title: Training
short_title: Training
class: formation
description: Learning in order to be more efficient in your actions to reduce your impact
layout: service
long_description: Learning in order to be more efficient in your actions to reduce your impact
order: 4
icon_utf8: 🎓
icon: graduation_hat_icon
grid_sizes: --small:100%; --medium:50%; --large:33%;
lang: en
locale: en_US
permalink: /en/services/training

---

Here are some examples of training offered:

| Name | Type | Duration | Number of trainees |
|-----|------|-------|---------------------------|
{% for formation in site.formations %}| {{ formation.title-en }} | {{formation.type-en}} | {{ formation.duration-en}} | {{ formation.effectif }} |
{% endfor %}

Feel free to contact us so we can create a tailored training program based on your needs.