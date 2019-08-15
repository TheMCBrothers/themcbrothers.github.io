---
layout: page
title: Useless Mod - Documentation
description: "The official documentation page for the Useless Mod"
in_nav: false
permalink: /docs/uselessmod/
---

Here you can find everything about the useless mod.
Just click on the links below and find out what you need

---

{% assign docs = site.pages | where_exp: "item" , "item.path contains 'docs/uselessmod'"%}
{% for item in docs %}
{% if item.doc_name and item.doc_desc %}
[{{item.doc_name}}]({{item.url | relative_url}}) - {{item.doc_desc}}
{% endif %}
{% endfor %}
