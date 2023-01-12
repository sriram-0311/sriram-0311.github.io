---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% assign show_preprints = false %}
{% for post in site.publications reversed %}
  {% if post.status == "in review" %}
    {% assign show_preprints = true %}
  {% endif %}
{% endfor %}

{% if show_preprints %}
