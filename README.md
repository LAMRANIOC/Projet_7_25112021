
# Projet 7 d'OpenClassroom : Groupomania

Le but de ce projet est de créer un réseau social d'entreprise permettant aux employés de créer un compte et de partager
des posts pouvant être commenté afin de leurs permettre de communiqué.
Ce projet nécéssite de créer un backend, et un frontend.

## Fonctionnalitées demandées pour le projet :

- Création d'un compte simple et possible depuis un mobile.
- Suppréssion de compte possible.
- Accès à un forum des salariés.
- Repérer les dernières publications facilement.
- Avoir un accès admin pour l'un des utilisateurs.

## Liste des technologies utilisées pour le projet :

### Frontend :

- Vue.js
- Axios

### Backend :

- Mysql
- Sequelize
- Node.js
- Express



# frontend

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## Instalation :

### Backend :

Ouvrez un terminal, dans lequel il faut se placer sur le dossier Backend :

```
cd Backend
```

Puis installez les modules :

```
npm i
```

Changez les valeurs du ".env" pour qu'il corresponde avec vos paramètres en changeant le DB_PASS par le votre.
Enfin, lancez le serveur :

```
node server
```

Le Backend se lancera à l'issus de ces commandes. Si erreur, faites la partie Base de données et réessayer de lancer le serveur

### Base de données :

Pour lancer la Bdd, lancez votre invite de commande MySql "MySQL 8.0 Command Line Client", et créez la Bdd groupomania
en important le fichier initialisationBdd.sql :

```
mysql > source C:/<cheminDuDossier>/initialisation.sql
```

Cela va générer une base de donnée MySQL contenant des tables : Users, Messages et Comments.

### Frontend :

Le serveur va se lancer, résultant sur :

App running at:

- Local: http://localhost:8080/


### Fonctionnement :

Arrivé sur la page de connection,Pour renseu=igner le 1er utilisateur.

Une fois inscrit, retournez sur votre invite de commande MySQL et importez le fichier "Admin.sql" :

```
mysql > source C:/<cheminDuDossier>/Admin.sql
```

Cette commande permettra de passer le premier utilisateur créer en "is_admin : 1", ce qui lui donnera les droits d'administration
étant : suppréssion de messages/comments et users. (Vous pourrez supprimer les messages & commentaires des autres utilisateurs ansi que leurs comptes).
