---
layout: page
title: Home
---

# Bem-vindo ao meu espaço de aprendizado!

Este site é dedicado a documentar minha evolução na programação e no desenvolvimento web. Sinta-se à vontade para explorar meus projetos e registros.

---

<div style="display: flex; flex-wrap: wrap; gap: 40px; margin-top: 40px; border-top: 1px solid #eee; padding-top: 20px;">

  <div style="max-width: 300px; flex: 1; min-width: 250px;">
    <h3 style="font-size: 1.2em;">Últimas Postagens</h3>
    <ul style="list-style: none; padding: 0; font-size: 0.9em;">
      {% for post in site.posts limit:5 %}
        <li style="margin-bottom: 10px;">
          <a href="{{ post.url }}" style="text-decoration: none; color: #2a7ae2;">{{ post.title }}</a>
        </li>
      {% endfor %}
    </ul>
    <a href="/blog/" style="font-size: 0.8em; color: #828282;">Ver tudo →</a>
  </div>

  <div style="flex: 2; min-width: 280px;">
    <h3 style="font-size: 1.2em;">Sobre o Site</h3>
    <p style="color: #555; line-height: 1.6;">
      {{ site.description }}
    </p>
  </div>

</div>
