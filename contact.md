---
layout: default
title: "Contact"
description: "Contactez-moi pour discuter de vos projets ou collaborations"
---

<div class="contact-hero">
  <div class="container">
    <h1>Contactez-moi</h1>
    <p class="lead">Une idée de projet ? Une question ? N'hésitez pas à me contacter !</p>
  </div>
</div>

<section class="contact-content">
  <div class="container">
    <div class="contact-grid">
      <div class="contact-info">
        <h2>Informations de contact</h2>
        <div class="contact-item">
          <h3>Email</h3>
          <p><a href="mailto:contact@jedimindgeeks.com">contact@jedimindgeeks.com</a></p>
        </div>
        
        <div class="contact-item">
          <h3>Réseaux sociaux</h3>
          <div class="social-links">
            <a href="https://github.com/jedimindgeeks" target="_blank" rel="noopener">
              <i class="icon-github"></i> GitHub
            </a>
            <a href="https://linkedin.com/in/jedimindgeeks" target="_blank" rel="noopener">
              <i class="icon-linkedin"></i> LinkedIn
            </a>
          </div>
        </div>
        
        <div class="contact-item">
          <h3>Disponibilité</h3>
          <p>Je suis disponible pour des projets freelance et des collaborations. N'hésitez pas à me contacter pour discuter de vos besoins.</p>
        </div>
      </div>
      
      <div class="contact-form">
        <h2>Envoyez-moi un message</h2>
        <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
          <div class="form-group">
            <label for="name">Nom *</label>
            <input type="text" id="name" name="name" required>
          </div>
          
          <div class="form-group">
            <label for="email">Email *</label>
            <input type="email" id="email" name="email" required>
          </div>
          
          <div class="form-group">
            <label for="subject">Sujet *</label>
            <input type="text" id="subject" name="subject" required>
          </div>
          
          <div class="form-group">
            <label for="message">Message *</label>
            <textarea id="message" name="message" rows="5" required></textarea>
          </div>
          
          <button type="submit" class="btn btn-primary">Envoyer le message</button>
        </form>
      </div>
    </div>
  </div>
</section>
