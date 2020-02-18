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
