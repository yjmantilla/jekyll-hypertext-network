---
title: Directories # you may put the course name here
---

<ul>
   {% for item in site.data.dirs-list%}
      <li><a href="{{ item.link }}">{{ item.title }}</a></li>
   {% endfor %}
</ul>
