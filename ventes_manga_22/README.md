# Projet de Récolte et d'Analyse des Ventes des Mangas dans le Monde - 2022

## Description
Ce projet a pour objectif de récolter, analyser et visualiser les données des ventes de mangas au niveau mondial et en France pour l'année 2022. Les données ont été collectées à partir de **Wikipedia** à l'aide de **web scraping** avec **Python** et **BeautifulSoup**, puis nettoyées et transformées pour être utilisées dans un **tableau de bord Power BI**. Ce tableau de bord permet de visualiser des indicateurs clés comme les chiffres d'affaires, le top 10 des mangas les plus vendus, ainsi que la répartition des ventes par genre et éditeur.

## Objectifs
- **Collecter** les données de vente des mangas en 2022 à partir de **Wikipedia** via **web scraping**.
- **Nettoyer** et **transformer** ces données avec **Python** pour faciliter leur analyse.
- **Visualiser** les données à l'aide d'un **tableau de bord Power BI** interactif.

## Technologies Utilisées
- **Python** : pour la collecte, le nettoyage et la transformation des données.
- **BeautifulSoup** : pour le web scraping des pages Wikipédia sur les ventes de mangas.
- **Pandas** : pour la manipulation des données (nettoyage, transformation).
- **Power BI** : pour la création du tableau de bord interactif.
  
## Structure du Projet
Le projet est organisé de la manière suivante :

```
/Manga-Sales-Analysis
│
├── static/
│   ├── data_mangas.xlsx           # Fichier Excel contenant les données de vente des mangas (nettoyées et transformées)
│
├── main/
│   ├── webscraping_mangas.ipynb   # Notebook Jupyter pour le web scraping et la collecte des données
│
├── dashboard_ventes_mangas_2022.pbix # Tableau de bord Power BI contenant la visualisation des données
│
├── README.md                      # Ce fichier
└── requirements.txt               # Liste des dépendances Python
```

## Collecte des Données
Les données ont été collectées via **web scraping** sur les pages Wikipédia concernant les ventes de mangas. Le fichier `webscraping_mangas.ipynb` contient le code Python utilisant la bibliothèque **BeautifulSoup** pour extraire les informations pertinentes (ventes mondiales et françaises, genre des mangas, éditeurs, etc.).

### Sources de données :
- Wikipédia

## Transformation des Données
Une fois les données extraites, elles ont été nettoyées et transformées à l'aide de **Pandas** dans le même notebook Jupyter. Le fichier `data_mangas.xlsx` contient les données nettoyées et prêtes pour l'analyse. Ces données sont structurées pour faciliter la visualisation dans le tableau de bord Power BI.

## Tableau de Bord Power BI
Un **tableau de bord Power BI** interactif a été créé pour afficher les informations suivantes :
- **Chiffre d'affaires (CA) en France** 
- **Top 10 des mangas les plus vendus en France**.
- **Nombre de mangas par genre** et **par éditeur**.
- **Nombre d'exemplaires vendus par éditeur** et **par genre**.
- **Répartition des ventes par genre**.

Le fichier **`dashboard_ventes_mangas_2022.pbix`** peut être ouvert avec **Power BI Desktop** pour explorer ces visualisations.

## Installation et Prérequis
1. Clonez ce dépôt sur votre machine locale :
   ```bash
   git clone https://github.com/AlyssaDerensy/Personal_Projects/tree/main/ventes_manga_22
   ```

2. Installez les dépendances Python :
   ```bash
   pip install -r requirements.txt
   ```

3. Lancez le notebook Jupyter pour effectuer le web scraping et générer le fichier Excel :
   ```bash
   jupyter notebook main/webscraping_mangas.ipynb
   ```

4. Ouvrez ensuite le fichier **`dashboard_ventes_mangas_2022.pbix`** dans **Power BI Desktop** pour explorer le tableau de bord interactif.


