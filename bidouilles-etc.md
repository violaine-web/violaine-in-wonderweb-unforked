---
layout: page
tartampions: 
  - Nataël
  - Bernard
  - Stéphane
---

## Ceci est une page de bidouilles, comme son nom l'indique !  
<!-- pour faire une boucle !-->
{% for tartampion in page.tartampions %}

Bonjour {{tartampion}}

{% endfor %}
<!-- ci-dessous ça ne marche pas ! -->
{{posts}}

<!-- ci-dessous cette fois-ci ça marche ! -->
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>