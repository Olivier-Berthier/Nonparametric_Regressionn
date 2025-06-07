# Régression Non-Paramétrique

Ce projet, réalisé dans le cadre de l’Executive Master Statistique & Intelligence Artificielle à Paris Dauphine PSL, consiste à explorer et modéliser une relation entre deux variables issues d’un jeu de données de 5000 observations, par des méthodes de régression non-paramétrique.

L’objectif principal est d’estimer la relation entre une variable explicative (X) et une variable à expliquer (Y), sans supposer de forme fonctionnelle. J’ai d’abord commencé par une exploration statistique du jeu de données (distributions, moments, histogramme), suivie de l’estimation de la densité de X via des méthodes à noyaux.

Ensuite, j’ai implémenté et comparé plusieurs techniques de régression non-paramétrique : la régression par noyau (kernel regression) et la méthode des k plus proches voisins (kNN regression). Une partie importante du travail porte sur l’optimisation des hyperparamètres (bandwidth h pour le noyau, nombre de voisins k en kNN), à travers la minimisation de l’erreur quadratique (MSE) par validation croisée Leave-One-Out, avec automatisation du choix optimal via des boucles de calcul.

Le projet inclut une discussion des méthodes d’optimisation du paramètre de régularisation : cross-validation (vise à minimiser l’ISE) et plug-in (MISE), appuyées par des références historiques et des aspects pratiques d’implémentation (vecteurisation des calculs, parallélisation via outer() en R).

