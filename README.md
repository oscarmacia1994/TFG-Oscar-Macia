# Estudio comparativo de modelos de aprendizaje automático

Repositorio asociado al Trabajo Fin de Grado de **Óscar Maciá Moreno**, realizado en el Grado en Estadística Empresarial de la Universidad Miguel Hernández durante el curso 2025-2026.

## Descripción

Este proyecto presenta un estudio comparativo de distintos modelos de aprendizaje automático basados en árboles de decisión:

- CART.
- Bagging con CART.
- Random Forest.
- Extra Trees.
- AdaBoost.
- Gradient Boosting.
- XGBoost.
- LightGBM.
- CatBoost.

Los modelos se aplican a dos tipos de problemas:

- Clasificación binaria con el conjunto de datos Bank Marketing.
- Regresión temporal con el conjunto de datos Individual Household Electric Power Consumption.

El estudio incluye el preprocesamiento de los datos, el ajuste de los modelos, la búsqueda de hiperparámetros, la validación y la comparación final de los resultados.

## Estructura del repositorio

```text
TFG-Oscar-Macia/
├── data/
│   └── README.md
├── notebooks/
│   ├── README.md
│   └── comparativa_modelos/
│       ├── 01_preprocesamiento_bank_marketing.ipynb
│       ├── 02_preprocesamiento_consumo_electrico.ipynb
│       ├── 03_modelos_cart.ipynb
│       ├── 04_modelos_bagging.ipynb
│       ├── 05_modelos_boosting.ipynb
│       └── 06_comparacion_computacional.ipynb
├── .gitignore
├── README.md
└── requirements.txt
```

## Cuadernos computacionales

Los cuadernos deben ejecutarse en el siguiente orden:

1. `01_preprocesamiento_bank_marketing.ipynb`
2. `02_preprocesamiento_consumo_electrico.ipynb`
3. `03_modelos_cart.ipynb`
4. `04_modelos_bagging.ipynb`
5. `05_modelos_boosting.ipynb`
6. `06_comparacion_computacional.ipynb`

Los dos primeros cuadernos realizan el preprocesamiento de los conjuntos de datos. Los siguientes ajustan y evalúan los modelos CART, bagging y boosting. El último reúne los resultados y realiza la comparación final.

## Conjuntos de datos

Los conjuntos de datos originales no se incluyen directamente en este repositorio.

Las instrucciones para descargarlos y colocarlos en las rutas esperadas se encuentran en:

```text
data/README.md
```

Los conjuntos utilizados son:

- Bank Marketing.
- Individual Household Electric Power Consumption.

Ambos proceden del UCI Machine Learning Repository.

## Instalación

Clonar el repositorio:

```bash
git clone https://github.com/oscarmacia1994/TFG-Oscar-Macia.git
cd TFG-Oscar-Macia
```

Crear un entorno virtual:

```bash
python -m venv .venv
```

Activarlo en Windows:

```bash
.venv\Scripts\activate
```

Instalar las dependencias:

```bash
pip install -r requirements.txt
```

## Ejecución

Una vez descargados y colocados los conjuntos de datos, iniciar Jupyter:

```bash
jupyter notebook
```

Después, acceder a la carpeta:

```text
notebooks/comparativa_modelos/
```

y ejecutar los cuadernos en el orden indicado.

## Metodología

En el problema de clasificación se utiliza como métrica principal el F1 de la clase positiva, acompañado del área bajo la curva ROC.

En el problema de regresión se utiliza el RMSE como métrica principal y el coeficiente de determinación R² como métrica complementaria.

La validación de los modelos de clasificación se realiza mediante validación cruzada estratificada. En regresión se emplea validación temporal para preservar el orden cronológico de las observaciones.

## Autor

**Óscar Maciá Moreno**

Trabajo Fin de Grado  
Grado en Estadística Empresarial  
Universidad Miguel Hernández  
Curso 2025-2026
