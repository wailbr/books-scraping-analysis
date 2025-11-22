🧠 Books Scraping & Data Analysis

Scraping → Cleaning → MySQL → Data Analysis (BooksToScrape project)

Ce projet met en place un pipeline complet de traitement de données e-commerce, depuis l’extraction de données brutes sur un site de livres jusqu’à leur nettoyage, stockage SQL et analyse statistique.

C’est un mini-projet parfait pour démontrer des compétences Data Engineer / Data Analyst :

✔ Web Scraping
✔ Nettoyage & Feature Engineering
✔ Base de données (MySQL)
✔ Visualisation & Analyse
✔ Architecture projet propre et modulaire

📁 1. Architecture du projet
books-scraping-analysis/
│
├── scraping/              → Extraction des données
│   ├── scapper.py
│   ├── books_toscrape.csv
│
├── cleaning/              → Nettoyage des données
│   ├── data_cleaning.py
│   ├── livres_nettoyes.csv
│
├── database/              → Base de données (MySQL)
│   ├── database_manager.py
│   ├── schema.sql
│
├── analysis/              → Analyse des données
│   ├── cleaned_data.csv
│   ├── test.py
│
├── docs/                  → Documentation
│   ├── README_original.md
│
├── main.py
├── requirements.txt
└── README.md

🕸️ 2. Scraping

Le script scapper.py extrait automatiquement les livres depuis BooksToScrape.com :

Données récupérées :

Nom du livre

Prix

Disponibilité

Catégorie

Note

Description

Résultat → books_toscrape.csv

Exécution :

cd scraping
python scapper.py

🧼 3. Cleaning

Le script data_cleaning.py :

Nettoie les colonnes

Convertit les types (prix → float, notes → int)

Supprime les valeurs manquantes

Formate le dataset pour MySQL

Sortie → livres_nettoyes.csv

Exécution :

cd cleaning
python data_cleaning.py

🗄️ 4. Stockage SQL (MySQL)

Le fichier schema.sql crée la structure SQL :

Table des livres

Contraintes

Index

Le script database_manager.py :

Connecte MySQL

Insère les livres nettoyés dans la base

Vérifie l’intégrité

Exécution :

cd database
python database_manager.py

📊 5. Analyse des données

Le script test.py analyse :

La répartition des prix

Le top catégories

Les notes les plus fréquentes

Le prix moyen par catégorie

Dataset utilisé → cleaned_data.csv

Exécution :

cd analysis
python test.py

🛠️ 6. Technologies utilisées

Python 3.x

pandas

BeautifulSoup

MySQL

matplotlib / seaborn

SQLSchema

Architecture modulaire

🎓 7. Compétences démontrées

✔ Web Scraping
✔ Data Cleaning & Manipulation
✔ SQL & Base de données
✔ Data Analysis
✔ Visualisation
✔ Organisation projet pro
✔ Documentation claire

👤 Auteur

Wail Brimesse
Bachelor Data & IA – ECE Paris
Recherche : Stage 6 mois (Data Engineer / Data Analyst / Data Scientist) – Mars 2026

🚀 8. Améliorations possibles

Déploiement d’un dashboard Streamlit

Ajout d’un pipeline ETL automatique

Intégration Airflow

Ajout d’indicateurs avancés
