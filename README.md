# born2beroot
Comment SSH fonctionne:
	SSH (Secure Shell) — c’est quoi ?

SSH est un protocole réseau qui permet de se connecter de manière sécurisée à un autre ordinateur (serveur) via un réseau, généralement Internet ou un réseau local.
À quoi sert SSH ?

    Contrôler à distance un serveur ou une machine

    Transférer des fichiers de façon sécurisée

    Exécuter des commandes à distance

    Gérer des systèmes sans accès physique

Comment ça marche ?

    Client SSH (ton ordi) lance une connexion vers un serveur SSH (la machine distante)

    Ils établissent une connexion sécurisée en utilisant un système de chiffrement pour que personne ne puisse intercepter ou lire les données échangées

    Le serveur demande une authentification (souvent par mot de passe ou clé SSH)

    Une fois authentifié, tu peux utiliser un terminal distant pour exécuter des commandes

Étapes techniques clés

    Le client initie la connexion sur le port 22 (par défaut)

    Le serveur envoie sa clé publique (pour le chiffrement)

    Le client vérifie l'identité du serveur (évite les attaques "man-in-the-middle")

    Le client et serveur négocient un chiffrement symétrique pour la session

    Authentification via :

        Mot de passe

        Clé publique/privée (plus sécurisée)

    Connexion établie, tu peux utiliser la machine distante

Exemple simple de connexion SSH

ssh user@serveur_ip

    user = nom d’utilisateur distant

    serveur_ip = adresse IP ou nom de domaine du serveur

Pourquoi SSH est sécurisé ?

    Les données sont chiffrées (cryptées)

    Les identités sont vérifiées avec des clés cryptographiques

    Protège contre les écoutes et intrusions
