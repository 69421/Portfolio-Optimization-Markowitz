{\rtf1\ansi\ansicpg1252\cocoartf2709
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # \uc0\u55357 \u56520  Optimisation de Portefeuille avec la Fronti\'e8re Efficace de Markowitz\
\
## Description du Projet\
Ce projet Jupyter Notebook applique la Th\'e9orie Moderne du Portefeuille (TMP), d\'e9velopp\'e9e par Harry Markowitz, pour d\'e9terminer la **Fronti\'e8re Efficace** et identifier le **Portefeuille \'e0 Risque Minimum Global (Minimum Variance Portfolio)** et le **Portefeuille Optimal (Sharpe Ratio Maximum)**.\
Le projet analyse les cours historiques de 30 actions composant l'indice DJIA.\
\
### Objectifs\
- Calculer les rendements et les risques (volatilit\'e9) historiques.\
- Simuler des milliers de portefeuilles al\'e9atoires.\
- Utiliser l'optimisation quadratique (avec `cvxpy`) pour tracer la Fronti\'e8re Efficace.\
\
## Technologies Utilis\'e9es\
Ce projet a \'e9t\'e9 d\'e9velopp\'e9 en Python 3.x.\
\
### D\'e9pendances\
Pour ex\'e9cuter ce notebook, vous devez installer les librairies list\'e9es dans le fichier `requirements.txt` :\
```bash\
pip install -r requirements.txt}