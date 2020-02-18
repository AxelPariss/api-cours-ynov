# API


Cloner le projet
```
git clone https://github.com/AxelPariss/api-cours-ynov
```

Installer les dépendances
```
npm install
```

Lancer l'API
```
npm run build
npm start
```

## Structure

### Ressources

- Utilisateurs
- Catégories
- Produits

### Rôles

- Public (non connecté)
  - Peut s'inscrire et se connecter
- Employé (authentifié)
  - Voir, compter et modifier des catégories
  - Voir, compter et modifier des produits
- Manager
  - Gérer les catégories
  - Gérer les produits


Documentation : `/documentation/v1.0.0`


#### S'inscrire

> Ne pas oublier le remplacer `http://localhost:1337` par l'URL ngrok.

POST : `http://localhost:1337/auth/local/register`
```
{
  "username": "Jean",
  "email": "jean@domaine.com",
  "password": "password"
}
```


#### Se connecter

POST : `http://localhost:1337/auth/local`
```
{
  "identifier": "jean@domaine.com",
  "password": "password"
}
```
