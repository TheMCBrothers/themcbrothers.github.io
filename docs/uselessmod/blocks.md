---
layout: page
title: Blocks - Useless Mod - Documentation
doc_name: Blocks
doc_desc: Everything about the useless mod blocks
permalink: /docs/uselessmod/blocks/
---

Here you can find the blocks

<h4>Block List</h4>
<ul>
{%- assign docs = site.pages | where_exp: "item" , "item.path contains 'docs/uselessmod/blocks'" -%}
{%- for item in docs -%}
{%- if item.doc_name and item.doc_desc -%}
[{{item.doc_name}}]({{item.url | relative_url}}) - {{item.doc_desc}}
{%- endif -%}
{%- endfor -%}
