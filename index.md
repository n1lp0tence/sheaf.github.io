---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
author_profile: true
permalink: /
redirect_from:
  - /about/
  - /about.html
---

Hi, I’m Qiwu. I write about **pure mathematics** and **philosophy**.

## Latest blog posts
<ul>
  {% for post in site.posts limit:6 %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## Papers
<ul>
  {% assign ps = site.papers | sort: "date" | reverse %}
  {% for p in ps limit:6 %}
    <li><a href="{{ p.url | relative_url }}">{{ p.title }}</a></li>
  {% endfor %}
</ul>

## Notes
<ul>
  {% assign ns = site.notes | sort: "date" | reverse %}
  {% for n in ns limit:6 %}
    <li><a href="{{ n.url | relative_url }}">{{ n.title }}</a></li>
  {% endfor %}
</ul>