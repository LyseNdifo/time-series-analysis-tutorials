# Tutoriel d’analyse de séries temporelles en R

Ce dépôt présente un ensemble de techniques d’analyse et de prévision de séries temporelles en R. Il couvre les approches classiques (SARIMA, régression dynamique) ainsi que des méthodes modernes (Prophet), avec une comparaison systématique des performances.

L’objectif est de fournir un tutoriel clair, reproductible et pédagogique pour comprendre et appliquer les principaux modèles de forecasting.


## 🎯 Objectifs du projet

- Identifier et ajuster des modèles **SARIMA** (manuels et automatiques).  
- Comparer les performances via AIC, BIC, RMSE, MAE, MAPE.  
- Diagnostiquer les résidus et valider les modèles.  
- Construire une **régression dynamique** avec erreurs ARIMA.  
- Simuler plusieurs **scénarios de prévision** (hausse, baisse, constant).  
- Utiliser **Prophet** pour modéliser tendances et saisonnalités complexes.  
- Réaliser un **benchmark SARIMA vs Prophet**.  
- Résoudre un défi de prévision sur données trimestrielles.


## 📁 Contenu du dépôt
```
time-series-analysis-tutorials/
├── README.md
├── notebook/
    └── Lab_time_series_analysis.ipynb
```


## 🧠 Méthodes étudiées

### **1. SARIMA**
- Transformation Box‑Cox  
- Différenciation saisonnière et non saisonnière  
- Identification via ACF/PACF  
- Modèles manuels :  
  - SARIMA(2,0,0)(0,1,0)\_12  
  - SARIMA(0,0,2)(0,1,0)\_12  
- Modèle automatique :  
  - SARIMA(2,0,0)(0,1,1)\_12 avec drift  
- Comparaison AIC / BIC / erreurs  
- Analyse des résidus (Ljung‑Box)

### **2. Régression dynamique**
- Détection de régression fallacieuse  
- Modèle ARIMA avec variable explicative  
- Validation des résidus  
- Prévisions sous trois scénarios :  
  - budget constant  
  - budget haut  
  - budget bas  

### **3. Prophet**
- Préparation des données (format ds / y)  
- Modèle Prophet standard  
- Prévisions à 30 jours  
- Décomposition : tendance, hebdomadaire, annuelle  
- Comparaison Prophet vs SARIMA  

### **4. Défi de prévision**
- Série NSWMetro (visnights)  
- Analyse de la saisonnalité  
- Split train/test  
- auto.arima vs ARIMA manuel  
- Prévision sur 2 ans  


## 📈 Visualisations incluses

- Graphiques de séries temporelles  
- ACF / PACF  
- Diagnostics des résidus  
- Prévisions multi‑scénarios  
- Composantes Prophet  
- Comparaison des modèles  
- Prévisions sur données trimestrielles  


## 🛠️ Technologies utilisées

- **R**  
- forecast  
- fma  
- fpp2  
- prophet  
- ggplot2  


## 📚 Références

- Hyndman, R.J., & Athanasopoulos, G. (2021). *Forecasting: Principles and Practice (3rd ed).* Monash University, Australia. 
- Documentation R : forecast, prophet, fpp2  


