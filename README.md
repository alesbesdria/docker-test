# Application WordPress Docker

Cette application WordPress utilise Docker et Docker Compose pour déployer un environnement WordPress avec une base de données MySQL.

## Prérequis

- Docker installé sur votre machine.
- Docker Compose installé sur votre machine.

## Structure du projet

project/
├── compose.yml
├── .env
├── config/
│   ├── nginx/
│   │   └── nginx.conf
│   └── php/
│       └── php.ini
├── src/
│   ├── app/
│   │   └── (contenu de l'application)
│   └── Dockerfile
└── .gitignore

# Projet Wordpress avec Docker Compose

Ce projet utilise Docker Compose pour exécuter une application Wordpress avec une base de données MySQL. Les informations sensibles, telles que les mots de passe, sont stockées de manière sécurisée à l'aide des secrets Docker Compose.

## Prérequis

- Docker et Docker Compose installés.

## Configuration des secrets

1. Crée les fichiers `db_password.txt` et `db_root_password.txt` dans le répertoire racine du projet.
2. Remplis chaque fichier avec le mot de passe approprié pour la base de données.
3. Docker Compose injecte ces secrets dans les conteneurs au démarrage.

## Lancer l'application

1. Cloner le dépôt :
   ```bash
   git clone <url-du-dépôt>
