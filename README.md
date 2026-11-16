# 🎓 School Attendance Management System

## 1. Présentation du projet

**School Attendance Management System** est une application web destinée à digitaliser et simplifier la gestion des absences et des retards au sein d'un établissement scolaire ou universitaire.

L'application permet de centraliser les informations relatives à l'assiduité des étudiants, de faciliter le travail des enseignants et du service de scolarité, et de fournir un suivi précis de la présence des étudiants.

Elle propose différents espaces selon le rôle de l'utilisateur : administrateur, enseignant, responsable pédagogique et étudiant.

### 🎯 Objectifs du projet

- Digitaliser la gestion des absences.
- Faciliter la saisie des présences par les enseignants.
- Permettre aux étudiants de consulter leur situation.
- Centraliser les données relatives à l'assiduité.
- Automatiser le suivi des absences et des retards.
- Générer des statistiques et des rapports.
- Améliorer la communication entre les étudiants, les enseignants et l'administration.

---

## 2. Acteurs du système

L'application comporte quatre principaux profils utilisateurs.

| Acteur | Responsabilités |
|---|---|
| Administrateur | Gestion globale de la plateforme |
| Enseignant | Gestion des présences et des absences |
| Responsable pédagogique | Suivi et validation des justificatifs |
| Étudiant | Consultation de ses absences et soumission des justificatifs |

---

## 3. Fonctionnalités principales

### 3.1. Authentification et gestion des utilisateurs

- Connexion et déconnexion.
- Authentification sécurisée.
- Gestion des rôles et permissions.
- Modification du profil utilisateur.
- Réinitialisation du mot de passe.
- Protection des routes selon le rôle.

### 3.2. Gestion administrative

- Ajouter, modifier et supprimer des étudiants.
- Ajouter, modifier et supprimer des enseignants.
- Créer et gérer les groupes et les classes.
- Gérer les filières et les niveaux d'études.
- Gérer les années universitaires et les semestres.
- Gérer les modules et les matières.
- Affecter les enseignants aux groupes et aux modules.
- Consulter toutes les absences de l'établissement.

### 3.3. Gestion des présences et des absences

- Enregistrer les présences des étudiants.
- Enregistrer les absences.
- Enregistrer les retards.
- Associer chaque absence à une séance.
- Consulter l'historique des absences.
- Modifier une feuille de présence.
- Éviter les doublons d'enregistrement.
- Distinguer les absences justifiées et non justifiées.

### 3.4. Gestion des justificatifs

- Soumettre un justificatif d'absence.
- Joindre un document justificatif (PDF, JPG, PNG).
- Consulter les justificatifs.
- Accepter ou refuser une demande.
- Ajouter un commentaire à une décision.
- Suivre le statut d'une demande.

Statuts possibles :
- En attente.
- Acceptée.
- Refusée.

### 3.5. Tableau de bord et statistiques

- Nombre total d'étudiants.
- Nombre total d'absences.
- Nombre de retards.
- Taux global d'assiduité.
- Statistiques par classe.
- Statistiques par module.
- Statistiques par enseignant.
- Statistiques par période.
- Identification des étudiants ayant dépassé le seuil d'absence autorisé.

### 3.6. Notifications

- Notification lorsqu'une absence est enregistrée.
- Notification lorsqu'un justificatif est accepté ou refusé.
- Alerte lorsqu'un étudiant dépasse le seuil d'absence.
- Notifications relatives aux changements de statut.

### 3.7. Exportation et rapports

- Génération des rapports d'absences en PDF.
- Exportation des données en Excel.
- Filtrage par étudiant, groupe, module et période.
- Génération des relevés individuels d'assiduité.

---

# 4. User Stories – Besoins fonctionnels

Les fonctionnalités de l'application sont définies sous forme de User Stories selon la méthodologie Agile.

Format utilisé :

**En tant que [acteur], je peux [action] afin de [objectif].**

## 4.1. User Stories – Administrateur

