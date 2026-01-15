---
layout: default
title: Case Studies
description: Real examples of judgment through decisions when scaling with AI-enabled systems.
permalink: /case-studies/
meta_description: Case studies demonstrating judgment through decisions. Real examples of how sequencing matters when scaling with AI.
---

# Case Studies

Real examples of judgment through decisions. These aren't success stories—they're situations where sequencing made the difference.


## Recent Case Studies

<div class="case-studies-grid">
{% assign case_studies = site.posts | where_exp: "post", "post.categories contains 'case-studies'" | sort: "date" | reverse %}
{% for post in case_studies %}
  <div class="case-study-card">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    {% if post.excerpt %}
    <p class="case-study-excerpt">{{ post.excerpt | strip_html }}</p>
    {% endif %}
    <a href="{{ post.url }}" class="case-study-link">Read more →</a>
  </div>
{% endfor %}
</div>

{% if case_studies.size == 0 %}
*No case studies yet. Check back soon.*

Want to see your situation featured? [Get in touch](/advisory).
{% endif %}

