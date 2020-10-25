<ul>
  {% for page in site.pages %}
    <li>
      <a href="{{ page.url }}">{{ page.title }}</a>
      {{ page.content | strip_html | truncatewords:75 }}
    </li>
  {% endfor %}
</ul>
