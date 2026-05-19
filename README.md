# Segundo_corte_2026
Repositorio para segundo corte 2026-1 

# Actividad: Introducción a Pandas en Python

## Descripción de la actividad

Esta actividad tiene como finalidad aplicar conceptos básicos de la librería Pandas utilizando Python en Google Colab. Durante el desarrollo se realizaron ejercicios relacionados con la creación de DataFrames, operaciones entre columnas, lectura de archivos CSV y manejo de datos sintéticos.

El trabajo fue desarrollado en un Notebook de Google Colab y posteriormente almacenado en un repositorio de GitHub como evidencia práctica del aprendizaje adquirido.

---

# Objetivo

Comprender y aplicar las funciones básicas de la librería Pandas para el análisis y manipulación de datos mediante ejercicios prácticos en Python.

---

# Temas investigados

Durante la actividad se investigaron los siguientes temas:

- ¿Qué es Pandas?
- Importancia de Pandas en el análisis de datos.
- Uso de DataFrames.
- Operaciones matemáticas entre columnas.
- Lectura de archivos CSV.
- Generación y manipulación de datos sintéticos.
- Uso de Google Colab.
- Integración de proyectos con GitHub.

---

# Herramientas utilizadas

- Python
- Pandas
- NumPy
- Google Colab
- GitHub

---

# Desarrollo de la actividad

## 1. Importación de librerías

Se importaron las librerías necesarias para el desarrollo de la actividad.

```python
import pandas as pd
import numpy as np
```

---

## 2. Creación de un DataFrame

Se creó un DataFrame con información de productos, precios y cantidades.

```python
datos = {
    "Producto": ["Laptop", "Mouse", "Teclado"],
    "Precio": [2500, 80, 150],
    "Cantidad": [3, 10, 5]
}

df = pd.DataFrame(datos)

print(df)
```

### Resultado

| Producto | Precio | Cantidad |
|----------|--------|----------|
| Laptop | 2500 | 3 |
| Mouse | 80 | 10 |
| Teclado | 150 | 5 |

---

## 3. Operaciones entre columnas

Se realizó una multiplicación entre las columnas `Precio` y `Cantidad` para calcular el total de ventas.

```python
df["Total"] = df["Precio"] * df["Cantidad"]

print(df)
```

### Resultado

| Producto | Precio | Cantidad | Total |
|----------|--------|----------|------|
| Laptop | 2500 | 3 | 7500 |
| Mouse | 80 | 10 | 800 |
| Teclado | 150 | 5 | 750 |

---

## 4. Lectura de archivos CSV

Se realizó la lectura de un archivo CSV utilizando Pandas.

```python
archivo = pd.read_csv("ventas.csv")

print(archivo.head())
```

### Explicación

El método `read_csv()` permite importar archivos CSV para analizarlos y manipularlos dentro de Python.

---

## 5. Trabajo con datos sintéticos

Se generaron datos aleatorios utilizando NumPy para simular información ficticia.

```python
datos_sinteticos = {
    "ID": range(1,11),
    "Edad": np.random.randint(18,60,10),
    "Salario": np.random.randint(1000,5000,10)
}

df_sintetico = pd.DataFrame(datos_sinteticos)

print(df_sintetico)
```

### Resultado

| ID | Edad | Salario |
|----|------|---------|
| 1 | 25 | 3200 |
| 2 | 41 | 2800 |
| ... | ... | ... |

---

# Capturas o resultados obtenidos

## Ejemplo de DataFrame generado

*(Aquí puedes insertar capturas de pantalla de Google Colab mostrando los resultados obtenidos.)*

Ejemplo:

- Captura de creación del DataFrame.
- Captura de operaciones entre columnas.
- Captura de lectura del CSV.
- Captura de datos sintéticos.

---

# Conclusiones

- Pandas es una herramienta fundamental para el análisis y manipulación de datos en Python.
- Los DataFrames permiten organizar información de forma eficiente y similar a una hoja de cálculo.
- Las operaciones entre columnas facilitan el análisis matemático y estadístico.
- Los archivos CSV son ampliamente utilizados para almacenar y compartir datos.
- Los datos sintéticos permiten realizar pruebas y simulaciones en proyectos de análisis de datos e Inteligencia Artificial.
- Google Colab facilita el desarrollo de proyectos sin necesidad de instalar software adicional.

---

# Referencias bibliográficas

- McKinney, W. (2022). *Python for Data Analysis*. O'Reilly Media.
- VanderPlas, J. (2016). *Python Data Science Handbook*. O'Reilly Media.

---

# Enlaces oficiales

- https://pandas.pydata.org/
- https://colab.research.google.com/
- https://github.com/
