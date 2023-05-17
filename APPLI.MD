# Appli web de visualisation des données

**L'application web est disponible à cette adresse : [https://soduco.github.io/ic_2023_photographes_parisiens/](https://soduco.github.io/ic_2023_photographes_parisiens/)**

Cette application web permet d'interroger les ressources disponibles dans le triplestore par le biais d'un formulaire de recherche (il complète une requête SPARQL). 
Les données peuvent être visualisées de deux manières : 
* spatialement (pour celles qui ont pu être géocodées) : affichage dans une carte web-interrogeable
* temporelement : au clic sur un point, une requête SPARQL est lancée pour récupérer toutes les ressources du sous-graphe associé. Les données sont représentées sous la forme d'une frise chronologique.

## Environnement et outils

* Graph DB (version utilisée : 9.10.3)
* Editeur de texte
* Serveur Apache (ex : [Laragon](https://laragon.org/))
* HTML, CSS, Javascript (Leaflet)

## Installation en local et utilisation
* Installer l'application : voir [tutoriel d'installation avec Laragon - partie 1](doc/Tutoriel_Laragon.pdf)
* Démarrer GraphDB (cf [Tutoriel GraphDB](doc/Tutoriel_GraphDB.pdf)) : 
* Choisir (ou créer) le répertoire GraphDB qui contient le graphe spatio-temporel à visualiser (cf [Tutoriel GraphDB](doc/Tutoriel_GraphDB.pdf)) ;
* Ouvrir le fichier _parameters.js_ avec un éditeur de texte ;
* Copier l'adresse du répertoire GraphDB dans le fichier _parameters.js_ (remplacer l'adresse actuelle) (cf [Tutoriel GraphDB](doc/Tutoriel_GraphDB.pdf)) ;
* Toujours dans _parameters.js_ : choisir d'afficher ou non le fichier de référence (false par défaut, mettre _true_ pour voir l'exemple des photographes)
* Démarrer Laragon : voir [tutoriel d'installation avec Laragon - partie 2](doc/Tutoriel_Laragon.pdf)