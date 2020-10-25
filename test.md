<ul>
  {% for page in site.pages %}
    <li>
      <a href="{{ page.url }}">{{ page.title }}</a>
      {{ page.content | strip_html | truncatewords:75 }}
    </li>
  {% endfor %}
</ul>

{% for page in site.pages %}
  {% if page.categories contains 'messages' %}
    <div class="item">
      <h3><a href="{{ page.url }}">
        {{ page.title }}
      </a></h3>

      <p>{{page.description}}</p>
    </div>
  {% endif %}
{% endfor %}