- US01 : En tant qu'administrateur, je peux me connecter à la plateforme afin d'accéder à mon espace de gestion.
- US02 : En tant qu'administrateur, je peux ajouter un étudiant afin de l'enregistrer dans le système.
- US03 : En tant qu'administrateur, je peux modifier les informations d'un étudiant afin de maintenir ses données à jour.
- US04 : En tant qu'administrateur, je peux supprimer un étudiant afin de gérer les inscriptions.
- US05 : En tant qu'administrateur, je peux ajouter et gérer les enseignants.
- US06 : En tant qu'administrateur, je peux créer et gérer les groupes et les classes.
- US07 : En tant qu'administrateur, je peux créer et gérer les filières et les niveaux d'études.
- US08 : En tant qu'administrateur, je peux créer et gérer les modules.
- US09 : En tant qu'administrateur, je peux affecter un enseignant à un module et à un groupe.
- US10 : En tant qu'administrateur, je peux consulter toutes les absences de l'établissement.
- US11 : En tant qu'administrateur, je peux modifier ou supprimer une absence en cas d'erreur.
- US12 : En tant qu'administrateur, je peux consulter les statistiques d'absences par étudiant, groupe, module et période.
- US13 : En tant qu'administrateur, je peux identifier les étudiants ayant dépassé le seuil d'absence autorisé.
- US14 : En tant qu'administrateur, je peux exporter les rapports d'absences au format PDF ou Excel.

## 4.2. User Stories – Enseignant

- US15 : En tant qu'enseignant, je peux me connecter à mon espace personnel.
- US16 : En tant qu'enseignant, je peux consulter mon emploi du temps.
- US17 : En tant qu'enseignant, je peux consulter la liste des étudiants de mes groupes.
- US18 : En tant qu'enseignant, je peux sélectionner une séance afin de gérer les présences.
- US19 : En tant qu'enseignant, je peux enregistrer les absences des étudiants pendant un cours.
- US20 : En tant qu'enseignant, je peux signaler un retard pour un étudiant.
- US21 : En tant qu'enseignant, je peux modifier une feuille de présence en cas d'erreur.
- US22 : En tant qu'enseignant, je peux consulter l'historique des absences de mes groupes.
- US23 : En tant qu'enseignant, je peux consulter le nombre d'absences d'un étudiant.
- US24 : En tant qu'enseignant, je peux filtrer les absences par date, groupe et module.
- US25 : En tant qu'enseignant, je peux consulter le statut des justificatifs de mes étudiants.

## 4.3. User Stories – Étudiant

- US26 : En tant qu'étudiant, je peux me connecter à mon espace personnel.
- US27 : En tant qu'étudiant, je peux consulter mon profil et mes informations scolaires.
- US28 : En tant qu'étudiant, je peux consulter mon historique d'absences.
- US29 : En tant qu'étudiant, je peux consulter mes absences par module.
- US30 : En tant qu'étudiant, je peux distinguer mes absences justifiées et non justifiées.
- US31 : En tant qu'étudiant, je peux consulter mon nombre total d'heures d'absence.
- US32 : En tant qu'étudiant, je peux consulter mon taux d'assiduité.
- US33 : En tant qu'étudiant, je peux recevoir une notification lorsqu'une nouvelle absence est enregistrée.
- US34 : En tant qu'étudiant, je peux soumettre un justificatif afin de demander la régularisation de mon absence.
- US35 : En tant qu'étudiant, je peux consulter le statut de ma demande de justification.
- US36 : En tant qu'étudiant, je peux consulter les commentaires associés à une demande refusée.

## 4.4. User Stories – Responsable pédagogique / Service de scolarité

