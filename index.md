---
layout: default
---
# Welcome to My Website
Hello there! Welcome to my site! My name is Minsoo Im.
I am currently in a winter semester working as an undergraduate research intern while taking a course on Neural Networks.
[Check out my GitHub Profile](https://github.com/min-5214)
---
## My Posts
<ul>
  {% for post in site.posts %}
    <li>
      <span style="color: gray; font-size: 0.9em;">{{ post.date | date: "%b %d, %Y" }}</span>
      
      <a href="{{ post.url | relative_url }}">
        <strong>{{ post.title }}</strong>
      </a>

      {% if post.tags %}
        <br>
        <small><i>Tags: {{ post.tags | join: ', ' }}</i></small>
      {% endif %}
    </li>
  {% endfor %}
</ul>