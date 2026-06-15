# Grupo 7 — Predicción de Duración de Viajes Ecobici

Trabajo Práctico Final — Aprendizaje de Máquina  
Carrera de Especialización en Inteligencia Artificial (CEIA) — FIUBA

---

## Descripción del proyecto

Clasificación multiclase supervisada para predecir la duración de viajes
en el sistema de bicicletas públicas Ecobici (CABA).

**Clases objetivo:**
- `Corto` — menos de 10 minutos (período gratuito)
- `Mediano` — entre 10 y 30 minutos (uso típico)
- `Largo` — más de 30 minutos (genera cargo adicional)

**Dataset:** Buenos Aires Data — Viajes Ecobici históricos  
**Fuente:** https://data.buenosaires.gob.ar/dataset/bicicletas-publicas  
**Licencia:** CC BY 4.0

---

## Estructura del repositorio

| Carpeta | Contenido |
|---|---|
| `TPMAQ1_preparacion_datos/` | EDA, limpieza y feature engineering |
| `TPMAQ2_modelado_evaluacion/` | Modelos ML, optimización y evaluación |

---

## Resultados principales

| Modelo | F1-macro | Recall Largo |
|---|---|---|
| XGBoost (Optuna) | **0.7037** | 0.478 |
| Random Forest (Optuna) ★ | 0.7032 | **0.607** |
| CatBoost (default) | 0.6708 | 0.657 |
| LinearSVC (Optuna) | 0.6005 | 0.358 |
| Baseline Log. Reg. | 0.5960 | 0.589 |
| KNN (Optuna) | 0.5916 | 0.351 |

**Modelo recomendado:** Random Forest — mejor Recall en clase Largo (0.607),
el evento operativamente más costoso para el usuario.

---

## Integrantes

Grupo 7 — CEIA FIUBA
