---
title: "Science"
permalink: /science/
layout: archive
author_profile: true
---

Research and teaching. Most of this is cyber-physical systems security. Plus the work that taught me how I learn.

---
{% assign entries = site.categories["Science"] %}
{% if entries %}{% for post in entries %}{% include archive-single.html %}{% endfor %}
{% else %}*Posts in this effort are on the way.*
{% endif %}
