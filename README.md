# Extraction de données boursières par Web Scraping

Ce projet a été réalisé dans le cadre du cours **[Python Project for Data Science](https://www.coursera.org/learn/python-project-for-data-science/home/welcome)**, proposé par IBM sur Coursera, dans le cadre de la formation pour devenir **Data Scientist (IBM Data Science)**.

## Description

Le notebook `Final_Assignment_Webscraping.ipynb` a pour objectif d'extraire des données financières historiques à partir d'une page web, en utilisant des techniques de **web scraping**, dans un contexte où ces données ne sont pas disponibles via une API.

Le notebook s'appuie sur l'exemple des données boursières de **Netflix** pour illustrer la méthode, puis propose un exercice pratique sur les données boursières d'**Amazon**.

## Objectifs pédagogiques

- Envoyer une requête HTTP vers une page web avec la librairie `requests`
- Analyser (parser) le contenu HTML d'une page avec `BeautifulSoup`
- Identifier les balises HTML contenant les données à extraire (tableau)
- Extraire les données et construire un `DataFrame` pandas
- Extraire des tableaux HTML directement avec `pandas.read_html()`

## Étapes suivies dans le notebook

1. **Installation et import des librairies** : `pandas`, `requests`, `bs4` (BeautifulSoup), `html5lib`, `lxml`, `plotly`
2. **Extraction avec BeautifulSoup**
   - Téléchargement de la page web via `requests.get()`
   - Analyse du HTML avec `BeautifulSoup`
   - Repérage des balises `<table>`, `<tr>`, `<td>` contenant les données boursières
   - Construction d'un DataFrame avec les colonnes : `Date`, `Open`, `High`, `Low`, `Close`, `Volume`
3. **Extraction avec pandas**
   - Utilisation de `pandas.read_html()` pour extraire directement le tableau HTML
4. **Exercice pratique**
   - Application de la même méthode sur une page contenant les données boursières d'Amazon
   - Réponses à des questions sur le DataFrame obtenu (aperçu des données, noms des colonnes, dernière valeur d'ouverture, etc.)

## Bibliothèques utilisées

- `pandas`
- `requests`
- `beautifulsoup4` (`bs4`)
- `html5lib`
- `lxml`
- `plotly`

## Utilisation

1. Ouvrir le notebook dans Jupyter Notebook / JupyterLab.
2. Exécuter les cellules dans l'ordre, en commençant par l'installation des dépendances.
3. Le notebook télécharge automatiquement les pages HTML d'exemple utilisées pour le scraping (aucun fichier externe à fournir).

## Contexte

Ce notebook a été fourni et complété dans le cadre du cours **Python Project for Data Science** de la spécialisation **IBM Data Science** sur Coursera. Le contenu de base (structure, exemples, jeux de données) est fourni par IBM (© IBM Corporation), les parties complétées correspondent aux exercices demandés dans le cadre de l'évaluation finale du cours.

## Auteur

Notebook complété par l'utilisateur dans le cadre de sa formation Data Science (IBM / Coursera).
