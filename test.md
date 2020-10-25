<ul>
  {% for page in site.pages %}
    <li>
      <a href="{{ page.url }}">{{ page.title }}</a>
      {{ page.excerpt | strip_html | normalize_whitespace | truncate: 160 | escape }}
    </li>
  {% endfor %}
</ul>
