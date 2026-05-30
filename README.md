# Analyse et Modélisation des Trajets des Taxis Jaunes de New York

Projet de fin de session — L3 DANT — Introduction à la Data Science 

## Équipe

Projet réalisé en **binôme** :

| Étudiante | Branche de travail |
|---|---|
| **Maissa Saci** | `maissa/main` |
| **Sara AitOuahioune** | `sara/main` |


## Structure du projet

```
Taxi-NYC/
├── data/               # Données brutes (non versionnées, fichier .parquet à télécharger)
├── notebooks/          # Notebooks Jupyter par étape
│   ├── 01_EDA.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_supervised_learning.ipynb
│   └── 04_unsupervised_learning.ipynb
├── figures/            # Visualisations exportées automatiquement
├── requirements.txt    # Dépendances Python
└── README.md
```

## Installation

```bash
pip install -r requirements.txt
```

## Source des données

- [TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- [Kaggle NYC Yellow Taxi](https://www.kaggle.com/datasets/elemento/nyc-yellow-taxi-trip-data)

Télécharger un fichier `.parquet` mensuel (ex : janvier 2026) et le placer dans `data/` sous le nom `yellow_tripdata.parquet`.

## Étapes du projet

| # | Notebook | Description | Tickets |
|---|----------|-------------|---------|
| 01 | `01_EDA.ipynb` | Exploration et nettoyage des données | T-02, T-03, T-04 |
| 02 | `02_feature_engineering.ipynb` | Création des variables dérivées | T-05, T-06 |
| 03 | `03_supervised_learning.ipynb` | Régression — prédiction du montant | T-07, T-08, T-09 |
| 04 | `04_unsupervised_learning.ipynb` | Clustering K-Means + PCA | T-10, T-11 |

Les notebooks doivent être exécutés **dans l'ordre** : chacun lit le fichier produit par le précédent.

## Résultats principaux

**Apprentissage supervisé** (prédiction de `total_amount`) :

| Modèle | RMSE | MAE | R² |
|---|---|---|---|
| Régression Linéaire | 7.87 $ | 3.37 $ | 0.874 |
| Random Forest | 6.50 $ | 2.92 $ | 0.914 |
| Gradient Boosting | 6.34 $ | 2.82 $ | 0.918 |

**Apprentissage non supervisé** : segmentation en 4 profils de trajets par K-Means (navetteur, aéroport, noctambule, heure de pointe).
