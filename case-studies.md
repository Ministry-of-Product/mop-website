---
layout: default
title: Case Studies
description: Real examples of judgment through decisions when scaling with AI-enabled systems.
permalink: /case-studies/
meta_description: Case studies demonstrating judgment through decisions. Real examples of how sequencing matters when scaling with AI.
---

# Case Studies

Real examples of judgment through decisions. These aren't success stories—they're situations where sequencing made the difference.

## Structure

Each case study focuses on:
- **The Situation** — What the business was trying to scale
- **The Decision** — What actually mattered
- **The Sequence** — What order things happened in
- **The Outcome** — What happened, and what should have happened

The goal is to demonstrate judgment, not just results.

## Recent Case Studies

{% assign case_studies = site.posts | where_exp: "post", "post.categories contains 'case-studies'" | sort: "date" | reverse %}
{% for post in case_studies limit: 10 %}
### [{{ post.title }}]({{ post.url }})

{% if post.excerpt %}{{ post.excerpt | strip_html }}{% endif %}

{% if post.categories %}{% assign cats = post.categories | join: ", " %}{% endif %}
**Categories:** {% if cats %}{{ cats }}{% else %}—{% endif %}

[Read more →]({{ post.url }})

---

{% endfor %}

{% if case_studies.size == 0 %}
*No case studies yet. Check back soon.*

Want to see your situation featured? [Get in touch](/advisory).
{% endif %}

