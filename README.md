# support-ticket-analytics
# Support Ticket Analytics & Resolution Helper

## 1. Présentation du projet

Ce projet consiste à analyser des tickets de support client afin de mieux comprendre les demandes, identifier les problèmes récurrents et faciliter la recherche de solutions déjà apportées.

L'objectif est de construire une solution combinant Python, Google BigQuery et Power BI.

## 2. Source des données

**Dataset :** Multilingual Customer Support Tickets  

**[Voir la carte mentale du projet](https://fdesjardin92-web.github.io/support-ticket-analytics/)**

Le dataset contient des tickets de support client avec notamment :
- Subject : sujet de la demande
- Body : description du problème
- Answer : réponse de l'agent
- Type : type de ticket
- Queue : équipe responsable
- Priority : niveau de priorité
- Language : langue du ticket

Un échantillon d'environ 10 000 lignes sera utilisé pour le projet.

Les données seront téléchargées depuis Kaggle. Le fichier CSV ne sera pas directement intégré au dépôt GitHub.

## 3. Objectifs métier

- Mesurer le volume de tickets reçus.
- Identifier les catégories de demandes les plus fréquentes.
- Analyser la répartition des priorités.
- Identifier les équipes qui reçoivent le plus de tickets.
- Repérer les problèmes récurrents.
- Retrouver des tickets similaires et consulter les réponses précédentes.

## 4. Technologies utilisées

| Outil | Utilisation |
|---|---|
| Python / Pandas | Exploration, nettoyage et analyse des données |
| Google BigQuery | Stockage et interrogation des données avec SQL |
| Power BI | Création du tableau de bord interactif |
| GitHub | Documentation et partage du projet |

## 5. Étapes de réalisation

### Étape 1 — Récupération des données
- Télécharger le dataset depuis Kaggle.
- Sélectionner environ 10 000 lignes.
- Importer le fichier dans Python.

### Étape 2 — Exploration et nettoyage avec Python
- Examiner les colonnes et les types de données.
- Identifier les valeurs manquantes.
- Rechercher les doublons.
- Vérifier les catégories, les priorités et les langues.
- Préparer un fichier CSV propre.

### Étape 3 — Stockage dans BigQuery
- Créer un projet Google Cloud.
- Activer BigQuery.
- Créer les tables nécessaires.
- Importer les données nettoyées.
- Vérifier les données avec des requêtes SQL.

### Étape 4 — Analyse SQL
- Calculer le nombre total de tickets.
- Analyser les tickets par catégorie.
- Comparer les niveaux de priorité.
- Identifier les équipes les plus sollicitées.
- Repérer les demandes récurrentes.

### Étape 5 — Recherche de solutions avec Python
- Rechercher des tickets à partir de mots-clés.
- Filtrer les demandes par catégorie et priorité.
- Afficher les tickets similaires déjà traités.
- Présenter les réponses précédemment fournies par les agents.

Cette fonctionnalité reposera sur les informations existantes dans le dataset, sans entraîner de modèle de Machine Learning.

### Étape 6 — Visualisation avec Power BI
Créer un tableau de bord comprenant :
- Le nombre total de tickets.
- La répartition des tickets par priorité.
- Les principales catégories de demandes.
- Le volume de tickets par équipe.
- Les langues les plus représentées.
- Les tendances et problèmes récurrents.

### Étape 7 — Tests et présentation
- Vérifier les résultats des analyses.
- Contrôler la cohérence des indicateurs.
- Finaliser le tableau de bord.
- Documenter les résultats et les recommandations métier.

## 6. Planning prévisionnel — 2 semaines

| Période | Travaux |
|---|---|
| Jours 1 à 2 | Téléchargement et exploration des données |
| Jours 3 à 4 | Nettoyage et préparation avec Python |
| Jours 5 à 6 | Création des tables et import dans BigQuery |
| Jours 7 à 8 | Analyses SQL et indicateurs métier |
| Jours 9 à 10 | Recherche de solutions avec Python et dashboard Power BI |

## 7. Livrables attendus

- Un dataset préparé et documenté.
- Des notebooks Python.
- Des scripts SQL.
- Une fonctionnalité de recherche de tickets et de réponses.
- Un tableau de bord Power BI.
- Une documentation expliquant les étapes et les résultats.

## 8. Résultat attendu

À la fin du projet, l'utilisateur pourra consulter les indicateurs du support client, identifier les principales sources de demandes et retrouver plus facilement des réponses déjà apportées à des problèmes similaires.
