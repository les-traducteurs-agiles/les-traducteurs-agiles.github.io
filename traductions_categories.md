---
layout: page
title: Traductions par catégories
permalink: /traductions_categories/
---
<ul class="post-list">
  <h1>Scrum</h1>
  <li>
    {% for post in site.categories.scrum %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>XP</h1>
  <li>
    {% for post in site.categories.xp %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Kanban</h1>
  <li>
    {% for post in site.categories.kanban %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Équipe</h1>
  <li>
    {% for post in site.categories.equipe %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Scrum Master</h1>
  <li>
    {% for post in site.categories.scrum-master %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Product Owner</h1>
  <li>
    {% for post in site.categories.product-owner %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Outils</h1>
  <li>
    {% for post in site.categories.outil %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Estimation</h1>
  <li>
    {% for post in site.categories.estimation %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Conception</h1>
  <li>
    {% for post in site.categories.conception %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Test</h1>
  <li>
    {% for post in site.categories.test %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Refactoring</h1>
  <li>
    {% for post in site.categories.refactoring %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>TDD</h1>
  <li>
    {% for post in site.categories.tdd %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Backlog</h1>
  <li>
    {% for post in site.categories.backlog %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Pratique</h1>
  <li>
    {% for post in site.categories.pratique %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Artefact</h1>
  <li>
    {% for post in site.categories.artefact %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Manifeste</h1>
  <li>
    {% for post in site.categories.manifeste %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Fiches</h1>
  <li>
    {% for post in site.categories.fiche %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>(mini)Livres</h1>
  <li>
    {% for post in site.categories.livre %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Inspirations</h1>
  <li>
    {% for post in site.categories.inspiration %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>

<ul class="post-list">
  <h1>Organisations</h1>
  <li>
    {% for post in site.categories.organisation %}
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    {% endfor %}
  </li>
</ul>