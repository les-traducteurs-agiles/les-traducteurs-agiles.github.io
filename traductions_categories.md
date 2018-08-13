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
{% assign rawtags = "" %}
{% for post in site.posts %}
    {% assign ctags = post.tags | join:'|' | append:'|' %}
    {% assign rawtags = rawtags | append:ctags %}
{% endfor %}
{% assign rawtags = rawtags | split:'|' | sort %}

{% comment %}
=======================
The following part removes dulpicated tags and invalid tags like blank tag.
=======================
{% endcomment %}
{% assign tags = "" %}
{% for tag in rawtags %}
    {% if tag != "" %}
        {% if tags == "" %}
            {% assign tags = tag | split:'|' %}
        {% endif %}
        {% unless tags contains tag %}
            {% assign tags = tags | join:'|' | append:'|' | append:tag | split:'|' %}
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
{% for tag in tags %}
  <a href="#{{ tag | slugify }}" style="font-size:125%"> {{ tag }} &nbsp; </a>
{% endfor %}
</div>

&nbsp;  

---


{% comment %}
=======================
The purpose of this snippet is to list all your posts posted with a certain tag.
=======================
{% endcomment %}


{% for tag in tags %}
  &nbsp;
  <h1 id="{{ tag | slugify }}"> {{ tag }} &nbsp;  
    <a class="post-meta" href="#top" title="retour vers le nuage de mots des catégories">⤴︎</a>
  </h1>
  <ul class="post-list">
  {% for post in site.posts %}
    {% if post.tags contains tag %}
    <li>
      <h2>
        <a class="post-link" href="{{ post.url }}"> {{ post.title }} </a>
      </h2>
    </li>
    {% endif %}
  {% endfor %}
  </ul>
{% endfor %}
