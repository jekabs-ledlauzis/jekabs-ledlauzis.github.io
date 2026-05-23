---
layout: default
title: Services
---

# Consulting Services

I offer specialized technical interventions for research institutes, environmental agencies, and engineering teams.

---

{% for service in site.services %}
### {{ service.title }}
{{ service.description }}

[Learn more about this package]({{ service.url | relative_url }})
{% unless forloop.last %}<hr style="border: 0; border-top: 1px dashed var(--border-color); margin: 2rem 0;">{% endunless %}
{% endfor %}