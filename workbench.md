---
layout: default
title: The Workbench
permalink: /workbench/
description: The Workbench — evergreen explainers on the frameworks and operating models behind how Ministry of Product builds.
meta_description: The Workbench is where Ministry of Product publishes its evergreen explainers — the frameworks, rules, and operating models behind how we build, including BSSS and the Product Path.
---

<span class="eyebrow">Ministry of Product</span>

# The Workbench

The frameworks, rules, and operating models behind how we build — written down so they can be learned, used, and built on. Not a blog; these are evergreen references, not news.

<div class="wb-list">
{% assign docs = site.workbench | sort: "order" %}
{% for doc in docs %}
  <a class="wb-card" href="{{ doc.url }}">
    <h3>{{ doc.title }}</h3>
    <p>{{ doc.summary }}</p>
    <span class="wb-more">Read →</span>
  </a>
{% endfor %}
</div>
