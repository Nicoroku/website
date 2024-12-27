---
layout: default
---

<html lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Nicoroku</title>
</head>
<body>
<main>
  <section id="about" class="section">
    <h2>Welcome to the personal website and blog of Nico Ackermann. </h2>
    <p>Publishing works and articles on pipe smoking, self-improvement, tech, lifelong learning, and more. </p>
  </section>

  <section id="portfolio" class="help">
    <h2>Recent articles</h2>
    <ul>
  {% for post in site.posts limit:3 %}
    <li>
      <a class="ap" href="{{ site.baseurl}} {{ post.url }}"><h3>{{ post.title }}</h3></a><a class="ptn"> </a>
       {% if post.thumbnail %}
        <img src="{{ post.thumbnail | relative_url }}" alt="{{ post.title }} Header Image" class="thumbnail">
     {% if post.image_description %}
            <p>{{ post.image_description }}</p>
          {% else %}
            <p>no description</p>
          {% endif %}
     
      {% endif %} 
   </li>
  {% endfor %}
</ul>
  </section>
 </main>
</body>
</html>