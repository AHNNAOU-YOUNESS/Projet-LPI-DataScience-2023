# Analyse de la performance logistique des pays — LPI 2023

## 1. Présentation du projet

Ce projet de Data Science vise à analyser et à regrouper différents pays selon leur performance logistique, à partir des données du **Logistics Performance Index (LPI) 2023** publiées par la Banque mondiale.

L'objectif principal est d'identifier des groupes de pays présentant des caractéristiques logistiques similaires à travers une approche de clustering non supervisé.

## 2. Problématique

Comment les pays peuvent-ils être regroupés en fonction des six composantes de leur performance logistique, selon les données du Logistics Performance Index (LPI) 2023 ?

## 3. Données utilisées

Les données proviennent de la Banque mondiale et portent sur le Logistics Performance Index 2023.

L'analyse repose sur les six composantes suivantes :

- Customs
- Infrastructure
- International Shipments
- Logistics Competence and Quality
- Tracking and Tracing
- Timeliness

L'échantillon final comprend 139 pays. Les scores des six composantes sont exprimés sur une échelle de 1 à 5.

## 4. Méthodologie

Le projet suit les principales étapes d'une démarche de Data Science :

1. Acquisition et chargement des données.
2. Exploration et compréhension du dataset.
3. Nettoyage et préparation des données.
4. Analyse exploratoire des données (EDA).
5. Sélection des six variables utilisées pour le clustering.
6. Standardisation des variables avec StandardScaler.
7. Application et comparaison de méthodes de clustering.
8. Évaluation des modèles à l'aide de métriques internes.
9. Réduction de dimensionnalité par ACP pour la visualisation.
10. Interprétation économique des groupes obtenus.

Le modèle final retenu pour l'interprétation économique est K-Means avec trois clusters.

## 5. Résultats principaux

La segmentation finale distingue trois catégories de performance logistique :

- **Faible performance :** 61 pays (43,88 %).
- **Performance intermédiaire :** 41 pays (29,50 %).
- **Performance élevée :** 37 pays (26,62 %).

Le choix de trois clusters vise à obtenir une segmentation plus détaillée et plus pertinente pour l'interprétation économique, même si la configuration à deux clusters présente de meilleurs résultats selon les métriques statistiques étudiées.

## 6. Structure du dépôt

- `notebook/` : notebook Jupyter contenant les étapes de l'analyse.
- `data/` : fichier de données utilisé.
- `figures/` : visualisations produites durant l'étude.
- `rapport/` : rapport final en LaTeX et en PDF.
- `presentation/` : support de présentation.
- `requirements.txt` : bibliothèques Python nécessaires à l'exécution du projet.

## 7. Exécution du projet

Le notebook peut être consulté et exécuté avec Google Colab.

Avant l'exécution, il faut s'assurer que le fichier de données `WB_LPI.csv` est disponible à l'emplacement indiqué dans le notebook.

Les bibliothèques nécessaires sont répertoriées dans le fichier `requirements.txt`.

## 8. Outils utilisés

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Git et GitHub
- LaTeX

## 9. Membres du binôme

- **AHNNAOU Youness**
- **AIT BOUSSALEM Israa**

## 10. Source des données

Banque mondiale — Logistics Performance Index (LPI) 2023.

https://lpi.worldbank.org/

