# Conjuntos de datos

Los conjuntos de datos originales utilizados en este proyecto no se incluyen en el repositorio. Deben descargarse desde el UCI Machine Learning Repository y colocarse en las rutas indicadas antes de ejecutar los cuadernos.

## 1. Bank Marketing

Página del conjunto de datos:

https://archive.ics.uci.edu/dataset/222/bank+marketing

Tras descargar y descomprimir el conjunto de datos, el archivo `bank-full.csv` debe colocarse en:

```text
data/raw/clasificacion/bank-full.csv
```

## 2. Individual Household Electric Power Consumption

Página del conjunto de datos:

https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption

Tras descargar y descomprimir el conjunto de datos, el archivo `household_power_consumption.txt` debe colocarse en:

```text
data/raw/regresion/household_power_consumption.txt
```

## Estructura esperada

```text
data/
├── README.md
└── raw/
    ├── clasificacion/
    │   └── bank-full.csv
    └── regresion/
        └── household_power_consumption.txt
```

Una vez colocados los archivos, los cuadernos deben ejecutarse en orden desde la carpeta `notebooks/comparativa_modelos`.
