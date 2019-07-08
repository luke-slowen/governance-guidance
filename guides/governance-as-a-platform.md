---
category: Governance as a Platform
expires: 2020-01-01
---

# What is Governance as a Platform?

Governance as a Platform (GaaP) is a collection of ideas, patterns and practical
advice that everyone in the public sector can use to improve their governance.

Each guide is structured in 3 sections:

1. **You need this when...** to help people identify which governance tools are needed and when
2. **Things to think about are...** to help people think critically about the issue they’re facing
3. **Here are some great examples you could use...** providing a library of tools, grounded in real cases/examples

## Try out the guides

{% assign guides = site.pages
  | where: "guide", true
  | group_by: "category" %}

{% for guide_group in guides %}
{% if guide_group.name == "Governance as a Platform" %}
{% for guide in guide_group.items %}
- [{{ guide.title }}]({{ guide.url | relative_url }})
{% endfor %}
{% endif %}
{% endfor %}
