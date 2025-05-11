
# Book Catalog Microservices

Ce projet met en place une architecture microservices basée sur Spring Boot pour la gestion d’un catalogue de livres avec configuration centralisée, découverte de services, Kafka, PostgreSQL, etc.

## 📦 Structure du projet

```
book-catalog-microservices/
│
├── discovery-service/         # Service Eureka pour la découverte
├── config-service/            # Spring Cloud Config Server
├── book-service/              # Gestion des livres
├── user-service/              # Gestion des utilisateurs
├── analytics-service/         # Consommation des événements Kafka
├── docker-compose.yml         # Conteneurisation avec Docker
├── init-multiple-dbs.sh       # Script pour initialiser les bases PostgreSQL
└── config-repo/               # Répertoire local des configs
```

## 🚀 Démarrage rapide

1. **Cloner le projet** et se placer dans le dossier racine :
    ```bash
    cd book-catalog-microservices
    ```

2. **Configurer les fichiers de configuration** dans `~/config-repo/` :
    - `book-service.properties`
    - `user-service.properties`
    - `analytics-service.properties`

3. **Vérifier que Docker est installé** puis lancer :
    ```bash
    docker-compose up --build
    ```

4. **Démarrer chaque microservice** via IntelliJ (clic droit sur chaque projet Spring Boot > Run).

## 🛠 Technologies utilisées

- Spring Boot (Spring Cloud, Eureka, Config Server, Kafka)
- PostgreSQL
- Apache Kafka
- Docker & Docker Compose
- Maven

## 📝 Auteur

Projet réalisé dans le cadre du module JEE (Teknolabs)