- US37 : En tant que responsable pédagogique, je peux consulter les absences de tous les groupes dont j'ai la responsabilité.
- US38 : En tant que responsable pédagogique, je peux suivre l'assiduité des étudiants par semestre.
- US39 : En tant que responsable pédagogique, je peux identifier les étudiants présentant un taux d'absence élevé.
- US40 : En tant que responsable pédagogique, je peux consulter les justificatifs déposés par les étudiants.
- US41 : En tant que responsable pédagogique, je peux accepter ou refuser une demande de justification.
- US42 : En tant que responsable pédagogique, je peux ajouter un commentaire à une décision.
- US43 : En tant que responsable pédagogique, je peux générer un rapport d'assiduité pour une classe ou une filière.
- US44 : En tant que responsable pédagogique, je peux consulter les statistiques globales de l'établissement.

---

# 5. Critères d'acceptation (Acceptance Criteria)

Chaque User Story doit être accompagnée de critères permettant de vérifier le bon fonctionnement de la fonctionnalité.

### Exemple 1 : Enregistrement d'une absence

**US19 : En tant qu'enseignant, je peux enregistrer l'absence d'un étudiant pendant une séance afin d'assurer le suivi de son assiduité.**

Critères d'acceptation :

1. L'enseignant doit être authentifié.
2. L'enseignant doit sélectionner un groupe et un module qui lui sont affectés.
3. Le système affiche la liste des étudiants concernés.
4. L'enseignant peut sélectionner un ou plusieurs étudiants absents.
5. Le système enregistre la date, le module, le groupe et la séance.
6. Le système empêche l'enregistrement de doublons pour une même séance.
7. L'absence apparaît dans l'historique de l'étudiant.
8. L'étudiant peut consulter cette absence depuis son espace personnel.

### Exemple 2 : Justification d'une absence

**US34 : En tant qu'étudiant, je peux soumettre un justificatif afin de demander la régularisation de mon absence.**

Critères d'acceptation :

1. L'étudiant doit être authentifié.
2. L'étudiant sélectionne l'absence concernée.
3. L'étudiant joint un document justificatif.
4. Le système vérifie le format et la taille du document.
5. Le système enregistre la demande avec le statut « En attente ».
6. Le responsable pédagogique peut accepter ou refuser la demande.
7. L'étudiant reçoit une notification concernant la décision.

### Exemple 3 : Validation d'un justificatif

**US41 : En tant que responsable pédagogique, je peux accepter ou refuser une demande de justification.**

Critères d'acceptation :

1. Le responsable pédagogique doit être authentifié.
2. Il peut consulter les demandes en attente.
3. Il peut consulter le justificatif associé.
4. Il peut accepter ou refuser la demande.
5. Il peut ajouter un commentaire.
6. Le statut de la demande est mis à jour.
7. L'étudiant reçoit une notification.

---

# 6. Règles de gestion

Les règles suivantes définissent le fonctionnement métier de l'application.

- Chaque utilisateur possède un compte personnel.
- Chaque utilisateur possède un rôle déterminant ses permissions.
- Un enseignant ne peut enregistrer des présences que pour les groupes et modules qui lui sont affectés.
- Chaque séance est associée à un groupe, un module, un enseignant, une date et un horaire.
- Un étudiant ne peut avoir qu'un seul enregistrement de présence par séance.
- Chaque étudiant peut avoir l'un des statuts suivants pour une séance : Présent, Absent ou En retard.
- Une absence peut être justifiée ou non justifiée.
- Une demande de justification doit être associée à une absence existante.
- Seul un utilisateur autorisé peut valider ou refuser un justificatif.
- Un étudiant ne peut consulter que ses propres informations.
- Les statistiques doivent être calculées à partir des données enregistrées.
- Les données doivent être conservées par année universitaire.

---

# 7. Technologies utilisées

L'application repose sur l'architecture MERN Stack.

| Technologie | Utilisation |
|---|---|
| React.js | Développement de l'interface utilisateur |
| Node.js | Environnement d'exécution backend |
| Express.js | Création de l'API REST |
| MongoDB | Base de données NoSQL |
| Mongoose | Modélisation des données |
| JWT | Authentification |
| bcrypt | Cryptage des mots de passe |
| Axios | Communication frontend/backend |
| Tailwind CSS | Mise en forme de l'interface |
| Git & GitHub | Gestion de versions et collaboration |
| Postman | Tests de l'API REST |

