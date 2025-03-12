#### == INNO_PRESTAPLESK == ####

Projet de déploiement Prestashop gérable par plesk

#### == Ordre Installation == ####

1)  Installation de plesk (container ou host)
2)  Déploiement containeur Base de donnée
3)  Configuration plesk
4)  Liaison plesk -> BDD
5)  Création de BDD avec plesk
6)  Déploiement container Prestashop
7)  Configurer Prestashop
8)  Liaison prestashop vers BDD créer avec plesk
9)  Déplacer dossier site prestashop vers emplacement site plesk
10) Changer VHOST container prestashop (/var/www/html/prestashop)


#### == Rôle == ####
C) INNO_LAUNCH_CONTAINERS

  Permet de lancer les containeurs nécessaire au déploiement.

D) INNO_DOCKER

  Permet d'installer docker sur la machine ciblé.
  Ce rôle n'est pas utiliser de base.

#### == Variable == ####

|| vars/main.yml ||

-- project_name --
-- site_name --
  Ces deux variables sont a modifié a chaque projet, en effet la plupart des fichiers seront nomé a l'aide de celle ci

-- my_remote_user --
  Comme son nom l'indique il faut y placer l'utilisateur distant

-- docker_container --
  Les information des différents containers devront être saisie ici
  nom,volume,restart_policy,adresse ip


## -- TO DO -- ##

Ajouter un utilisateurs ftp pour plesk
gérer les droits de celui ci
gérer les droits du dossier du site
