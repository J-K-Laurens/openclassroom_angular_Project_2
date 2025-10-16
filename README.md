# Application des Jeux Olympiques

Cette application Angular permet de visualiser et d'analyser les données des Jeux Olympiques pour différents pays. Elle affiche les statistiques et l'évolution des médailles au fil des années.

## Fonctionnalités

- Vue d'ensemble des pays participants avec un graphique en camembert (pie)
- Page détaillée pour chaque pays montrant :
  - Nombre total de participations
  - Nombre total de médailles
  - Nombre total d'athlètes
  - Graphique linéaire de l'évolution des médailles
- Gestion des erreurs et navigation intuitive
- Design responsive

## Prérequis

- Node.js (version recommandée : 14.x ou supérieure)
- npm (installé avec Node.js)
- Angular CLI (version 18.0.3)

## Installation

1. Clonez le repository :
```bash
git clone https://github.com/J-K-Laurens/openclassroom_angular_Project_2.git
```

2. Installez les dépendances :
```bash
npm install
```

## Lancement de l'application

1. Pour démarrer le serveur de développement :
```bash
ng serve
```

2. Ouvrez votre navigateur et accédez à :
```
http://localhost:4200
```

L'application se rechargera automatiquement si vous modifiez les fichiers sources.

## Structure du projet

L'application est organisée comme suit :

- `src/app/core/` : Logique métier
  - `models/` : Interfaces TypeScript
  - `services/` : Services de l'application
- `src/app/pages/` : Composants de pages
  - `home/` : Page d'accueil avec le graphique en camembert (pie)
  - `detail/` : Page de détail d'un pays
  - `not-found/` : Page d'erreur 404
- `src/assets/` : Ressources statiques
  - `mock/` : Données JSON des Jeux Olympiques

## Build

Pour créer une version de production :
```bash
ng build
```

Les fichiers de build seront stockés dans le dossier `dist/`.

## Gestion des erreurs

L'application gère différents cas d'erreur :
- Paramètres d'URL invalides
- Pays non trouvé
- Problèmes de connexion
- Données manquantes ou incorrectes

## Technologies utilisées

- Angular 18.0.3
- Chart.js pour les visualisations
- TypeScript
- SCSS pour le styling
