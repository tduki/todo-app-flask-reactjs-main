# TP Docker - Application Todo List

## Structure de la stack

Ce projet est une stack web complète comprenant :
- **Frontend** : Application React, servie avec Nginx (port 3000).
- **Backend** : API Flask (port 5000).
- **Base de données** : MySQL 8 (port 3306).
- **PHPMyAdmin** : Interface d'administration MySQL (port 8080).
- **Reverse Proxy** : Nginx configuré comme proxy pour le frontend et le backend (port 80).

---

## Prérequis

Avant de commencer, assurez-vous d'avoir installé sur votre machine :
- **Docker** : [Télécharger Docker](https://www.docker.com/products/docker-desktop)
- **Docker Compose** : Inclus dans Docker Desktop ou téléchargeable séparément.

---

## Instructions d'installation

### 1. Cloner le dépôt
Clonez le dépôt GitHub contenant les fichiers nécessaires au projet :
```bash
git clone <URL_REPO>
cd <REPO>

Puis lancer depuis le repertoire courant de votre projet: 

docker-compose up --build


