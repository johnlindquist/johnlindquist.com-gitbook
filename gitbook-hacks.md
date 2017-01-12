Open `~/.gitbook/versions/3.2.2/node_modules/gitbook-plugin-theme-default`


Delete from `page.html`:
```
            {% block book_navigation %}
                {% if page.previous and page.previous.path %}
                <a href="{{ page.previous.path|resolveFile }}{{ page.previous.anchor }}" class="navigation navigation-prev {% if not (page.next and page.next.path) %}navigation-unique{% endif %}" aria-label="Previous page: {{ page.previous.title }}">
                    <i class="fa fa-angle-left"></i>
                </a>
                {% endif %}
                {% if page.next and page.next.path %}
                <a href="{{ page.next.path|resolveFile }}{{ page.next.anchor }}" class="navigation navigation-next {% if not (page.previous and page.previous.path) %}navigation-unique{% endif %}" aria-label="Next page: {{ page.next.title }}">
                    <i class="fa fa-angle-right"></i>
                </a>
                {% endif %}
            {% endblock %}
```

Change "Published by Gitbook" in `summary.html`:
```
    <li>
        <a href="https://www.gitbook.com" target="blank" class="gitbook-link">
            {{ "GITBOOK_LINK"|t }}
        </a>
    </li>
```