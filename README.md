Rapport KAGONE Yasmine Oulia


Ce laboratoire nous a initié au déploiement et à la distribution de charge. Dans un premier temps,
nous avons appris à créer un environnement virtuel de travail à l'intérieur d'un répertoire et à le partager grâce à GitHub.
Nous avons créer notre repository à l'intérieur duquel nous avons installé notre environnement virtuel de travail. Nous avons 
ensuite obtenu les répertoires: Include, lib, Script. Par la suite, nous avons ensuite activé notre environnement de travail, 
puis installé la librairie flask. L'installation de flask nous a permit d'initialiser un fichier texte contenant toutes les 
dépendances de notre environnement.

Lorsque nous clonons l'application de notre collaborateur, nous devons installer son fichier texte contenant toutes ses dépendances
pour un bon fonctionnement.

Nous avons manipulé Nginx qui est un logiciel souvent utilisé comme serveur http, distributeur de charge pour distribuer les 
requêtes entre deux instances de l'application, testant ainsi la tolérance aux pannes et la gestion des volumes de requêtes.


Réponses aux questions:


6-Lorsque nous arrêtons l'application Python, la page web devient inaccessible via l'adresse http://IP_DE_LA_MACHINE:3001/


16-Lorsque nous rafraichissons la page plusieurs fois, nous remarquons que les réponses alternent entre les deux applications, ce qui nous montre que Nginx distribue les requêtes entre les deux machines.


17-a. Quand on arrête nginx, l'application est toujours accessible via l'adresse http://IP_DE_LA_MACHINE:3001/


b. Quand on arrête nginx, l'application devient inaccessible via l'adresse http://IP_DE_LA_MACHINE:8181/


Lien pour la vidéo de démonstration: https://uqac.ca.panopto.com/Panopto/Pages/Viewer.aspx?id=81c06e66-3934-4b77-bba3-b1fd0002930c 


Commandes utilisées:


-mkdir "nom du repertoire desire": pour créer le dossier qui contiendra répertoire virtuel


-cd "nom du repertoire desire": entrer dans le dossier créé


-python -m venv "nom du repertoire desire": pour créer l'envrionnement virtuel à l'interieur du dossier desirer


-cd Script, activate.bat, cd ..: pour activer l'environnement virtuel


-python -m pip install flask: pour installer la librairie flask


-python -m pip freeze > requierements.txt: pour initialer un fichier texte contenant tout les dépendances de notre envrionnement


-python -m pip install -r requierements.txt: pour installer les dépendances necessaires inscrites dans le fichier requierements.txt


-start nginx.exe: pour lancer le logiciel Nginx.
