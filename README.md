# 🌫️ Beijing Air Quality Prediction

## 📖 Description
Projet de Machine Learning pour prédire les concentrations horaires de PM2.5 à Pékin à partir de données multi-sources (2013-2017). Développé dans le cadre du cours Data Driven Decision Making à l'École Centrale Casablanca.

**Problématique** : Anticiper les pics de pollution pour permettre des interventions proactives.  
**Solution** : Pipeline complet de data science incluant :
- Nettoyage des données (20k+ valeurs manquantes traitées)
- Feature engineering (variables cycliques, agrégations temporelles)
- Comparaison de 5 modèles de régression
- Visualisations interactives

## 🏆 Résultats Principaux
| Modèle                  | RMSE (µg/m³) | MAE (µg/m³) | R² Score |
|-------------------------|--------------|-------------|----------|
| RandomForestRegressor   | **29.39**    | **18.11**   | 0.862    |
| GradientBoosting        | 40.11        | 25.52       | 0.746    |
| KNN                     | 39.52        | 24.09       | 0.756    |

**Key Insights** :
- 🔥 Pics hivernaux (2× supérieurs aux niveaux estivaux)
- 🚗 Corrélation trafic-pollution (NO₂/CO → PM2.5 ρ > 0.7)
- 🌬️ Impact météo : Température (-), Humidité (+)

## 🛠️ Installation
```bash
git clone https://github.com/votre_repo/air-quality-prediction.git
cd air-quality-prediction
pip install -r requirements.txt