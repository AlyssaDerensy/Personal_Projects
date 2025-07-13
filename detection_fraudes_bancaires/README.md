# Détection de Fraude sur les Transactions par Carte Bancaire

## Description

Ce projet a pour objectif de détecter les transactions frauduleuses à partir d'un jeu de données de transactions par carte bancaire. Il s'appuie sur des techniques de machine learning supervisé, notamment la régression logistique et les forêts aléatoires, pour identifier efficacement les fraudes malgré un fort déséquilibre des classes.

## Données

Le jeu de données utilisé provient d'un ensemble de transactions réalisées par des titulaires de cartes européennes en septembre 2013. Il contient :

- 284 807 transactions
- 492 fraudes (soit environ 0.17 % du total)
- Des variables anonymisées (V1 à V28), ainsi que le montant, le temps, et la variable cible `Class` (0 pour non frauduleux, 1 pour frauduleux)

## Étapes du projet

1. **Importation et exploration des données**
   - Chargement du dataset
   - Analyse du déséquilibre de classes
   - Inspection des corrélations et des valeurs manquantes

2. **Prétraitement**
   - Normalisation des données
   - Application de SMOTE (Synthetic Minority Over-sampling Technique) pour équilibrer les classes

3. **Modélisation**
   - Entraînement d'un modèle de régression logistique
   - Entraînement d'un modèle de forêt aléatoire
   - Évaluation avec les métriques suivantes :
     - Matrice de confusion
     - Rapport de classification
     - AUC (Area Under Curve)

## Installation

Cloner le dépôt Git :

```bash
git clone https://github.com/AlyssaDerensy/Personal_Projects/detection_fraudes_bancaires
cd detection_fraudes_bancaires

python -m venv env
env\\Scripts\\activate

pip install -r requirements.txt
