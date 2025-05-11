# Surveillance des Conteneurs avec Prometheus, Grafana et cAdvisor

Ce projet met en place une infrastructure de surveillance des conteneurs Docker à l'aide de Prometheus pour la collecte des métriques, cAdvisor pour la collecte des données des conteneurs et Grafana pour la visualisation des métriques.

##Prérequis

* Docker
* Docker Compose
* WSL (Windows Subsystem for Linux) pour les utilisateurs Windows

##Structure des fichiers

* `docker-compose.yml` : Décrit les services Docker (Prometheus, cAdvisor, Grafana, Nginx)
* `prometheus.yml` : Configuration des cibles à surveiller par Prometheus

##Installation

1. Clonez ce dépôt :

   ```bash
   git clone <URL_DU_REPO>
   cd monitoring-project
   ```

2. Assurez-vous que Docker est en cours d'exécution.

3. Lancer les services :

   ```bash
   sudo docker-compose up -d
   ```

##Accéder aux interfaces

* **cAdvisor** : `http://localhost:8081`
* **Prometheus** : `http://localhost:9090`
* **Grafana** : `http://localhost:3000`

##Arrêter les services

Pour arrêter tous les services :

```bash
sudo docker-compose down
```

##Auteur

Projet réalisé par MAZIH Bouchra
Contact : mazihbouchra@gmail.com

