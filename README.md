# Detect'o'Bird
## Description
L'objectif de ce projet était de réaliser un detect'o'bird capable de détecter un type d'oiseau à partir d'une image.  
Nous avons réussis à compléter le projets dans les délais, il s'agit d'une classification d'images réalisée via `sklearn` en Python.  
Ce projet intervient dans le cadre de la deuxième année de DUT informatique.

## Fichiers
Vous trouverez dans ce dépôt :
* ce fichier `README.txt`
* un fichier de type `.ipynb` pour le notebook. Il contient tout le code documenté ainsi que le rapport expliqué.
* un fichier `.html` pour la verison numérique du notebook : il ne sera pas possile d'executer le code avec ce fichier, mais il est utile pour la visualisation des données sans passer par Jupyter. 

Le dataset est bien trop lourd, il n'est pas intégré à ce dépôt. En revanche, vous pouvez le trouver à l'adresse suivante : https://www.kaggle.com/gpiosenka/100-bird-species

## Comment lancer le programme ?
1. Lancer Jupyter, télécharger le dataset.
2. Vérifier les chemins d'accès, définis en début de programme (après chargement des modules), et les changer si necessaire (s'ils se trouvent à un emplacement différents). Il n'y a que deux chemins à changer normalement : celui du fichier CSV et celui du dossier des images.
3. Il est possible de modifier la constante `NUMBER_MAX_OF_CLASSES` pour tester plus ou moins de classes d'oiseaux mais attention, ne pas mettre une valeur inférieure à `3` ou supérieure à `50`. De grandes valeurs conduiront à des temps de chargement bien plus longs.
4. Une fois ceci réalisé, executer toutes les cellules. Au bout d'un moment le programme demande à sauvegarder les images en version redimensionnée (pour les charger plus vite + gain de temps), choisir une option.
5. Le reste du code devrait se dérouler sans problème.

> ⚠️ ATTENTION : nous avons remarqué qu'une erreur se produisait parfois et que des fois il manquait des données dans le dataset (cela ne nous est arrivé qu'une fois sur 4 téléchargements du dataset). Si cela arrive, aller dans le dossier de l'oiseau correspondant et ajouter 5 images portant les noms des fichiers.  
Nous n'avons pas prévus ce problème car le dataset a changé récemment et des images ont été ajoutés, donc s'il vous plaît, soyez vigilants.

## Librairies utilisées
- [x] `os` pour la gestion des chemins, création de dossiers, sauvegarde d'images.
- [x] `random` pour des tirages aléatoires.
- [x] `PIL` pour la gestion des images
- [x] `matplotlib` pour l'affichage de nos divers graphiques
- [x] `numpy` pour le stockages de toutes nos données
- [x] `pandas` pour le stockage de nos données dans des DataFrame et Series, ainsi que pour la lecture du fichier CSV.
- [x] `sklearn` pour l'apprentissage et les prédictions, plus généralement, tous nos modèles.

## Resultats et informations

Référez-vous à la notebook si vous souhaitez consulter les résultats obtenus par nos 10 modèles et notre réseau de neurones. Nous sommes autour de 70% d'accuracy actuellement. Ce résultat est largement améliorable.

## Auteurs

Jérémy TREMBLAY  
Rémi PALISSON
