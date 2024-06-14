---
title: Graphs

_graphs: # start with _ to ignore the filter for this attribute
  - link: ./../graphs/knowledge-graph-subdirs.html
    title: Graph with Categories
  - link: ./../graphs/knowledge-graph.html
    title: Graph without Categories
---

<ul>
   {% for item in page.ignoreFilter_graphs %}
      <li><a href="{{ item.link }}">{{ item.title }}</a></li>
   {% endfor %}
</ul>
