# Rapport d'exploration – Lab 0

## Tests fonctionnels (QA – Belvina Kanga)

**Bug #1** : L’API ne démarrait pas car `MONGODB_URI` manquante dans `.env`.  
**Solution** : Création d’un cluster MongoDB Atlas, configuration d’un utilisateur (`qa_user`), ajout de l’URI correcte.

**Bug #2** : Le script `npm run seed` échouait (erreur `undefined`).  
**Solution** : Correction de `seed.js` en ajoutant `require('dotenv').config()`.

**Tests effectués** :
- ✅ Page d’accueil affiche la liste des restaurants
- ✅ Page détail d’un restaurant affiche les plats
- ✅ Routes API `/api/restaurants` et `/api/plats` renvoient du JSON valide

**Conclusion** : L’application est fonctionnelle pour le Lab 0.