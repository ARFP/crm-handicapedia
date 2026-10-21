# Projet Handicapedia - Cahier des charges

## 1. Présentation du projet

> Slogan : **Votre guide vers une meilleure compréhension du handicap**

### Contexte

Handicapedia est un portail web destiné à centraliser de l'information fiable, accessible et actualisée sur les différents types de handicaps.

Le site s'adresse à un public varié :

- Professionnels de la formation
- Référents handicap
- Formateurs
- Apprenants et stagiaires en situation de handicap
- Familles et aidants
- Grand public

L'objectif est de proposer des fiches descriptives claires, des ressources utiles, des actualités et un espace d'échange communautaire.

---

## 2. Objectifs

### Objectifs principaux

- Informer sur les différents handicaps.
- Faciliter l'accès à des ressources fiables.
- Sensibiliser à l'inclusion.
- Favoriser les échanges entre membres de la communauté.
- Proposer un contenu accessible à tous.

### Objectifs secondaires

- Constituer une base documentaire évolutive.
- Diffuser des actualités liées au handicap.
- Créer une communauté d'entraide et de partage.

---

## 3. Solution technique

### CMS

Le site sera développé avec :

- WordPress (dernière version stable)
- Thème responsive compatible RGAA
- Hébergement mutualisé ou VPS

---

## 4. Arborescence fonctionnelle

### Accueil

Présentation du projet :

- Mission du portail
- Dernières actualités
- Dernières fiches handicap
- Accès rapide aux ressources principales

### Actualités

Utilisation du système natif de publications WordPress.

Contenus :

- Actualités réglementaires
- Événements
- Innovations
- Témoignages
- Ressources institutionnelles

### Fiches Handicap

Création d'un **Custom Post Type (CPT) `handicap`**.

Chaque fiche contiendra :

#### Informations générales

- Nom du handicap
- Catégorie
- Définition
- Description détaillée

#### Caractéristiques

- Manifestations courantes
- Impacts possibles dans la vie quotidienne
- Impacts possibles en formation
- Difficultés fréquemment rencontrées

#### Bonnes pratiques

- Aménagements recommandés
- Conseils pour les professionnels
- Conseils pour l'entourage

#### Ressources

- Organismes spécialisés
- Associations
- Sites institutionnels
- Documentation complémentaire

#### Métadonnées

- Date de création
- Date de mise à jour
- Auteur

---

## 5. Recherche

Mise en place d'un moteur de recherche permettant :

- Recherche par mot-clé
- Recherche dans les fiches handicap
- Recherche dans les actualités

Possibilité d'ajouter ultérieurement :

- Filtrage par catégorie
- Filtrage par public concerné

---

## 6. Espace communautaire

### Objectif

Permettre aux utilisateurs d'échanger et de partager leurs expériences.

### Fonctionnalités attendues

- Création de sujets
- Réponses aux discussions
- Modération
- Signalement de contenu
- Gestion des profils utilisateurs

### Authentification

Les comptes WordPress doivent être réutilisés pour le forum.

#### Solution recommandée

**bbPress**

Avantages :

- Plugin officiel de l'écosystème WordPress
- Utilise les comptes WordPress existants
- Gestion native des rôles utilisateurs
- Léger et simple à administrer
- Compatible avec la majorité des thèmes

#### Alternatives

- Asgaros Forum
- wpForo

**Préconisation : bbPress**, suffisante pour la V1 du projet.

---

## 7. Gestion des utilisateurs

### Visiteurs

- Consultation libre du contenu

### Membres

- Participation au forum
- Gestion de leur profil

### Modérateurs

- Modération des discussions
- Gestion des signalements

### Administrateurs

- Gestion complète du site
- Gestion des fiches handicap
- Gestion des actualités
- Gestion des utilisateurs

---

## 8. Accessibilité

L'accessibilité constitue un objectif majeur du projet.

### Exigences

- Navigation clavier
- Contrastes renforcés
- Responsive mobile / tablette
- Compatibilité lecteurs d'écran
- Structure HTML sémantique
- Textes rédigés en langage clair

### Référentiel

- RGAA 4.x
- WCAG 2.2 niveau AA

---

## 9. Commentaires

Les commentaires WordPress seront désactivés :

- Sur les actualités
- Sur les fiches handicap

Les échanges devront se faire exclusivement dans le forum.

---

## 10. Administration

### Gestion des fiches handicap

Interface simplifiée permettant :

- Ajouter une fiche
- Modifier une fiche
- Archiver une fiche
- Ajouter des ressources associées

### Gestion des actualités

Utilisation de l'interface native WordPress.

---

## 11. Évolutions futures

- Annuaire des organismes spécialisés
- Carte géographique des structures d'accompagnement
- Bibliothèque documentaire
- Podcasts et vidéos
- Newsletter
- Espace ressources pour les organismes de formation
- Système de favoris
- Version multilingue

---

# Livrables V1

## Front-office

- Page d'accueil
- Actualités
- Liste des fiches handicap
- Fiche handicap détaillée
- Recherche
- Forum communautaire
- Gestion des comptes utilisateurs

## Back-office

- CPT Handicap
- Gestion des catégories de handicap
- Gestion des ressources associées
- Gestion des actualités
- Gestion du forum
- Gestion des utilisateurs

## Plugins envisagés

- Custom Post Type UI
- Advanced Custom Fields (ACF)
- bbPress
- SEO (Rank Math ou Yoast)
- WP Mail SMTP
- Wordfence Security
- UpdraftPlus Backup