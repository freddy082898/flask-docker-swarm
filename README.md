# flask-docker-swarm

1-Création du dépôt sur GitHub:

-Allez sur le site de GitHub (github.com) et se connecter à notre compte.
-Cliquez sur le bouton "New" pour créer un nouveau dépôt.
-Donnez un nom au dépôt, "flask-docker-swarm".
-Cochez l'option pour initialiser le dépôt avec un README.md.
-Cliquez sur le bouton "Create repository" pour créer le dépôt.

2-Développement de l'application Flask:

-Utilisez le code fourni dans app.py pour créer l'application Flask.
-S'assurez que les variables d'environnement pour la connexion à la base de données sont correctement définies.
-Créez un fichier requirements.txt contenant les dépendances nécessaires à l' application Flask.

3-Utilisation de Docker pour la conteneurisation:

-Créez un fichier Dockerfile à la racine de votre projet.
-Utilisez le Dockerfile pour définir les étapes nécessaires à la construction de l'image Docker de l'application Flask.
-Installez les dépendances Python à partir de requirements.txt.
-Exposez le port sur lequel  l'application Flask écoute ( le port 5000).

4- Création d'un Docker Swarm Cluster:

-S'assurer d'avoir Docker installé sur la  machine.
-Initialisez un cluster Docker en mode Swarm en exécutant la commande docker swarm init.


5- Stockage sécurisé des informations de connexion à la base de données:

-Utilisez la fonctionnalité Docker secrets pour stocker de manière sécurisée les informations de connexion à la base de données.
-Créez un secret Docker pour chaque variable d'environnement requise pour la connexion à la base de données.

6- Déploiement de l'application sur le cluster Swarm:

-Utilisez Docker Stack pour déployer votre application Flask et la base de données MariaDB en tant que services dans le cluster Swarm.
-Définissez un fichier docker-compose.yml pour spécifier les services à déployer.
-Exécutez la commande docker stack deploy pour déployer les services sur le cluster Swarm.

7- Configuration de GitHub Actions pour la génération d'image Docker:

-Créez un fichier de configuration GitHub Actions (.github/workflows/docker-build.yml).
-Définissez des étapes dans ce fichier pour construire et pousser l'image Docker vers un registre privé  à chaque push sur la branche main.

8- Ajout de collaborateurs au dépôt GitHub:

-Allez dans les paramètres de votre dépôt sur GitHub.
-Cliquez sur "Manage access" ou "Collaborators".
-Tapez le nom d'utilisateur hellodamien et appuyez sur "Add collaborator".
