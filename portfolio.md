---
layout: default
title: about me

---

 <section id="portfolio" class="help">
    <h2>Latest articles</h2>
    <ul>
      {% for post in site.posts  %}
    <li>
      <a href="{{ site.baseurl }}{{ post.url }}"><h3>{{ post.title }}</h3></a><a class="ptn"> </a>
       {% if post.thumbnail %}
        <img src="{{ post.thumbnail | relative_url }}" alt="{{ post.title }} Header Image" class="thumbnail">
    {% if post.image_description %}
            <p>{{ post.image_description }}</p>
          {% else %}
            <p>Keine Beschreibung verfügbar.</p>
          {% endif %}
   
      {% endif %} 
   </li>
  {% endfor %}
</ul>
  </section>