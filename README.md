# Prédiction de Souscription à un Dépôt à Terme - Bank Marketing Dataset

##  Contexte

Ce projet utilise un jeu de données issu de campagnes de marketing téléphonique réalisées par une institution bancaire. L’objectif est de prédire si un client va **souscrire à un dépôt à terme (term deposit)** en se basant sur ses caractéristiques sociodémographiques, ses relations avec la banque, et l’historique des campagnes précédentes.

---

##  Objectifs

- Comprendre les facteurs influençant la souscription au produit bancaire.
- Mettre en place plusieurs **modèles de Machine Learning** pour prédire la variable cible `y`.
- Identifier les variables les plus importantes pour guider les décisions marketing.
- Segmenter les clients grâce au **clustering** pour des campagnes plus ciblées.

---

##  Description des variables

###  Données clients :
| Variable     | Description                              | Type        |
|--------------|------------------------------------------|-------------|
| `age`        | Âge du client                            | Numérique   |
| `job`        | Type d’emploi                            | Catégorielle|
| `marital`    | Statut matrimonial                       | Catégorielle|
| `education`  | Niveau d'éducation                       | Catégorielle|
| `default`    | A des crédits en défaut ?                | Binaire     |
| `balance`    | Solde annuel moyen (en euros)            | Numérique   |
| `housing`    | A un prêt immobilier ?                   | Binaire     |
| `loan`       | A un prêt personnel ?                    | Binaire     |

###  Données sur le dernier contact :
| Variable     | Description                              | Type        |
|--------------|------------------------------------------|-------------|
| `contact`    | Type de contact                          | Catégorielle|
| `day`        | Jour du mois du dernier contact          | Numérique   |
| `month`      | Mois du dernier contact                  | Catégorielle|
| `duration`   | Durée du dernier contact (en secondes)   | Numérique   |

###  Autres caractéristiques :
| Variable     | Description                                         | Type        |
|--------------|-----------------------------------------------------|-------------|
| `campaign`   | Nb de contacts durant cette campagne                | Numérique   |
| `pdays`      | Nb de jours depuis le dernier contact précédent     | Numérique   |
| `previous`   | Nb de contacts lors de campagnes précédentes        | Numérique   |
| `poutcome`   | Résultat de la campagne précédente                  | Catégorielle|

### Variable cible :
| Variable | Description                                | Type    |
|----------|--------------------------------------------|---------|
| `y`      | Le client a-t-il souscrit un dépôt à terme ? | Binaire (`1 = non`, `2 = oui`) |

---

##  Étapes du projet

1. **Analyse exploratoire des données** :
   - Statistiques descriptives, visualisations, distribution des classes.

2. **Prétraitement des données** :
   - Encodage des variables catégorielles, gestion des valeurs manquantes, normalisation.

3. **Modélisation** :
   - Entraînement de plusieurs modèles de Machine Learning :
     - Logistic Regression
     - Random Forest
     - XGBoost
     - SVM, etc.
   - Évaluation avec :
     - Matrice de confusion
     - Courbe ROC / AUC
     - Précision, Rappel, F1-score

4. **Interprétation des résultats** :
   - Analyse des variables les plus influentes
   - Sélection du **modèle champion**

5. **Clustering (segmentation)** :
   - Regroupement des clients selon des profils similaires
   - Analyse descriptive par cluster

6. **Stratégies marketing recommandées** :
   - Plan d’action personnalisé par segment

---

##  Outils & Librairies

- Python (pandas, scikit-learn, seaborn, matplotlib, xgboost)
- Jupyter Notebook
- Power BI (pour les visualisations de synthèse)
- Git & GitHub (versioning)

---

##  Organisation du projet

| Dossier/Fichier  | Description                                      |
|------------------|------------------------------------------------|
| `data/`          | Données brutes ou prétraitées                   |
| `notebooks/`     | Analyse exploratoire, modélisation, clustering |
| `README.md`      | Présentation générale du projet                  |


## Auteur

**Mahamadou Sangaré**  
Master 1 Data Science, Big Data & IA  
[LinkedIn](https://www.linkedin.com/in/mahamadou-sangare-b53b7b351)