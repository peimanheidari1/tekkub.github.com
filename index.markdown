---
layout: default
---

<article>
  <ul id="posts">
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url }}">{{ post.title | xml_escape }}</a>
        <span>{{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</article>
