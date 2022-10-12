---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% comment %} thanks to https://chrirupp.github.io/ for the code to fix the link {% endcomment %}
{% if page.author and site.data.authors[page.author] %}
  {% assign author = site.data.authors[page.author] %}{% else %}{% assign author = site.author %}
{% endif %}

You can also find my articles on <a href="{{author.googlescholar}}">my Google Scholar profile</a>.

{% include base_path %}

{% bibliography %}



