---
layout: default
title:  "Artikel"
date:   2024-11-25 08:40:42 +0100
thumbnail: "assets/sticker02-min.png"
---
<body>
 <div class="post-container">
    <h1>{{ page.title }}</h1>
    {% if page.header_image %}
      <img src="{{ page.header_image }}" alt="{{ page.title }}">
    {% endif %}
    <div class="content">
      {{ content }}
    </div>
  </div>
    
</body>