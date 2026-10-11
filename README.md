# MERN TP2

Node.js + Express

## Lancer

```bash
npm install
npm run dev   # http://localhost:3000 (recharge auto)
```

## Endpoints

| Méthode | URL | Réponse |
|---|---|---|
| GET | `/` | message d'accueil |
| GET | `/api/articles` | liste (?author= pour filtrer) |
| GET | `/api/articles/:id` | un article (404 sinon) |
| POST | `/api/articles` | crée {title, author} → 201 |
| PUT | `/api/articles/:id` | modifie {title, author} → 200 (404 sinon) |
| DELETE | `/api/articles/:id` | supprime → 200 (404 sinon) |
| GET | `/api/users` | liste (?role= pour filtrer) |
| GET | `/api/users/:id` | un utilisateur (404 sinon) |
| POST | `/api/users` | crée {name, email, role} → 201 (400 si invalide) |
| DELETE | `/api/users/:id` | supprime → 200 (404 sinon) |

## Fichiers

    server.js – point d'entrée Express, middlewares, montage routeurs
    controllers/articleController.js – logique métier articles
    controllers/userController.js – logique métier users
    routers/articleRoutes.js – routes /api/articles
    routers/userRoutes.js – routes /api/users
    utils/validators.js – validation réutilisable
    exercices_js.js – exercices JS (node exercices_js.js)
    Compte-rendu-API-SoC-Aziz-MANSOUR.pdf – rapport

Mohamed Aziz Mansour – 5ème DS G3 – EPS 2026/2027
