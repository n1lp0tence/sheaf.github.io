---
title: "Papers"
permalink: /papers/
layout: single
---


## Papers

<ul>
{% for entry in site.data.files %}
  {% if entry.type == "paper" %}
    <li>
      <a href="/files/{{ entry.repo }}.pdf">
        {{ entry.repo | replace: "_", " " }}
      </a>
    </li>
  {% endif %}
{% endfor %}
</ul>