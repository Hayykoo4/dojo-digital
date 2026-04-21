# Dojo Digital 🥋

Blog éditorial moderne sur les sports de combat : MMA, Judo, Jujitsu/BJJ et Lutte.

## 🚀 Démarrage rapide

### Prérequis

- Ruby (version 2.7 ou supérieure)
- Bundler (`gem install bundler`)

### Installation

1. Clonez le repository :
```bash
git clone https://github.com/votre-username/dojo-digital.git
cd dojo-digital
```

2. Installez les dépendances :
```bash
bundle install
```

3. Lancez le serveur de développement :
```bash
bundle exec jekyll serve
```

4. Ouvrez votre navigateur à l'adresse : `http://localhost:4000`

## 📁 Structure du projet

```
dojo-digital/
├── _config.yml          # Configuration Jekyll
├── _includes/           # Composants réutilisables
│   ├── head.html        # Balises <head> (meta, CSS, etc.)
│   ├── header.html      # En-tête avec navigation
│   ├── footer.html      # Pied de page
│   ├── scripts.html     # JavaScript
│   ├── post-card.html   # Carte d'article
│   └── share-buttons.html # Boutons de partage
├── _layouts/            # Templates de page
│   ├── default.html     # Layout de base
│   ├── home.html        # Page d'accueil
│   ├── post.html        # Page d'article
│   ├── page.html        # Pages simples
│   └── category.html    # Pages de catégorie
├── _posts/              # Articles du blog
├── assets/
│   └── css/
│       └── style.css    # Styles CSS
├── index.md             # Page d'accueil
├── judo.md              # Page catégorie Judo
├── mma.md               # Page catégorie MMA
├── jujitsu.md           # Page catégorie Jujitsu
├── lutte.md             # Page catégorie Lutte
├── a-propos.md          # Page À propos
├── contact.md           # Page Contact
└── Gemfile              # Dépendances Ruby
```

## ✍️ Ajouter un nouvel article

Créez un fichier dans `_posts/` avec le format : `YYYY-MM-DD-titre-de-larticle.md`

### Front matter obligatoire

```yaml
---
layout: post
title: "Titre de votre article"
date: 2026-03-30
category: mma  # ou judo, jujitsu, lutte
description: "Description courte pour le SEO"
---
```

### Front matter optionnel

```yaml
---
author: Votre Nom
tags: [tag1, tag2, tag3]
image: /assets/images/mon-image.jpg
type: futur_evenement  # ou evenement_passe, decouverte
event_date: 2026-04-15  # Pour les événements
---
```

### Types d'articles spéciaux (pour la page d'accueil)

1. **`type: futur_evenement`** + `event_date` : Affiché dans "Événements à venir"
2. **`type: evenement_passe`** + `event_date` : Affiché dans "Événements passés"
3. **`type: decouverte`** : Affiché aléatoirement dans "À découvrir aujourd'hui"

## 🎨 Personnalisation

### Couleurs

Modifiez les variables CSS dans `assets/css/style.css` :

```css
:root {
  --color-primary: #dc2626;    /* Rouge principal */
  --color-judo: #2563eb;       /* Bleu judo */
  --color-mma: #dc2626;        /* Rouge MMA */
  --color-jujitsu: #7c3aed;    /* Violet jujitsu */
  --color-lutte: #059669;      /* Vert lutte */
}
```

### Configuration site

Éditez `_config.yml` pour modifier :
- Titre et description du site
- Liens réseaux sociaux
- Navigation principale
- Descriptions des catégories

## 🌐 Déploiement sur GitHub Pages

1. Poussez votre code sur GitHub
2. Allez dans Settings > Pages
3. Sélectionnez la branche `main` et le dossier `/ (root)`
4. Votre site sera disponible à `https://username.github.io/dojo-digital/`

### Configuration pour GitHub Pages

Si votre site est dans un sous-dossier, modifiez `_config.yml` :

```yaml
baseurl: "/dojo-digital"
url: "https://username.github.io"
```

## 📱 Fonctionnalités

- ✅ Design responsive (mobile-first)
- ✅ SEO optimisé (meta tags, Open Graph)
- ✅ Flux RSS automatique
- ✅ 4 catégories de sports de combat
- ✅ Section "Gros Titres" dynamique
- ✅ Boutons de partage (X, Facebook, copie)
- ✅ Navigation mobile
- ✅ Compatible GitHub Pages

## 📄 License

MIT License - Utilisez librement ce template !

---

Fait avec ❤️ pour les passionnés de sports de combat.
