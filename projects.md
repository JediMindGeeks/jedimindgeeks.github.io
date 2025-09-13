---
layout: default
title: "Projets"
description: "Découvrez mes projets techniques et réalisations dans le développement web"
---

<div class="projects-hero">
  <div class="container">
    <h1>Mes projets</h1>
    <p class="lead">Une sélection de projets qui illustrent mon expertise et ma passion pour le développement web.</p>
  </div>
</div>

<section class="projects-content">
  <div class="container">
    <div class="projects-grid">
      {% for project in site.projects %}
      <div class="project-card">
        {% if project.image %}
        <div class="project-image">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" loading="lazy" decoding="async">
        </div>
        {% endif %}
        <div class="project-content">
          <h3>{{ project.title }}</h3>
          <p class="project-description">{{ project.description }}</p>
          <div class="project-tech">
            {% for tech in project.technologies %}
            <span class="tech-tag">{{ tech }}</span>
            {% endfor %}
          </div>
          <div class="project-links">
            {% if project.github %}
            <a href="{{ project.github }}" target="_blank" rel="noopener" class="btn btn-outline">
              <i class="icon-github"></i> Code
            </a>
            {% endif %}
            {% if project.demo %}
            <a href="{{ project.demo }}" target="_blank" rel="noopener" class="btn btn-primary">
              <i class="icon-external"></i> Demo
            </a>
            {% endif %}
          </div>
        </div>
      </div>
      {% endfor %}
    </div>
    
    {% if site.projects.size == 0 %}
    <div class="empty-state">
      <h3>Aucun projet disponible</h3>
      <p>Les projets seront bientôt ajoutés. Revenez plus tard !</p>
    </div>
    {% endif %}
  </div>
</section>
