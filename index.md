---
layout: default
# title: index
# permalink: index.html
---
<div>
    {% for post in site.posts %}
    <a href="{{ site.url }}{{ post.url }}" class="post-list-item">
        {{ post.title }} -- {{ post.date | date: "%Y-%m-%d" }}
    </a>
    {% endfor %}
</div>