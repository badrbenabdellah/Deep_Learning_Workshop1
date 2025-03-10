Table des Matières
Introduction
Installation des Dépendances
Téléchargement des Données
Exploration des Données
 * Données NYSE
 * Données de Maintenance Prédictive
Visualisation des Données
Analyse des Données
Conclusion

1. Introduction
Ce notebook Jupyter est conçu pour analyser deux ensembles de données distincts :

Données NYSE : Un ensemble de données contenant les prix des actions de la Bourse de New York.

Données de Maintenance Prédictive : Un ensemble de données utilisé pour la classification des pannes de machines.

L'objectif principal est d'explorer ces données, de les visualiser et de réaliser des analyses préliminaires pour comprendre les tendances et les caractéristiques des données.

2. Installation des Dépendances
Pour exécuter ce notebook, vous devez installer les bibliothèques Python suivantes :

pip install kagglehub pandas numpy torch matplotlib seaborn scikit-learn imblearn

Ces bibliothèques sont utilisées pour le téléchargement des données, la manipulation des données, l'apprentissage automatique, la visualisation et le rééchantillonnage des données.

3. Téléchargement des Données
Le notebook utilise kagglehub pour télécharger les ensembles de données nécessaires depuis Kaggle. Les données sont stockées dans des fichiers CSV et sont chargées dans des DataFrames Pandas pour une manipulation ultérieure.

Données NYSE
 * Fichier : prices.csv

 * Description : Contient les prix d'ouverture, de clôture, les prix bas et hauts, ainsi que le volume des actions de la NYSE.

Données de Maintenance Prédictive
Fichier : machine-predictive-maintenance-classification.csv

Description : Contient des données utilisées pour prédire les pannes de machines.

4. Exploration des Données
- Données NYSE
 * Aperçu des Données : Les premières lignes des données sont affichées pour comprendre la structure des données.
 * Statistiques Descriptives : Les statistiques de base (moyenne, écart-type, min, max, etc.) sont calculées pour chaque colonne.
 * Valeurs Manquantes : Vérification des valeurs manquantes dans les données.

- Données de Maintenance Prédictive
 * Aperçu des Données : Les premières lignes des données sont affichées pour comprendre la structure des données.
 * Statistiques Descriptives : Les statistiques de base sont calculées pour chaque colonne.
 * Valeurs Manquantes : Vérification des valeurs manquantes dans les données.

5. Visualisation des Données
- Données NYSE
 * Distribution des Prix de Clôture : Un histogramme est utilisé pour visualiser la distribution des prix de clôture.
 * Prix Bas vs Prix Hauts : Un graphique en nuage de points est utilisé pour visualiser la relation entre les prix bas et les prix hauts.

- Données de Maintenance Prédictive
 * Visualisation des Caractéristiques : Des graphiques sont utilisés pour visualiser les relations entre différentes caractéristiques des machines.

6. Analyse des Données
- Données NYSE
 * Tendances des Prix : Analyse des tendances des prix au fil du temps.
 * Corrélations : Calcul des corrélations entre les différentes colonnes pour identifier les relations potentielles.

- Données de Maintenance Prédictive
 * Classification : Utilisation de techniques de classification pour prédire les pannes de machines.
 * Rééchantillonnage : Utilisation de SMOTE pour équilibrer les classes dans les données de maintenance prédictive.

7. Conclusion
Ce notebook fournit une analyse approfondie des données boursières de la NYSE et des données de maintenance prédictive. Les visualisations et les analyses effectuées permettent de mieux comprendre les tendances et les caractéristiques des données, ce qui peut être utile pour des prédictions futures ou des décisions stratégiques.

Utilisation
Pour exécuter ce notebook, assurez-vous d'avoir installé toutes les dépendances nécessaires. Ensuite, ouvrez le notebook dans un environnement Jupyter et exécutez les cellules dans l'ordre.

jupyter notebook Atelier1.ipynb
