---
layout: default
---

{% for park in site.data.d %}
  <h2>{{ park.park }}</h2>
  Established: <b>{{ "now" | date: "%Y" | minus: park.established }} years ago</b>
{% endfor %}

{% for post in site.posts %}
  <a href="{{ post.url }}"><h2>{{ post.title }}</h2></a>
{% endfor %}