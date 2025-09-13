---
layout: project
title: "Application React E-commerce"
description: "Application e-commerce moderne développée avec React, Redux et Node.js"
image: "/assets/images/projects/react-ecommerce.jpg"
technologies: ["React", "Redux", "Node.js", "MongoDB", "Stripe", "JWT"]
github: "https://github.com/jedimindgeeks/react-ecommerce"
demo: "https://react-ecommerce-demo.vercel.app"
featured: true
---

## Description du projet

Application e-commerce complète développée avec React et Node.js, incluant un panier d'achat, un système de paiement avec Stripe, et une interface d'administration.

## Fonctionnalités principales

- **Catalogue produits** : Affichage et filtrage des produits
- **Panier d'achat** : Gestion des articles et quantités
- **Paiement sécurisé** : Intégration Stripe pour les transactions
- **Authentification** : Système de connexion/inscription avec JWT
- **Interface admin** : Gestion des produits et commandes
- **Responsive** : Design adaptatif pour tous les appareils

## Technologies utilisées

- **Frontend** : React 18, Redux Toolkit, Material-UI
- **Backend** : Node.js, Express, MongoDB
- **Paiement** : Stripe API
- **Authentification** : JWT, bcrypt
- **Déploiement** : Vercel (frontend), Heroku (backend)

## Architecture technique

### Frontend
- **React Router** : Navigation entre les pages
- **Redux Toolkit** : Gestion d'état globale
- **Material-UI** : Composants d'interface utilisateur
- **Axios** : Communication avec l'API

### Backend
- **Express.js** : Framework web Node.js
- **MongoDB** : Base de données NoSQL
- **Mongoose** : ODM pour MongoDB
- **Stripe** : API de paiement

## Défis techniques

- **Performance** : Optimisation du rendu avec React.memo et useMemo
- **Sécurité** : Validation des données et protection CSRF
- **UX** : Gestion des états de chargement et erreurs
- **Scalabilité** : Architecture modulaire et réutilisable

## Résultats

- Application entièrement fonctionnelle
- Temps de chargement < 2 secondes
- Interface intuitive et moderne
- Code maintenable et documenté
- Tests unitaires et d'intégration
