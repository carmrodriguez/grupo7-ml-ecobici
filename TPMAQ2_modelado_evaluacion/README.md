# TPMAQ2 — Modelado y Evaluación

## Archivos

| Archivo | Descripción |
|---|---|
| `TPMAQ2_V2.ipynb` | Notebook principal con todos los modelos |
| `Ecobici_ML_V2.pptx` | Presentación ejecutiva del proyecto |

## Modelos implementados

1. Baseline — Regresión Logística Multinomial
2. KNN con optimización Optuna
3. LinearSVC con optimización Optuna
4. Random Forest con optimización Optuna ★
5. XGBoost con optimización Optuna
6. CatBoost (experimento adicional)

## Métricas principales

- **Métrica principal:** F1-macro
- **Métrica operativa:** Recall de clase Largo
- **Evaluación:** test set completo (~975k muestras)

## Requisitos

- Python 3.10+
- scikit-learn, xgboost, catboost, optuna, pandas, numpy, matplotlib, seaborn

Instalar con: `pip install -r requirements.txt`
