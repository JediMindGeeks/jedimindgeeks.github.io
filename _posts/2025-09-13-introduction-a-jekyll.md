---
layout: post
title: "Introduction à Jekyll"
date: 2025-09-13 19:00:00 +0200
categories: [Tutoriels]
tags: [jekyll, static-site, tutorial, web]
author: JediMindGeeks
excerpt: "Découvrez Jekyll, le générateur de site statique qui simplifie la création de blogs et sites web modernes."
---

Jekyll est un générateur de site statique écrit en Ruby qui transforme du texte brut en sites web statiques. Il est particulièrement populaire pour créer des blogs et des sites de documentation.

## Qu'est-ce que Jekyll ?

Jekyll prend du contenu en Markdown, des templates Liquid, et des fichiers CSS/JS, puis génère un site web statique complet. Contrairement aux CMS traditionnels, il n'y a pas de base de données - tout est généré à partir de fichiers.

### Avantages de Jekyll

- **Performance** : Sites statiques ultra-rapides
- **Sécurité** : Pas de base de données à sécuriser
- **Simplicité** : Workflow de développement simple
- **Versioning** : Contenu versionné avec Git
- **Hébergement** : Compatible avec GitHub Pages

## Structure d'un projet Jekyll

```
mon-site/
├── _config.yml      # Configuration
├── _layouts/        # Templates
├── _includes/       # Composants réutilisables
├── _posts/          # Articles de blog
├── _sass/           # Styles SCSS
├── assets/          # Images, CSS, JS
└── index.html       # Page d'accueil
```

## Configuration de base

Le fichier `_config.yml` contient la configuration principale :

```yaml
title: "Mon Site"
description: "Description du site"
baseurl: ""
url: "https://monsite.com"

# Plugins
plugins:
  - jekyll-feed
  - jekyll-sitemap

# Collections
collections:
  posts:
    output: true
    permalink: /:year/:month/:day/:title/
```

## Création d'articles

Les articles se trouvent dans le dossier `_posts/` avec le format :
```
YYYY-MM-DD-titre-de-l-article.md
```

Front matter requis :
```yaml
---
layout: post
title: "Titre de l'article"
date: 2025-09-13 19:00:00 +0200
categories: [Catégorie]
tags: [tag1, tag2]
---
```

## Templates et layouts

Jekyll utilise le système de templates Liquid pour générer le HTML. Les layouts se trouvent dans `_layouts/` et les composants réutilisables dans `_includes/`.

## Conclusion

Jekyll est un excellent choix pour créer des blogs et sites web statiques. Sa simplicité et ses performances en font un outil idéal pour les développeurs qui souhaitent un contrôle total sur leur site.

<!--more-->

## Ressources utiles

- [Documentation officielle Jekyll](https://jekyllrb.com/docs/)
- [Jekyll Themes](https://jekyllthemes.org/)
- [GitHub Pages](https://pages.github.com/)
- [Liquid Template Language](https://shopify.github.io/liquid/)

## Prochaines étapes

Dans le prochain article, nous verrons comment personnaliser un thème Jekyll et ajouter des fonctionnalités avancées.
