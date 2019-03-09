---
layout: default
---


# This is the games page!

Check out some of the content that our students have made! 

<div id="posts">
  <h1>Posts</h1>

  {% for post in site.posts %}
    <a href="{{ site.url }}{{ post.url }}"><h2>{{ post.title }}</h2></a>
    <p class="post-meta">
      <time class="dt-published" datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        {{ post.date | date: date_format }}
      </time></p>
    <p> {{ post.excerpt }} </p>
  {% endfor %}

</div> <!-- End Posts -->
