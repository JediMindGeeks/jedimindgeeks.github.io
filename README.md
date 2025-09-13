# Site Web JediMindGeeks

Site web personnel et portfolio technique construit avec Jekyll et hébergé sur GitHub Pages.

## Fonctionnalités

- Blog : articles techniques et tutoriels
- Portfolio : présentation des projets
- Design responsive : optimisé pour tous les appareils
- SEO optimisé : meta tags et sitemap automatiques
- Performance : site statique rapide et léger

## Technologies utilisées

- Jekyll 4.3.x
- Sass pour le CSS
- JavaScript vanilla
- GitHub Pages pour l’hébergement

## Installation locale

1. Clonez le dépôt :
```bash
git clone https://github.com/jedimindgeeks/jedimindgeeks.github.io.git
cd jedimindgeeks.github.io
```

2. Installez les dépendances :
```bash
bundle install
```

3. Lancez le serveur de développement :
```bash
bundle exec jekyll serve --livereload
```

4. Ouvrez votre navigateur sur `http://localhost:4000`

## Structure du projet

```
├── _config.yml          # Configuration Jekyll
├── _layouts/            # Gabarits de pages
├── _includes/           # Fragments réutilisables
├── _sass/               # Styles Sass (partials)
├── _posts/              # Articles de blog
├── _projects/           # Projets du portfolio
├── assets/              # Images, CSS, JS
├── index.html           # Page d’accueil
└── README.md            # Ce fichier
```

## Personnalisation

### Couleurs
Modifiez les variables dans `_sass/_variables.scss` :
```scss
$primary-color: #2563eb;
$secondary-color: #64748b;
// ...
```

### Contenu
- Articles : ajoutez des fichiers Markdown dans `_posts/`
- Projets : ajoutez des fichiers Markdown dans `_projects/`
- Pages : créez des fichiers HTML/Markdown à la racine

## Écriture d’articles

Créez un nouveau fichier dans `_posts/` avec le format :
```
YYYY-MM-DD-titre-de-l-article.md
```

Front matter requis :
```yaml
---
layout: post
title: "Titre de l'article"
date: 2025-09-13 18:00:00 +0200
categories: [Catégorie]
tags: [tag1, tag2]
author: JediMindGeeks
---
```

## Déploiement

Le site se déploie automatiquement sur GitHub Pages à chaque push sur la branche `main`.

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## Contribution

Les contributions sont les bienvenues ! N’hésitez pas à :
- Signaler des bugs
- Proposer des améliorations
- Soumettre des pull requests

## Contact

- Email : contact@jedimindgeeks.com
- GitHub : [@jedimindgeeks](https://github.com/jedimindgeeks)
- LinkedIn : [JediMindGeeks](https://linkedin.com/in/jedimindgeeks)
