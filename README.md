## Welcome to lockg

### Tags

<ul>
  {% for tag in site.tags %}
    <li>
		<a href="/tag/{{ tag[0] }}/">{{ tag[0] }}</a>
		{{ tag[1] | size}}
		{% if tag[1].size == 1 %}
			post
		{% else %}
			posts
		{% endif %}
    </li>
  {% endfor %}
</ul>

### Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
	  <p>{{ post.date | date_to_long_string }}</p>
	  <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
