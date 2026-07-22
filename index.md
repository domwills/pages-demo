<ul>
{% for page in site.pages %}
  {% if page.path contains 'pages/' %}
    <li>
      {{ page.url | relative_url }}
        {{ page.name | replace: '.md', '' }}
      </a>
    </li>
  {% endif %}
{% endfor %}
</ul>
