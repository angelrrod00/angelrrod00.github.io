---
title: "Music"
permalink: /music/
layout: archive
author_profile: true
---

Music is where I practice letting a thing become itself. Production, synthesis, sequencing

---
{% assign entries = site.categories["Music"] %}
{% if entries %}{% for post in entries %}{% include archive-single.html %}{% endfor %}
{% else %}*Posts in this effort are on the way.*
{% endif %}
