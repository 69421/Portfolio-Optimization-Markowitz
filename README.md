

<h1 align="center">📈 Optimisation de Portefeuille avec la Théorie de Markowitz</h1>

<p align="center">
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white" alt="Python"></a>
  <a href="https://cvxpy.org/"><img src="https://img.shields.io/badge/CVXPY-Optimization-orange" alt="CVXPY"></a>
  <a href="https://matplotlib.org/"><img src="https://img.shields.io/badge/Matplotlib-Visualization-green" alt="Matplotlib"></a>
  <a href="https://plotly.com/"><img src="https://img.shields.io/badge/Plotly-Interactive-lightgrey?logo=plotly" alt="Plotly"></a>
  <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT License"></a>
</p>

---

Ce projet implémente l’**Optimisation de Portefeuille** basée sur la **Théorie Moderne du Portefeuille (MPT)** de Harry Markowitz.  
Il utilise des données de marché réelles (ETFs) et la bibliothèque de modélisation convexe **CVXPY** pour calculer la **frontière efficiente** et déterminer les **allocations optimales** sous différentes contraintes d’investissement.

---

### 🌟 Points Clés du Projet

- **Analyse de Rendement et de Risque** : Calcul des rendements, de la volatilité et de la matrice de covariance annualisés.  
- **Frontière Efficiente** : Simulation de milliers de portefeuilles aléatoires pour visualiser la relation risque-rendement.  
- **Optimisation Avancée** : Utilisation de la programmation convexe (**cvxpy**) pour résoudre des problèmes d’optimisation complexes.  
- **Stratégies Clés** : Détermination du portefeuille à **Ratio de Sharpe Maximum** et du **Portefeuille à Variance Minimum**.  

---

### 🛠️ Technologies Utilisées

- **Langage** : Python 3.12  
- **Analyse de données** : `pandas`, `numpy`  
- **Acquisition de données** : `yfinance`  
- **Optimisation** : `cvxpy`  
- **Visualisation** : `matplotlib`, `plotly`, `seaborn`  

---

### 📦 Structure du Répertoire

| Fichier | Description |
|----------|-------------|
| `Portfolio_optimisation_Python.ipynb` | Carnet Jupyter contenant l’acquisition des données, l’analyse statistique, la simulation et les scénarios d’optimisation avec CVXPY. |

---

### 🚀 Mise en Route

#### 1️⃣ Cloner le Dépôt
```bash
git clone https://github.com/69421/Portfolio-Optimization-Markowitz.git
cd Portfolio-Optimization-Markowitz
```

#### 2️⃣ Installer les Dépendances
Il est recommandé d’utiliser un environnement virtuel (venv ou conda).
```bash
pip install pandas numpy yfinance cvxpy matplotlib plotly
```

### 3️⃣ Exécuter l’Analyse
Ouvrez et exécutez le carnet Jupyter dans votre environnement préféré :
```bash
Portfolio_Optimisation.ipynb
```

### 📊 Scénarios d’Optimisation
Le projet calcule les poids optimaux pour 5 ETFs : SPY, TLT, GLD, QQQ, EEM,en utilisant des données historiques de 2018 à 2024, selon trois cas distincts :
| Objectif du Portefeuille      | Contraintes Clés                                                                 |
| ----------------------------- | -------------------------------------------------------------------------------- |
| **1. Max Sharpe Ratio**       | Poids pouvant être négatifs (shorting autorisé).                                 |
| **2. Min Variance**           | Investissement Long-Only (pas de shorting).                                      |
| **3. Min Variance (Bounded)** | Long-Only, rendement minimal (ex. 0.1% annuel), limites de poids (ex. 5% à 40%). |


### 📈 Exemple de Résultat (Synthèse)
Le carnet se termine par un tableau comparatif des performances des portefeuilles :
| Portefeuille                                           | Rendement Ann. | Volatilité Ann. | Ratio de Sharpe | SPY     | QQQ     | GLD     | TLT     | EEM     |
|:-------------------------------------------------------|:---------------:|:----------------:|:----------------:|:-------:|:-------:|:-------:|:-------:|:-------:|
| **Sharpe Maximal (Vente à découvert autorisée)**       | **1.3599**      | **1.0000**       | **1.3599**       | -5.0712 | 3.9383  | 4.1342  | 0.8844  | -2.8857 |
| **Sharpe Maximal (Long-only)**                         | **0.0970**      | **0.1095**       | **0.8862**       | 0.0000  | 0.4271  | 0.0000  | 0.3463  | 0.2266  |
| **Variance Minimale (Rendement ≥ 0.1%, bornes 5–50%)** | **0.0720**      | **0.1075**       | **0.6695**       | 0.0500  | 0.3246  | 0.0500  | 0.2120  | 0.3634  |


### 🎯 Perspective
Ce projet constitue une première étape vers la modélisation avancée du risque et de la performance financière.
Les prochaines évolutions envisagées incluent :
- L’intégration de mesures de risque alternatives (Value-at-Risk, CVaR).
- L’ajout de contraintes dynamiques basées sur la volatilité du marché.
- L’implémentation de modèles d’optimisation robustes pour données incertaines.
- La création d’un dashboard interactif pour visualiser la frontière efficiente en temps réel.
- L’exploration d’approches machine learning (par ex. clustering ou prédiction de rendements attendus).

Ce travail s’inscrit dans une démarche de recherche appliquée en finance quantitative et optimisation convexe.

### 📝 Licence
Ce projet est distribué sous la licence MIT.

### 💡 Auteur
Projet réalisé par **Cheikh Abdou Mbacke**,
dans le cadre d’une exploration pratique de la théorie moderne du portefeuille et de l’optimisation convexe.



