---
layout: default
title: List of Recipes
---

{% for recipes in site.my_recipes %}


<a href="{{ recipes.url | prepend: site.baseurl }}">
        <h2>{{ recipes.title }}</h2>
</a>

<p class="post-excerpt">{{ recipes.description | truncate: 160 }}</p>

{% endfor %}      
