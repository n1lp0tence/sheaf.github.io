---
title: "Notes"
permalink: /notes/
layout: single
---

## Notes

<ul>
{% for entry in site.data.files %}
  {% if entry.type == "notes" %}
    <li>
      <a href="/files/{{ entry.repo }}.pdf">
        {{ entry.repo | replace: "_", " " }}
      </a>
    </li>
  {% endif %}
{% endfor %}
</ul>