## Welcome to lockg

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
