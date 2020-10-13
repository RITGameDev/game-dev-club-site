---
layout: default
---

# Club Presentations

Check out our club presentations as well as follow up resources and challenges

<div id="posts">
  {% for post in site.categories.resources %}
    <a href="{{ site.url }}{{ post.url }}"><h2>{{ post.title }}</h2></a>
    <p class="post-meta">
      <time class="dt-published" datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        {{ post.date | date: date_format }}
      </time></p>
    <p> {{ post.excerpt }} </p>
    <hr>
  {% endfor %}

</div> <!-- End Posts -->
