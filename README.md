# Analyse et Modélisation des Trajets des Taxis Jaunes de New York

Projet de fin de session — L3 DANT — Introduction à la Data Science — Hiver 2026

## Structure du projet

```
Taxi-NYC/
├── data/               # Données brutes (non versionnées)
├── notebooks/          # Notebooks Jupyter par étape
├── src/                # Scripts Python utilitaires
├── figures/            # Visualisations exportées
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

Télécharger un fichier `.parquet` mensuel et le placer dans `data/`.

## Étapes du projet

| # | Notebook | Description |
|---|----------|-------------|
| 01 | `01_EDA.ipynb` | Exploration et nettoyage des données |
| 02 | `02_feature_engineering.ipynb` | Création des variables |
| 03 | `03_supervised_learning.ipynb` | Apprentissage supervisé |
| 04 | `04_unsupervised_learning.ipynb` | Clustering |

## Auteur

Maissa Saci — L3 DANT — 2026
