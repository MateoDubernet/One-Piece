# Projet Fullstack One Piece (Angular & Spring)

## Présentation
Ce projet a été réalisé durant mon alternance pour approfondir mes compétences sur les frameworks **Angular** et **Spring Boot**. Il s'agit d'une application complète permettant de gérer des équipages et des membres, incluant une interface interactive et un mini-jeu.

### Architecture :
- **Front-end** : Angular & TypeScript (Interface interactive et gestion d'état).
- **Back-end** : Spring Boot (API REST, Java 11).
- **Base de données** : PostgreSQL (Persistance des données).
- **Infrastructure** : Docker & Docker Compose.

---

## Installation et Lancement
### 1. Clonage du dépôt
```bash
    git clone https://github.com/MateoDubernet/service-worker.git
```

### 2. Lancement (Docker)
**Prérequis :** [Docker Desktop](https://www.docker.com/products/docker-desktop) installé et lancé.

```bash
    cd ./one-piece
    docker-compose up --build
```

### 3. Accès
- Interface Client : http://localhost (Port 80)
- API Backend : http://localhost:8080

[!IMPORTANT]
Assurez-vous que les ports 80 et 8080 ne sont pas déjà utilisés par une autre application sur votre machine avant de lancer le conteneur.

---

## Fonctionnement du Système
L'interface dispose d'une barre de navigation avec trois sections principales

1. Navire : Un mini-jeu interactif sur un quadrillage. En cliquant sur le navire, vous pouvez le déplacer à l'aide des flèches directionnelles du clavier.

2. Crew (Équipages) : Un tableau listant les différents équipages. Cette section permet la création et la modification des groupes.

3. Member (Membres) : Un tableau listant les membres. Note : Il est nécessaire d'avoir créé au moins un équipage avant de pouvoir ajouter un membre.
