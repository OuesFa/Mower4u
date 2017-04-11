# Mower4u
## Cas d'étude pour Xebia

**Objectif:** Estimer/Prédire l'attractivité des tondeuses.

## I. La démarche:

Nous avons souhaité réaliser une étude qui suit le cheminement d'une démarche d'étude  : à savoir acquérir la donnée, l'observer, se l'approprier et la nettoyer. Suite à cela nous appliquons nos algorithmes de machine learning afin de prédire notre cible. Il est nécessaire pour chaque model de paramétrer l'algorithme choisi afin d'en tirer les meilleurs performances, mais très vite on s'aperçoit que les résultats atteignent rapidement un plafond que l'on ne peut améliorer seulement en retravaillant le tuning de l'algorithme.

Le gain le plus important sur les performances est atteint en retraitant la donnée la plus intelligemment possible, dans notre situation, avec des retraitements simples on obtient des gains de performances notables pour la métrique RMSLE.

## II. Data management:

- Imputation des données catégorielles par leur top représentant et des données continues par leur médiane.
- Label Encodage sur les variables catégorielles
- Normalisation des données mal formatées
- Traitement des outliers

## III. Choix des algorithmes:

- 1er. For�ts Al�atoires (nb_estimateurs=300, max_profondeur=7)
- 2nd. Régression Linéaire standard (sans pénalisatio
- 3eme. XGBoost (profondeur 4, nb_estimateurs : 400, learning rate à 0.05) sur donnée d'ordre 1.

