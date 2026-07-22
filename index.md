{{ site.docs.size }}


<ul>
{% for doc in site.docs %}
  {% if doc.path contains 'docs/' %}
    <li>
      {{ doc.url | relative_url }}
        {{ doc.name | replace: '.md', '' }}
      </a>
    </li>
  {% endif %}
{% endfor %}
</ul>
