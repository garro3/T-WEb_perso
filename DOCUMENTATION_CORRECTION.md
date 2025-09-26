# Documentation pour la Correction - Site Web CacaCar

## Structure générale du projet

### Architecture des fichiers
```
T-WEB_perso/
├── index.html          # Page d'accueil principale
├── catalogue.html      # Page catalogue des voitures
├── product.html        # Page détail produit
├── about.html          # Page à propos
├── contact.html        # Page de contact
├── style.css           # Fichier CSS principal avec tous les styles
├── regle.txt          # Fichier de règles du projet
└── voiture/           # Dossier contenant toutes les ressources
    ├── logo.png       # Logo de l'entreprise
    ├── *.jpg/webp     # Images des voitures (voiture1.jpg à voiture23.jpg)
    └── *.mp4          # Vidéo pour section héros
```

## Technologies utilisées

### Frontend
- **HTML5** : Structure sémantique des pages
- **CSS3** : Styles personnalisés avec variables CSS et flexbox
- **Bootstrap 5.3.8** : Framework CSS pour le responsive et les composants
- **Font Awesome 6.4.0** : Bibliothèque d'icônes pour les réseaux sociaux

### Fonctionnalités implémentées

#### 1. Navigation (Navbar)
- **Navbar fixe** en haut de toutes les pages
- **Logo cliquable** redirigeant vers l'accueil
- **Menu hamburger** pour les écrans mobiles (responsive)
- **Liens de navigation** vers toutes les pages

#### 2. Page d'accueil (index.html)
- **Section héros** avec image de fond et texte centré
- **Section découverte** avec appel à l'action vers le catalogue
- **Section style Shopify** avec texte + galerie d'images 2x2
- **Footer complet** avec 4 colonnes : marque, liens, contact, réseaux sociaux

#### 3. Page catalogue (catalogue.html)
- **Grille responsive** de cartes produits (3 colonnes desktop, 2 tablet, 1 mobile)
- **Cartes personnalisées** avec effet hover et animations CSS
- **Contenu caché** qui apparaît au survol (description produit)
- **Images optimisées** avec object-fit: cover

#### 4. Styles CSS (style.css)
- **Variables CSS** pour la cohérence des couleurs
- **Dégradé de fond** diagonal sur le body
- **Effets hover** sur les cartes avec transforms et box-shadow
- **Transitions fluides** (0.3s) pour tous les effets
- **Section vidéo héros** prête à l'emploi

## Détails techniques

### Responsive Design
- **Mobile First** avec Bootstrap
- **Breakpoints** : 
  - Mobile : col-12
  - Tablet : col-md-6  
  - Desktop : col-lg-4
- **Navbar collapsible** pour mobile

### Accessibilité
- **Attributs alt** sur toutes les images
- **Aria-labels** sur les sections importantes
- **Structure sémantique** HTML5 (header, main, footer, section)
- **Contraste** suffisant entre texte et fond

### Performance
- **CDN** pour Bootstrap et Font Awesome (chargement rapide)
- **Images optimisées** avec différents formats (jpg, webp)
- **CSS minimaliste** et organisé

## Classes CSS principales

### Layout
- `.container` : Conteneurs Bootstrap
- `.row`, `.col-*` : Système de grille Bootstrap

### Composants personnalisés
- `.custom-card` : Cartes avec effets hover
- `.hidden-content` : Contenu révélé au survol
- `.video-hero` : Section héros avec vidéo de fond
- `.video-background` : Vidéo en arrière-plan

### Effets visuels
- `transform: scale(1.05)` : Agrandissement au hover
- `box-shadow` : Ombres portées avec variations
- `border-radius: 15px` : Coins arrondis
- `transition: 0.3s` : Transitions fluides

## Points forts du projet

1. **Code bien commenté** : Chaque section est expliquée
2. **Structure claire** : HTML sémantique et CSS organisé
3. **Responsive design** : Fonctionne sur tous les écrans
4. **Interactions utilisateur** : Effets hover et animations
5. **Cohérence visuelle** : Variables CSS et thème unifié
6. **Accessibilité** : Attributs ARIA et structure sémantique

## Améliorations possibles

- Ajout de JavaScript pour interactivité avancée
- Optimisation des images (lazy loading)
- Mise en place d'un système de filtres sur le catalogue
- Ajout d'un système de panier
- Formulaires de contact fonctionnels