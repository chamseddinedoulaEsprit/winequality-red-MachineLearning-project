# 🍷 Analyse de la Qualité des Vins Rouges

## 📋 Description du Projet
Ce projet utilise le machine learning pour analyser et prédire la qualité des vins rouges en se basant sur leurs caractéristiques physicochimiques. L'analyse comprend à la fois des approches supervisées (classification) et non supervisées (clustering) pour extraire des insights pertinents.

## 🎯 Objectifs
1. **DSO1**: Prédire la qualité du vin selon ses caractéristiques chimiques
2. **DSO2**: Classifier les groupes de vin selon des caractéristiques similaires (segmentation)

## 📊 Structure du Projet

Le projet est organisé en plusieurs phases d'analyse :

1. **Compréhension des Données**
   - Analyse de la structure et distribution des variables
   - Détection des valeurs manquantes et aberrantes
   - Visualisation des corrélations

2. **Préparation des Données**
   - Standardisation des caractéristiques
   - Analyse en Composantes Principales (ACP)
   - Sélection des composantes optimales

3. **Modélisation**
   - Classification supervisée avec Random Forest, Bagging et Stacking
   - Clustering non supervisé (K-Means, DBSCAN)
   - Validation croisée et optimisation des hyperparamètres

4. **Évaluation**
   - Métriques de performance (Accuracy, Precision, Recall, F1-Score)
   - Analyse des clusters et leur signification
   - Courbes ROC et matrices de confusion

## 📈 Principaux Résultats

### Classification
- Meilleur modèle : **Bagging Classifier** avec une précision de **75.62%**
- Performances comparées :
  - Bagging: 75.62%
  - Random Forest: 74.87%
  - Stacking: 74.06%

### Caractéristiques Importantes
Les variables les plus influentes pour la qualité du vin sont :
1. La teneur en alcool
2. Les sulfates
3. L'acidité volatile

### Clustering
- Identification de segments distincts de vins avec des caractéristiques chimiques similaires
- Validation par multiple métriques (Silhouette, Davies-Bouldin, Calinski-Harabasz)

## 🛠 Technologies Utilisées
- Python 3.x
- Bibliothèques principales :
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn

## 📖 Guide d'Utilisation

1. Ouvrir le notebook `Wine_quality.ipynb`
2. Exécuter les cellules dans l'ordre pour reproduire l'analyse
3. Les visualisations et résultats seront générés automatiquement
4. Les modèles entraînés sont sauvegardés pour une utilisation ultérieure

## 🔍 Conclusions Clés

1. **Prédiction de Qualité** :
   - Les modèles d'ensemble (Bagging, Random Forest) montrent les meilleures performances
   - La teneur en alcool est le prédicteur le plus important de la qualité

2. **Segmentation** :
   - Les vins peuvent être regroupés en clusters distincts basés sur leurs propriétés chimiques
   - Chaque cluster présente des caractéristiques uniques de qualité

## 📝 Licence
Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.