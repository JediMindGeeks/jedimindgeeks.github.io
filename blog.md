---
layout: default
title: "Blog"
description: "Articles techniques, tutoriels et réflexions sur le développement web"
---

<div class="blog-hero">
  <div class="container">
    <h1>Blog</h1>
    <p class="lead">Articles techniques, tutoriels et réflexions sur le développement web et les technologies.</p>
  </div>
  </div>

<section class="blog-content">
  <div class="container">
    {% if site.posts.size > 0 %}
    <div class="posts-list">
      {% for post in site.posts %}
      <article class="post-item">
        <div class="post-item-content">
          <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
          <div class="post-meta">
            <time datetime="{{ post.date | date_to_xmlschema }}">
              {{ post.date | date: "%d %B %Y" }}
            </time>
            {% if post.author %}
            <span>par {{ post.author }}</span>
            {% endif %}
            {% if post.categories %}
            <div class="post-categories">
              {% for category in post.categories %}
              <span class="category-tag">{{ category }}</span>
              {% endfor %}
            </div>
            {% endif %}
          </div>
          <p>{{ post.excerpt | strip_html | truncate: 200 }}</p>
          <div class="post-tags">
            {% for tag in post.tags %}
            <span class="tag">{{ tag }}</span>
            {% endfor %}
          </div>
          <a href="{{ post.url | relative_url }}" class="read-more">Lire la suite</a>
        </div>
      </article>
      {% endfor %}
    </div>

    {% else %}
    <div class="empty-state">
      <h3>Aucun article disponible</h3>
      <p>Les articles seront bientôt publiés. Revenez plus tard !</p>
    </div>
    {% endif %}
  </div>
</section>

<style>
.blog-hero {
  background: linear-gradient(135deg, var(--primary-color) 0%, color-mix(in srgb, var(--primary-color) 80%, black) 100%);
  color: white;
  padding: 3rem 0;
  text-align: center;
}

.posts-list {
  display: grid;
  gap: 2rem;
  margin-bottom: 3rem;
}

.post-item {
  background: white;
  border: 1px solid var(--border-color);
  border-radius: var(--border-radius-lg);
  padding: 2rem;
  transition: var(--transition);
}

.post-item:hover {
  transform: translateY(-4px);
  box-shadow: var(--shadow-lg);
}

.post-item h2 {
  margin-bottom: 1rem;
}

.post-item h2 a {
  color: var(--text-color);
  text-decoration: none;
}

.post-item h2 a:hover {
  color: var(--primary-color);
}

.post-meta {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  align-items: center;
  margin-bottom: 1rem;
  font-size: 0.9rem;
  color: var(--text-light);
}

.post-categories {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
}

.category-tag {
  background: var(--primary-color);
  color: white;
  padding: 0.25rem 0.5rem;
  border-radius: 0.25rem;
  font-size: 0.8rem;
}

.post-tags {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
  margin: 1rem 0;
}

.tag {
  background: var(--bg-light);
  color: var(--text-light);
  padding: 0.25rem 0.5rem;
  border-radius: 0.25rem;
  font-size: 0.8rem;
}

.read-more {
  color: var(--primary-color);
  font-weight: 500;
  text-decoration: none;
}

.read-more:hover {
  text-decoration: underline;
}

.empty-state {
  text-align: center;
  padding: 4rem 2rem;
  color: var(--text-light);
}

@media (max-width: 768px) {
  .post-item {
    padding: 1.5rem;
  }
}
</style>

