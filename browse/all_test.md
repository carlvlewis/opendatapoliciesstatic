---
layout: default
title: List of all open-data policies
---

{% include base.html %}

These are all the open-data policies we have on this site:

<ul>
{% assign docs = site.documents | sort: "place" %}
{% for doc in docs %}
  <li>
    <a href="{{ doc.url }}">1: {% include docname.html doc_page=doc %}; 2: {% include placename.html doc_page=doc %}</a>
  </li>
{% endfor %}
</ul>
