# 📊 Customer Segmentation RFM & API Pipeline

## 🎯 Présentation du Projet
Ce projet automatise l'analyse de segmentation client (RFM) en récupérant des données en temps réel via une API. L'objectif est de transformer des données brutes de transactions en segments actionnables pour optimiser les stratégies marketing.

## 🚀 Fonctionnalités Clés
* **Extraction API :** Collecte automatisée des données transactionnelles (Python `requests`).
* **Data Cleaning :** Traitement des types de données, gestion des doublons et des valeurs manquantes avec `Pandas`.
* **Analyse RFM :** Calcul des scores de Récence, Fréquence et Montant.
* **Visualisation :** Création de dashboards de segmentation avec `Seaborn` et `Matplotlib`.

## 🛠️ Stack Technique
* **Langage :** Python 3.x
* **Librairies :** Pandas, NumPy, Matplotlib, Seaborn, Requests.
* **Environnement :** Jupyter Notebook / VS Code.

## 📡 Détails de l'intégration API
Le script se connecte à l'API ["https://dummyjson.com/users?limit=400"] pour récupérer les données. 
> **Note :** Pour des raisons de sécurité, les clés d'API ne sont pas incluses dans ce dépôt. Utilisez un fichier `.env` pour vos propres tests.

```python
# Exemple de la logique d'appel utilisée
response = requests.get(url, headers=headers)
data = response.json()
