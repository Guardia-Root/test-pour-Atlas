# Guardia Root - Moteur du Club Dev

Vous voici sur le site officiel du club **Guardia Root**. Vous pouvez y retrouver les membres du club, les projets qui ont été réalisés et bien plus encore.

---

## 🚀 Comment lancer le projet

Le projet est entièrement sous Docker.
*Inutile d'installer séparément React, Node ou MySQL sur votre ordinateur.*

### Prérequis
- [Docker Desktop](https://www.docker.com/products/docker-desktop/) installé et lancé.

### 1. Configuration des variables d'environnement

Copiez le fichier `.env.example` en `.env` (si ce n'est pas déjà fait) :

```bash
cp .env.example .env
```

### 2. Démarrer le projet

Ouvrez un terminal à la racine du projet, puis exécutez :

```bash
docker compose up -d --build
```

### 2. Accéder aux services de l'application

Une fois le `docker-compose` lancé, le projet est prêt !
Ouvrez votre navigateur web :

* 🌐 **Site Principal (Frontend)** : [http://localhost:3000](http://localhost:3000)
* ⚙️ **Serveur (Backend API)** : [http://localhost:4000/api/health](http://localhost:4000/api/health)
* 🗄️ **Vue de la base de données (Adminer)** : [http://localhost:8080](http://localhost:8080)
  * *(Remplissez : Système "MySQL", Serveur `db`, Utilisateur `atlas_user`, MDP `atlas_password`, DB `atlas_db`)*

### 3. Autres commandes utiles

- **Couper les serveurs** :
  ```bash
  docker-compose down
  ```
- **Suivre les bugs "en direct" (Logs)** :
  ```bash
  docker-compose logs -f
  ```
