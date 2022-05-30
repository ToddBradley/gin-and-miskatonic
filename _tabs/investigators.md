---
layout: investigator
title: Investigators
icon: fas fa-stream
order: 1
---

# Here are the investigators

{% for investigator in site.investigators %}
* [{{ investigator.name }}]({{ investigator.url }}) - {{ investigator.summary }}

{% endfor %}
