# Traitement-des-donnees-distribuees

Pour ce projet, nous avons utilisé le jeu de données suivant : https://www.kaggle.com/geomack/spotifyclassification/data
Ce jeu de données contient 2017 chansons avec des attributs de l'API Spotify.
Un utilisateur a attribué la note de « 1 » s’il aime la chanson et « 0 » s’il n’aime pas la chanson. L’objectif est de construire un classificateur qui pourrait prédire si l'utilisateur aime ou non une chanson.
La base est composée de 16 colonnes : 13 sont des attributs de chanson, une colonne pour le nom de la chanson, une pour l'artiste, et une colonne cible ("target") qui est l'étiquette avec la note attribuée à la chanson.
Les 13 attributs de la piste sont les suivants : l'acoustique, la danceabilité, la durée, l'énergie, l'instrumentalité, la touche, la vivacité, le volume, le mode, la faculté d'expression, le tempo, la signature temporelle, la valence.
Vous trouverez une définition détaillée de chaque variable au lien suivant : https://developer.spotify.com/web-api/get-audio-features/

Dans une première, nous avons fait une analyse exploratoire des données. 
Dans une seconde partie, nous avons cherché à prédire si le testeur aime ou non cette chanson. Nous avons tester les modèles suivantes : une régression logistique, un arbre de décision et une forêt aléatoire. Pour chacun de ces modèles, nous testons d'abord le modèle avec les paramètres par défaut, puis nous cherchons les paramètres optimaux avec les librairies "ParamGridBuilder" et "CrossValidator".

Ce projet a été réalisé avec la librairie PySpark sous Python.

Dans ce répertoire, vous trouverez le notebook python.


