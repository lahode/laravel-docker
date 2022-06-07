# Projet bibliothèque

-----

## Installation

### 1. Lancer le conteneur

```
docker-compose up -d
```

### 2. Configurer le fichier d'environnement

Copier-coller le fichier .env.exemple vers .env

Et modifier les lignes suivantes:

```
DB_HOST=0.0.0.0
DB_PORT=33006
DB_DATABASE=realise_biblio
DB_USERNAME=realise
DB_PASSWORD=realise1234
```

### 3. Installer le projet

```
composer install
```

### 4. Tester la connexion (en lançant la migration)

```
php artisan migrate:fresh --seed
```
