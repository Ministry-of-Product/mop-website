---
layout: default
title: Writing
description: Ongoing trust, pattern recognition, and filtering through writing about AI-enabled systems and decision-making.
permalink: /writing/
meta_description: Writing about decision case analysis, patterns of failure, sequencing, systems thinking, and evaluation frameworks for operators.
---

# Writing

Ongoing trust, pattern recognition, and filtering through writing about AI-enabled systems and decision-making.

## Categories

### [Decision Case Analysis](/writing/decision-case-analysis)

Real situations where decisions about sequencing made the difference.

### [Patterns of Failure](/writing/patterns-of-failure)

Common ways businesses waste effort when scaling with AI.

### [Sequencing & Restraint](/writing/sequencing-restraint)

What to build first, what to ignore, and when to say no.

### [Systems Thinking for Operators](/writing/systems-thinking)

How to think about AI systems as part of a larger business.

### [Evaluation Frameworks](/writing/evaluation-frameworks)

Frameworks for evaluating AI opportunities and experiments.

---

## Recent Posts

{% assign all_posts = site.posts | sort: "date" | reverse %}
{% for post in all_posts limit: 10 %}
### [{{ post.title }}]({{ post.url }})

{% if post.excerpt %}{{ post.excerpt | strip_html }}{% endif %}

{% if post.date %}{{ post.date | date: "%B %d, %Y" }}{% endif %}
{% if post.categories %}{% assign cats = post.categories | join: ", " %} • {{ cats }}{% endif %}

[Read more →]({{ post.url }})

---

{% endfor %}

{% if all_posts.size == 0 %}
*No posts yet. Check back soon.*
{% endif %}

