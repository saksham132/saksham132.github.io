<ul>
  {% for item in site.social_links %}
    <li>{{ item.icon }} <a href="{{ item.url }}">{{ item.name }}</a></li>
  {% endfor %}
</ul>
