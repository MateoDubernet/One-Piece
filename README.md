# Projet Fullstack One Piece (Angular & Spring)

## Contexte
Ce projet a été réalisé durant mon alternance dans le but de me former aux frameworks Angular et Spring. Il s'agit d'une application complète permettant de gérer des équipages et des membres, tout en incluant une interface interactive.

L'architecture se compose de deux parties :
- Client (Front-end) : Développé avec Angular et TypeScript, il communique avec le serveur via des requêtes HTTP pour l'affichage et la gestion des données.

- Serveur (Back-end) : Développé avec Spring (Java), il gère la persistance des données via une API REST et une base de données PostgreSQL.

---

## Prérequis
### Client (Front-end)
- Node.js & npm
- Angular CLI (npm install -g @angular/cli)

### Serveur (Back-end)
- Java 11 (Amazon Corretto 11 recommandé)
- PostgreSQL
- IntelliJ IDEA (ou autre IDE compatible)

---

## Installation et Lancement
### 1. Clonage des dépôts
1. Cloner le client :
```bash
    git clone https://github.com/MateoDubernet/One-Piece-Client.git
```

2. Cloner le serveur :
```bash
    git clone https://github.com/MateoDubernet/One-Piece-Server.git
```

### 2. Configuration du Serveur (Back-end)
1. Base de données : Créez une base de données nommée one_piece dans PostgreSQL.
2. Configuration : Dans src/main/resources/application.properties, remplacez les valeurs de connexion par les vôtres.
3. IDE : Ouvrez le projet dans IntelliJ, configurez le SDK sur Corretto 11 et créez une configuration "Application" pointant sur la classe com.example.demo.DemoApplication.

### 3. Configuration du Client (Front-end)
1. Accédez au dossier : cd One-Piece-Client.
2. Installez les dépendances : npm install --force.
3. Lancez l'application : ng serve.
4. Ouvrez votre navigateur à l'adresse : http://localhost:4200.

---

## Fonctionnalités de l'application
L'interface dispose d'une barre de navigation avec trois sections principales

1. Navire : Un mini-jeu interactif sur un quadrillage. En cliquant sur le navire, vous pouvez le déplacer à l'aide des flèches directionnelles du clavier.

2. Crew (Équipages) : Un tableau listant les différents équipages. Cette section permet la création et la modification des groupes.

3. Member (Membres) : Un tableau listant les membres. Note : Il est nécessaire d'avoir créé au moins un équipage avant de pouvoir ajouter un membre.
