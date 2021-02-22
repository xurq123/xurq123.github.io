---
layout: page
permalink: /readings/
title: 资料
description: Readings about theorem proving.
nav: true
---
### Official
{% for items in site.data.tutorials.official%}
* <a class="page-link" href="{{items.link}}"> {{items.name}} </a>
{% endfor %}

### Tutorials/Books

{% for item in site.data.tutorials.books_tutorials%}
#### {{item.name}}
{% for reading in item.readings%}
{% if reading.authors %}
* {{reading.authors}}: <a class="page-link" href="{{reading.url}}">{{reading.name}}</a>
{% else %}
* <a class="page-link" href="{{reading.url}}">{{reading.name}}</a>
{% endif %}
{% endfor %}
{% endfor %}

### Courses
{% for course in site.data.tutorials.courses %}
* <a class="page-link" href="{{course.url}}">{{course.name}}</a>
{% endfor %}

### Websites
{% for site in site.data.tutorials.websites %}
* <a class="page-link" href="{{site.url}}">{{site.name}}</a>
{% endfor %}

### Groups
{% for group in site.data.tutorials.groups%}
* <a class="page-link" href="{{group.url}}">{{group.name}}</a>
{% endfor %}

### Competitions
{% for competition in site.data.tutorials.competitions%}
* <a class="page-link" href="{{competition.url}}">{{competition.name}}</a>
{% endfor %}