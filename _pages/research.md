---
layout: archive
permalink: /research/
title: "Research"
author_profile: true
---

{% include base_path %}

## Publications

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

## Working Papers

{% for post in site.working-papers reversed %}
  {% include archive-single.html %}
{% endfor %}
