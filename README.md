# TP2 - Machine Learning  
## Classification de Maladies avec un SVM

### 🎯 Objectif de l'exercice

L'objectif de cet exercice est d'appliquer un **modèle de Support Vector Machine (SVM)** afin de classifier différentes **maladies** à partir des **symptômes** présentés par les patients. Ce travail s'inscrit dans le cadre du **TP2 du cours de Machine Learning**.

### 📊 Description des données

Le dataset utilisé, `DiseaseAndSymptoms.csv`, contient des informations sur :
- des **maladies diagnostiquées** (variable cible),
- les **symptômes observés** pour chaque patient (jusqu'à 4 par individu).

Ce jeu de données a été récupéré sur [Kaggle](https://www.kaggle.com/) (lien à ajouter si nécessaire).

### 🛠️ Étapes du TP

1. **Chargement et sélection des colonnes pertinentes**
   - Colonnes utilisées : `Disease`, `Symptom_1`, `Symptom_2`, `Symptom_3`, `Symptom_4`

2. **Prétraitement des données**
   - Suppression des valeurs manquantes
   - Encodage des maladies avec `LabelEncoder`
   - Encodage one-hot des symptômes

3. **Préparation des données**
   - Séparation des features (`X`) et de la cible (`y`)
   - Découpage en ensemble d'entraînement et de test (80/20)

4. **Entraînement du modèle**
   - Utilisation d’un modèle `SVC` (Support Vector Classifier) avec noyau linéaire
   - Approche **One-vs-Rest** pour la classification multiclasse

5. **Évaluation**
   - Calcul de la précision (`accuracy`)
   - Affichage d’un rapport de classification (précision, rappel, F1-score)

### 🧰 Technologies utilisées

- Python 3
- Bibliothèques :
  - `pandas`
  - `numpy`
  - `scikit-learn`
