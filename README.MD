Modélisation Prédictive des Loyers en France
Contexte

Ce projet a pour objectif de prédire le loyer au mètre carré (€/m²) à partir de caractéristiques des logements et de leur environnement, en utilisant des techniques de Machine Learning appliquées à des données publiques françaises.

Projet réalisé dans le cadre de la Licence 2 Informatique – Aix-Marseille Université.

Membres du groupe

Zoubiri Liza

Khati Maria

Sahin Melis

📁 Structure du projet
.
├── data/ # Données brutes et nettoyées (CSV)
│ ├── loyers_raw.csv
│ └── loyers_clean.csv
│
├── figures/ # Graphiques générés (PNG)
│ ├── hist_loyer_m2.png
│ ├── boxplot_type_habitat.png
│ ├── heatmap_correlation.png
│ └── importances_rf_lasso.png
│
├── top_erreurs_random_forest.xlsx # Résultats des erreurs les plus fortes
│
├── loyers_obtain.py # Script d’extraction et de fusion des données
├── loyers_scrub.py # Nettoyage et préparation
├── loyers_explore.py # Analyse exploratoire (EDA)
├── loyers_modelisation.py # Modélisation prédictive
└── ProjetInfo.ipynb # Version notebook (Google Colab)

Technologies utilisées

Langage : Python 3.10

Bibliothèques principales :

pandas, numpy → manipulation des données

matplotlib, seaborn → visualisations

scikit-learn → modèles prédictifs (Random Forest, Lasso, Régression Linéaire)

Méthodologie

Collecte des données depuis OpenDataSoft et Data.gouv.fr

Nettoyage & préparation des variables

Exploration (EDA) : statistiques descriptives, visualisations

Modélisation :

Régression Linéaire

Lasso

Random Forest (meilleur score)

Évaluation : RMSE, MAE, R²

Analyse des erreurs

Résultats principaux

Le modèle Random Forest obtient les meilleures performances pour la prédiction du loyer au m².

Les visualisations générées permettent d’identifier les variables les plus influentes.
