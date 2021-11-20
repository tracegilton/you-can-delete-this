---
layout: default
---

{% for park in site.data.d %}
  <h2>{{ park.park }}</h2>
  Established: <b>{{ "now" | date: "%Y" | minus: park.established }} years ago</b>
{% endfor %}

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
{% endfor %}

<b>Nice to see ya — I've been here since {{ "now" | date: "%c" }} 🆒</b>