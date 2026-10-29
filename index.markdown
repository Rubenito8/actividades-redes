---
layout: default
title: Inicio
---

# Bienvenido a mi Blog
Este blog ha sido creado como parte de la actividad práctica de la asignatura. Aquí se publicaran las entradas:

<div class="home">
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
      </li>
    {% endfor %}
  </ul>
</div>

<!-- Script de Modo Claro/Oscuro -->
{% include dark-mode.html %}