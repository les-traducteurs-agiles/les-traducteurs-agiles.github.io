---
layout: page
title: Traductions par catégories
permalink: /traductions_categories/
---
{% comment %}
=======================
Trouvé sur https://codinfox.github.io/dev/2015/03/06/use-tags-and-categories-in-your-jekyll-based-github-pages/
The following part extracts all the tags from your posts and sort tags, so that you do not need to manually collect your tags to a place.
=======================
{% endcomment %}
{% assign rawcategories = "" %}
{% for post in site.posts %}
    {% assign ccategories = post.categories | join:'|' | append:'|' %}
    {% assign rawcategories = rawcategories | append:ccategories %}
{% endfor %}
{% assign rawcategories = rawcategories | split:'|' | sort %}

{% comment %}
=======================
The following part removes dulpicated categories and invalid tags like blank tag.
=======================
{% endcomment %}
{% assign categories = "" %}
{% for category in rawcategories %}
    {% if category != "" %}
        {% if categories == "" %}
            {% assign categories = category | split:'|' %}
        {% endif %}
        {% unless categories contains category %}
            {% assign categories = categories | join:'|' | append:'|' | append:category | split:'|' %}
        {% endunless %}
    {% endif %}
{% endfor %}

# <a name="top"></a> Catégories

{% comment %}
=======================
The purpose of this snippet is to list all the tags you have in your site.
=======================
{% endcomment %}
<div>
{% for category in categories %}
  <a href="#{{ category | slugify }}" style="font-size:125%"> {{ category }} &nbsp; </a>
{% endfor %}
</div>

&nbsp;  

---


{% comment %}
=======================
The purpose of this snippet is to list all your posts posted with a certain tag.
=======================
{% endcomment %}


{% for category in categories %}
  &nbsp;
  <h1 id="{{ category | slugify }}"> {{ category }} &nbsp;  
    <a class="post-meta" href="#top" title="retour vers le nuage de mots des catégories">⤴︎</a>
  </h1>
  <ul class="post-list">
  {% for post in site.posts %}
    {% if post.categories contains category %}
    <li>
      <h2>
        <a class="post-link" href="{{ post.url }}"> {{ post.title }} </a>
      </h2>
    </li>
    {% endif %}
  {% endfor %}
  </ul>
{% endfor %}
