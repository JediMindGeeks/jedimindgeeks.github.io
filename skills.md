---
layout: default
title: "Compétences"
description: "Mes compétences techniques et outils de développement"
---

<div class="skills-hero">
  <div class="container">
    <h1>Mes compétences</h1>
    <p class="lead">Technologies et outils que j'utilise pour créer des solutions modernes et performantes</p>
  </div>
</div>

<section class="skills-content">
  <div class="container">
    <div class="skills-grid">
      <!-- Frontend -->
      <div class="skill-category">
        <div class="skill-header">
          <h2>Frontend</h2>
          <p>Développement d'interfaces utilisateur modernes et interactives</p>
        </div>
        <div class="skill-items">
          <div class="skill-item">
            <div class="skill-name">HTML5</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 95%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">CSS3 / Sass</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 90%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">JavaScript (ES6+)</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 88%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">React</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 85%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">Vue.js</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 80%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">TypeScript</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 82%"></div>
            </div>
          </div>
        </div>
      </div>

      <!-- Backend -->
      <div class="skill-category">
        <div class="skill-header">
          <h2>Backend</h2>
          <p>Développement d'APIs et de services backend robustes</p>
        </div>
        <div class="skill-items">
          <div class="skill-item">
            <div class="skill-name">Node.js</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 87%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">Python</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 85%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">Express.js</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 88%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">FastAPI</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 83%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">Django</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 80%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">PHP / Laravel</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 75%"></div>
            </div>
          </div>
        </div>
      </div>

      <!-- Base de données -->
      <div class="skill-category">
        <div class="skill-header">
          <h2>Base de données</h2>
          <p>Gestion et optimisation des données</p>
        </div>
        <div class="skill-items">
          <div class="skill-item">
            <div class="skill-name">PostgreSQL</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 85%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">MongoDB</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 82%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">MySQL</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 80%"></div>
            </div>
          </div>
        </div>
      </div>

      <!-- DevOps & Outils -->
      <div class="skill-category">
        <div class="skill-header">
          <h2>DevOps & Outils</h2>
          <p>Chaîne d'outils de développement et d'intégration continue</p>
        </div>
        <div class="skill-items">
          <div class="skill-item">
            <div class="skill-name">Docker</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 80%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">Kubernetes</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 68%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">AWS / Azure / GCP</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 70%"></div>
            </div>
          </div>
          <div class="skill-item">
            <div class="skill-name">CI/CD (GitHub Actions)</div>
            <div class="skill-level">
              <div class="skill-bar" style="width: 75%"></div>
            </div>
          </div>
        </div>
      </div>

    </div>
  </div>
</section>

<style>
.skills-hero {
  background: var(--bg-light);
  padding: 3rem 0;
}

.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.skill-category {
  background: white;
  border: 1px solid var(--border-color);
  border-radius: var(--border-radius-lg);
  padding: 2rem;
  transition: var(--transition);
}

.skill-category:hover {
  transform: translateY(-4px);
  box-shadow: var(--shadow-lg);
}

.skill-header {
  margin-bottom: 2rem;
  text-align: center;
}

.skill-header h2 {
  color: var(--primary-color);
  margin-bottom: 0.5rem;
}

.skill-header p {
  color: var(--text-light);
  font-size: 0.9rem;
}

.skill-items {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.skill-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1rem;
}

.skill-name {
  font-weight: 500;
  color: var(--text-color);
  min-width: 120px;
}

.skill-level {
  flex: 1;
  height: 8px;
  background: var(--bg-light);
  border-radius: 4px;
  margin-left: 1rem;
  overflow: hidden;
}

.skill-bar {
  height: 100%;
  background: linear-gradient(90deg, var(--primary-color) 0%, var(--accent-color) 100%);
  border-radius: 4px;
  transition: width 0.3s ease;
}

.certifications {
  margin-top: 4rem;
  padding-top: 2rem;
  border-top: 1px solid var(--border-color);
}

.certifications h2 {
  text-align: center;
  margin-bottom: 2rem;
  color: var(--text-color);
}

.certifications-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
}

.certification-item {
  background: var(--bg-light);
  padding: 1.5rem;
  border-radius: var(--border-radius);
  text-align: center;
  transition: var(--transition);
}

.certification-item:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow-md);
}

.certification-item h3 {
  color: var(--primary-color);
  margin-bottom: 0.5rem;
  font-size: 1.1rem;
}

.certification-item p {
  color: var(--text-light);
  margin-bottom: 0.5rem;
  font-size: 0.9rem;
}

.cert-date {
  background: var(--primary-color);
  color: white;
  padding: 0.25rem 0.5rem;
  border-radius: 0.25rem;
  font-size: 0.8rem;
  font-weight: 500;
}

@media (max-width: 768px) {
  .skills-grid {
    grid-template-columns: 1fr;
  }
  
  .skill-category {
    padding: 1.5rem;
  }
  
  .skill-item {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.5rem;
  }
  
  .skill-level {
    width: 100%;
    margin-left: 0;
  }
}
</style>
