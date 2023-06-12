# Projet sur les accidents corporels de la circulation routière en France entre 2005 et 2021

Auteur : Nicolas Lejay dans le cadre du DU Data Analyst / Université de Cergy

## Description

Ce projet consiste à étudier un jeu de données sur les accidents corporels de la circulation routière entre 2005 et 2021. Il est fourni par l'
Observatoire National Interministériel de la Sécurité Routière (ONISR).

Les données sont disponibles sur le site [https://www.data.gouv.fr/fr/](https://www.data.gouv.fr/fr/). Il est constitué de quatre fichiers csv par année :

- le fichier *caracteristiques* contient les données des caractéristiques de l'accident (date, heure, conditions météo,...)
- le fichier *lieux* contient les données sur le type de route, l'état de la surface (normale, mouillée,...),...
- le fichier *vehicules* contient les informations sur les véhicules impliqués dans l'accident
- le fichier *usagers* contient les informations sur les personnes impliquées dans l'accident

L'ensemble du projet est codé en python et contient deux notebooks :

- le premier appelé *acc_route_import_concat.ipynb* dans lequel j'ai importé tous les fichiers de données et je les ai concaténés pour obtenir uniquement 4 fichiers (*caracteristiques*, *lieux*, *vehicules* et *usagers*), chacun contenant toutes les années de 2005 à 2021
- le deuxième qui regroupe les travaux sur le jeu de données, y compris le nettoyage.

## Installation

Clonez le repository et exécutez la commande suivante dans une invite de commande pour installer les librairies nécessaires à l'exécution du code :

```
pip install -r requirements.txt
```

Comme dit ci-dessus, les données sont disponibles sur le site [https://www.data.gouv.fr/fr/](https://www.data.gouv.fr/fr/). 

Attention, les fichiers ne possèdent pas tous le même encodage. Avant de les ouvrir dans le notebook avec la bilbiothèque pandas, j'ai changé l'encodage pour que tous les fichiers soient en utf-8.

