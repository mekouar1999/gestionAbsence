# 🎓 School Attendance Management System

## 1. Présentation du projet

Application web de gestion des absences et des retards au sein d'un établissement scolaire ou universitaire.

L'application permet aux administrateurs, enseignants, responsables pédagogiques et étudiants de gérer et consulter les informations relatives à l'assiduité.

## 2. Technologies utilisées

### Frontend
- React.js
- Create React App (CRA)
- React Router DOM
- Axios
- Tailwind CSS

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT
- bcryptjs

### Outils
- Git et GitHub
- Postman
- Visual Studio Code

## 3. Architecture du projet

```text
school-attendance/
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── layouts/
│   │   ├── services/
│   │   ├── hooks/
│   │   ├── context/
│   │   ├── routes/
│   │   ├── App.js
│   │   └── index.js
│   │
│   └── package.json
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   │   ├── User.js
│   │   ├── Academic.js
│   │   ├── Assignment.js
│   │   ├── Session.js
│   │   ├── Attendance.js
│   │   ├── Notification.js
│   │   └── AuditLog.js
│   ├── routes/
│   ├── services/
│   ├── utils/
│   ├── server.js
│   └── package.json
│
├── .gitignore
└── README.md
```

## 4. Installation et configuration

### Prérequis

- Node.js (version LTS)
- npm
- MongoDB ou MongoDB Atlas
- Git
- Visual Studio Code

### Étape 1 : Cloner le projet

```bash
git clone https://github.com/username/school-attendance.git

cd school-attendance
```

### Étape 2 : Créer le frontend avec Create React App

Si le dossier frontend n'existe pas encore :

```bash
npx create-react-app frontend
```

Puis accéder au dossier :

```bash
cd frontend
```

### Étape 3 : Installer les dépendances frontend

```bash
npm install react-router-dom axios
```

Pour Tailwind CSS, suivre la documentation correspondant à la version de Create React App utilisée.

### Étape 4 : Installer les dépendances backend

Depuis la racine du projet :

```bash
cd ../backend

npm init -y

npm install express mongoose bcryptjs jsonwebtoken dotenv cors

npm install --save-dev nodemon
```

### Étape 5 : Configurer les variables d'environnement

Créer un fichier `.env` dans le dossier `backend` :

```env
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/school_attendance
JWT_SECRET=your_secret_key
NODE_ENV=development
```

### Étape 6 : Configurer les scripts du backend

Dans `backend/package.json` :

```json
{
  "scripts": {
    "start": "node server.js",
    "dev": "nodemon server.js"
  }
}
```

### Étape 7 : Configurer le proxy du frontend

Dans `frontend/package.json`, ajouter :

```json
"proxy": "http://localhost:5000"
```

Cela permettra au frontend de communiquer avec le backend en utilisant des chemins comme :

```javascript
axios.get("/api/students");
```

### Étape 8 : Démarrer le backend

Dans le dossier `backend` :

```bash
npm run dev
```

Le backend sera accessible sur :

`http://localhost:5000`

### Étape 9 : Démarrer le frontend

Dans un autre terminal, accéder au dossier `frontend` :

```bash
npm start
```

L'application React sera accessible sur :

`http://localhost:3000`

## 5. Scripts disponibles

### Frontend

| Commande | Description |
|---|---|
| `npm start` | Démarrer React en développement |
| `npm test` | Lancer les tests |
| `npm run build` | Générer la version de production |
| `npm run eject` | Exposer la configuration CRA (irréversible) |

### Backend

| Commande | Description |
|---|---|
| `npm run dev` | Démarrer avec Nodemon |
| `npm start` | Démarrer en production |

## 6. Organisation du développement

Le développement suivra la méthodologie Agile Scrum, avec les Sprints suivants :

- Sprint 1 : Authentification et gestion des utilisateurs.
- Sprint 2 : Gestion des étudiants, enseignants, groupes et modules.
- Sprint 3 : Gestion des séances et des absences.
- Sprint 4 : Justificatifs et notifications.
- Sprint 5 : Statistiques, tableaux de bord et exports.

## 7. Objectif final

Développer une application web moderne, sécurisée et évolutive permettant de centraliser la gestion des absences et de faciliter le suivi pédagogique et administratif d'un établissement scolaire.

**Architecture :** MERN Stack  
**Frontend :** React.js avec Create React App  
**Backend :** Node.js et Express.js  
**Database :** MongoDB  
**Version :** 1.0.0