---

# 8. Architecture du projet

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
│   │   └── App.jsx
│   │
│   ├── package.json
│   └── vite.config.js
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── utils/
│   ├── server.js
│   └── package.json
│
├── .gitignore
└── README.md
```

---

# 9. Modélisation de la base de données

Les principales collections MongoDB sont les suivantes :

| Collection | Description |
|---|---|
| Users | Comptes utilisateurs et rôles |
| Students | Informations des étudiants |
| Teachers | Informations des enseignants |
| Groups | Classes et groupes |
| Programs | Filières et niveaux |
| Modules | Matières et modules |
| Sessions | Séances de cours |
| Attendance | Présences, absences et retards |
| Justifications | Justificatifs et demandes de validation |
| Notifications | Notifications des utilisateurs |

### Relations principales

- Un groupe contient plusieurs étudiants.
- Un enseignant peut être affecté à plusieurs modules.
- Un module peut être enseigné dans plusieurs groupes.
- Une séance appartient à un groupe et à un module.
- Une séance possède plusieurs enregistrements de présence.
- Un étudiant possède plusieurs enregistrements de présence.
- Une absence peut être associée à une demande de justification.
- Un utilisateur peut recevoir plusieurs notifications.

---

# 10. API REST – Endpoints principaux

### Authentification

| Méthode | Endpoint | Description |
|---|---|---|
| POST | `/api/auth/login` | Connexion |
| POST | `/api/auth/register` | Création d'un compte |
| GET | `/api/auth/me` | Informations utilisateur |
| POST | `/api/auth/logout` | Déconnexion |

### Étudiants

| Méthode | Endpoint | Description |
|---|---|---|
| GET | `/api/students` | Liste des étudiants |
| GET | `/api/students/:id` | Détails d'un étudiant |
| POST | `/api/students` | Ajouter un étudiant |
| PUT | `/api/students/:id` | Modifier un étudiant |
| DELETE | `/api/students/:id` | Supprimer un étudiant |

### Enseignants

| Méthode | Endpoint | Description |
|---|---|---|
| GET | `/api/teachers` | Liste des enseignants |
| POST | `/api/teachers` | Ajouter un enseignant |
| PUT | `/api/teachers/:id` | Modifier un enseignant |
| DELETE | `/api/teachers/:id` | Supprimer un enseignant |

### Présences et absences

| Méthode | Endpoint | Description |
|---|---|---|
| GET | `/api/attendance` | Consulter les absences |
| GET | `/api/attendance/:id` | Détails d'une absence |
| POST | `/api/attendance` | Enregistrer une présence ou absence |
| PUT | `/api/attendance/:id` | Modifier un enregistrement |
| DELETE | `/api/attendance/:id` | Supprimer un enregistrement |

### Justificatifs

| Méthode | Endpoint | Description |
|---|---|---|
| GET | `/api/justifications` | Liste des justificatifs |
| POST | `/api/justifications` | Soumettre un justificatif |
| PUT | `/api/justifications/:id/approve` | Accepter une demande |
| PUT | `/api/justifications/:id/reject` | Refuser une demande |

### Statistiques et rapports

| Méthode | Endpoint | Description |
|---|---|---|
| GET | `/api/reports/dashboard` | Statistiques globales |
| GET | `/api/reports/students/:id` | Rapport individuel |
| GET | `/api/reports/groups/:id` | Rapport par groupe |
| GET | `/api/reports/export` | Exporter les données |

---

# 11. Sécurité

La sécurité de l'application repose sur plusieurs mécanismes :

- Authentification avec JSON Web Token (JWT).
- Hachage des mots de passe avec bcrypt.
- Middleware de vérification des tokens.
- Gestion des rôles et des permissions (RBAC).
- Protection des routes privées.
- Validation des données côté serveur.
- Vérification des fichiers téléchargés.
- Protection contre les accès non autorisés.
- Utilisation de variables d'environnement pour les informations sensibles.

---

# 12. Méthodologie Agile – Organisation des Sprints

Le développement est organisé selon la méthodologie Agile Scrum.

### Sprint 1 – Authentification et gestion des utilisateurs

Objectifs :
- Création du projet frontend et backend.
- Configuration de MongoDB.
- Mise en place de l'authentification.
- Gestion des rôles.
- Création des interfaces de connexion.

### Sprint 2 – Gestion administrative

Objectifs :
- Gestion des étudiants.
- Gestion des enseignants.
- Gestion des groupes et des classes.
- Gestion des filières et des modules.
- Affectation des enseignants.

### Sprint 3 – Gestion des présences et des absences

Objectifs :
- Création et gestion des séances.
- Consultation des listes d'étudiants.
- Enregistrement des présences.
- Enregistrement des absences et retards.
- Consultation de l'historique.

### Sprint 4 – Justificatifs et notifications

Objectifs :
- Dépôt des justificatifs.
- Consultation des demandes.
- Validation et refus des justificatifs.
- Mise en place des notifications.

### Sprint 5 – Statistiques et reporting

Objectifs :
- Création du tableau de bord.
- Calcul du taux d'assiduité.
- Statistiques par groupe et module.
- Exportation PDF et Excel.
- Tests et corrections.

---

# 13. Installation et configuration

### Prérequis

- Node.js (version LTS).
- npm.
- MongoDB local ou MongoDB Atlas.
- Git.
- Un éditeur de code (VS Code recommandé).

### Étape 1 : Cloner le projet

```bash
git clone [https://github.com/username/school-attendance.git](https://github.com/mekouar1999/gestionAbsence#pr%C3%A9requis)

cd school-attendance
```

### Étape 2 : Installer le frontend

```bash
cd frontend

npm install
```

### Étape 3 : Installer le backend

```bash
cd ../backend

npm install
```

### Étape 4 : Configurer les variables d'environnement

Créer un fichier `.env` dans le dossier `backend` :

```env
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/school_attendance
JWT_SECRET=your_secret_key
NODE_ENV=development
```

### Étape 5 : Démarrer le backend

```bash
cd backend

npm run dev
```

### Étape 6 : Démarrer le frontend

Dans un autre terminal :

```bash
cd frontend

npm run dev
```

L'application sera accessible à l'adresse indiquée par Vite, généralement :

`http://localhost:5173`

Le backend sera accessible sur :

`http://localhost:5000`

---

# 14. Tests

Les tests doivent couvrir les principales fonctionnalités de l'application.

### Tests fonctionnels

- Vérifier la connexion selon chaque rôle.
- Vérifier les permissions des utilisateurs.
- Vérifier la création et la modification des étudiants.
- Vérifier l'enregistrement des présences et absences.
- Vérifier la soumission des justificatifs.
- Vérifier la validation des justificatifs.
- Vérifier les statistiques.

### Tests API

Les endpoints REST seront testés avec Postman.

### Tests de sécurité

- Vérifier l'accès aux routes protégées.
- Vérifier les autorisations selon les rôles.
- Vérifier la validation des données.
- Vérifier la protection des informations personnelles.

---

# 15. Améliorations futures

Plusieurs évolutions pourront être intégrées :

- Application mobile Android et iOS.
- Notifications par e-mail.
- Intégration avec l'emploi du temps de l'établissement.
- Génération automatique des rapports mensuels.
- Signature électronique des feuilles de présence.
- Système de QR Code pour enregistrer les présences.
- Tableau de bord analytique avancé.
- Intégration avec le système de gestion scolaire existant.

---

# 16. Objectif final

L'objectif final est de développer une plateforme centralisée permettant à un établissement scolaire ou universitaire de gérer efficacement l'assiduité de ses étudiants.

L'application doit être intuitive, sécurisée, évolutive et adaptée aux besoins des différents acteurs de l'établissement.

---

**Projet :** School Attendance Management System  
**Architecture :** MERN Stack  
**Méthodologie :** Agile Scrum  
**Version :** 1.0.0  
**Statut :** En cours de développement
