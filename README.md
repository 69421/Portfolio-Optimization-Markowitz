# 📊 Portfolio Optimization - Efficient Frontier Analysis

Ce projet implémente une analyse d'optimisation de portefeuille financier en utilisant Python. Il simule des milliers de portefeuilles possibles avec ventes à découvert autorisées et visualise la frontière efficiente pour aider à la prise de décision d'investissement.

## 🎯 Objectifs

- Analyser la performance historique de 5 ETFs majeurs
- Calculer les rendements moyens et matrices de covariance
- Simuler des portefeuilles avec différentes pondérations
- Identifier les portefeuilles optimaux selon le ratio de Sharpe
- Visualiser la frontière efficiente

## 📈 Données Utilisées

- **Période** : 1er janvier 2019 - 31 décembre 2023
- **Actifs** :
  - `SPY` (S&P 500 ETF)
  - `TLT` (iShares 20+ Year Treasury Bond ETF)
  - `GLD` (SPDR Gold Shares)
  - `QQQ` (Invesco QQQ Trust)
  - `EEM` (iShares MSCI Emerging Markets ETF)




### 3. Simulation Monte Carlo
- **10,000 portefeuilles** aléatoires
- Pondérations générées avec distribution normale
- **Ventes à découvert autorisées**
- Normalisation L1 des pondérations

### 4. Métriques de Performance
- 📈 **Rendement attendu** : `portfolio_return = np.dot(weights, mean_returns)`
- 📉 **Volatilité** : `np.sqrt(weights.T @ cov_matrix @ weights)`
- ⚡ **Ratio de Sharpe** : `portfolio_return / portfolio_volatility` (rf = 0%)

## 🎨 Visualisations

Graphique interactif Plotly montrant :
- **Axe X** : Volatilité (risque)
- **Axe Y** : Rendement attendu  
- **Couleur** : Ratio de Sharpe
- Chaque point représente un portefeuille simulé

## 🚀 Fonctionnalités Principales

| Fonctionnalité | Statut | Description |
|---------------|--------|-------------|
| Simulation Monte Carlo | ✅ | 10,000 portefeuilles simulés |
| Ventes à découvert | ✅ | Pondérations négatives autorisées |
| Visualisation interactive | ✅ | Graphique Plotly dynamique |
| Calculs statistiques | ✅ | Rendements, volatilité, Sharpe |
| Reproductibilité | ✅ | Seed aléatoire fixe |

```markdown
## 📁 Structure du Projet
Portfolio_Optimisation/
├── Portfolio_Optimisation.ipynb # Notebook principal
├── requirements.txt # Dépendances Python
├── README.md # Documentation
└── images/
└── efficient_frontier.png # Visualisations
```
## 🔧 Installation & Utilisation

### Prérequis
```bash
Python 3.12
Jupyter Notebook
```
### Installation
```bash
git clone https://github.com/votre-username/portfolio-optimization.git
cd portfolio-optimization
pip install -r requirements.txt
```
### Exécution
jupyter notebook Portfolio_Optimisation.ipynb



## 🔮 Extensions Futures

- [ ] Optimisation avec contraintes (sans vente à découvert)
- [ ] Ajout d'un taux sans risque
- [ ] Optimisation du ratio de Sharpe avec CVXPY
- [ ] Backtesting des stratégies optimales
- [ ] Analyse de sensibilité aux paramètres
- [ ] Interface utilisateur Streamlit

## 🤝 Contribution

Les contributions sont les bienvenues ! Voici comment participer :

1. 🍴 Fork le projet
2. 🌿 Créer une branche feature (`git checkout -b feature/AmazingFeature`)
3. 💾 Commit les changements (`git commit -m 'Add AmazingFeature'`)
4. 📤 Push vers la branche (`git push origin feature/AmazingFeature`)
5. 🔄 Ouvrir une Pull Request

## 📄 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 👨‍💻 Auteur

**Cheikh Abdou Mbacke**

## 🙏 Remerciements

- Yahoo Finance pour l'accès aux données historiques
- La communauté Python pour les excellentes bibliothèques
- Markowitz pour la théorie moderne du portefeuille

---

*Développé avec ❤️ pour la communauté finance quantitative*
```
