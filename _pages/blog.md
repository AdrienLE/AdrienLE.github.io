---
layout: archive
title: "Blog"
permalink: /blog/
author_profile: true
---

While I plan to import the posts presented here into this website directly, for now this is just a collection of links to various blog posts and other informal publications.

{% include base_path %}

{% for post in site.blog reversed %}
  {% include archive-single.html %}
{% endfor %}
