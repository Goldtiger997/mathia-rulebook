---
title: Godfather
layout: role
alignment: mafia
enabled: no
description: A mafia that doesn't show up as guilty to Detective
---

The Godfather is exactly the same as an Ordinary Mafia except that the detective get's the result "Innocent" when they investigate the Godfather.

Just like the Ordinary Mafia the Godfather can be nominated to perform a kill.

{% capture interactions %}
Godfather > X;
X dies;

---
Detective > Godfather;
Detective returns "Innocent";
{% endcapture %}
{% include interactions.html content=interactions %}
