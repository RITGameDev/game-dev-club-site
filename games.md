---
layout: default
---

# Student Games Showcase

Check out some of the content that our students have made! 

Do you have a game that you want to see on our club page? Just make a PR to your website with your new post info! You can do this here: [https://github.com/RITGameDev/game-dev-club-site](https://github.com/RITGameDev/game-dev-club-site)

<div id="posts">
  <h1>Games</h1>

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
