---
title: Jester
layout: role
alignment: neutral
enabled: no
description: must get themselves lynched to win, has no abilities
---

The Jester wins if and only if they die by being lynched by town. If they are killed by mafia, vigilante, or clumsy vigilante, then they have lost since it is now impossible for them to get lynched.

{% capture interactions %}
Detective > Jester;
Detective returns "Innocent";
Neutral roles show up as innocent to the detective;
{% endcapture %}
{% include interactions.html content=interactions %}
