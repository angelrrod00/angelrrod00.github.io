---
title: "Engineering"
permalink: /engineering/
layout: archive
author_profile: true
---

Invention. Things that went from an idea thing, to a drawing thing, to a physical thing (or a granted claim!): CAD, milling, circuitry, high voltage, and the patent system.

---
{% assign entries = site.categories["Engineering"] %}
{% if entries %}{% for post in entries %}{% include archive-single.html %}{% endfor %}
{% else %}*Posts in this effort are on the way.*
{% endif %}
