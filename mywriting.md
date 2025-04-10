{% assign posts = site.data.bloomberg.items %}
<ul class="bloomberg-columns">
  {% for post in posts %}
    <li>
      <a href="{{ post.link }}" target="_blank">{{ post.title }}</a><br/>
      <small>{{ post.pubDate | date: "%B %-d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
