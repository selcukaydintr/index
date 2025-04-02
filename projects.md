---
layout: page
title: Projeler
permalink: /projects/
---

# Projelerim

Aşağıda geliştirdiğim bazı projelerden örnekler bulabilirsiniz.

<div class="projects-grid">
  {% for project in site.projects %}
    <div class="project-card">
      <div class="project-image">
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
      </div>
      <div class="project-content">
        <h3>{{ project.title }}</h3>
        <p class="project-tags">
          {% for tag in project.tags %}
            <span class="project-tag">{{ tag }}</span>
          {% endfor %}
        </p>
        <p class="project-description">{{ project.excerpt }}</p>
        <div class="project-links">
          {% if project.demo %}
            <a href="{{ project.demo }}" class="btn btn-sm btn-primary" target="_blank">Demo</a>
          {% endif %}
          {% if project.github %}
            <a href="{{ project.github }}" class="btn btn-sm btn-outline-secondary" target="_blank">GitHub</a>
          {% endif %}
          <a href="{{ project.url | relative_url }}" class="btn btn-sm btn-outline-primary">Detaylar</a>
        </div>
      </div>
    </div>
  {% endfor %}
</div>

## Diğer Katkılar

Açık kaynak projelere yaptığım katkılar:

- [Awesome Project](https://github.com/awesome/project) - CSS hata düzeltmeleri
- [Cool Library](https://github.com/cool/library) - Dokümantasyon geliştirme
- [Useful Tool](https://github.com/useful/tool) - Yeni özellik ekleme