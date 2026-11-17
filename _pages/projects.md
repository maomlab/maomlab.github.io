---
title: "Maom Lab - Projects"
layout: textlay
excerpt: "Maom Lab: Research projects"
sitemap: false
permalink: /projects/
---
# Projects
<div class="row projects-row">
{% assign sorted_projects = site.projects | sort: "order" %}{% for p in sorted_projects %}{% include project_card.html project=p %}{% endfor %}
</div>
