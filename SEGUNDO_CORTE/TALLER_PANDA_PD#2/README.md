**# Taller de Inteligencia Artificial (Librería Pandas) - Corte II 🚀
**Programa de Ingeniería de Sistemas** | *Universidad del Pacífico*

---

## 📝 Descripción del Proyecto
Este repositorio contiene el desarrollo del **Taller Práctico de Pandas y Operaciones Matemáticas**. El objetivo principal es la aplicación de conceptos fundamentales de análisis de datos, manipulación de DataFrames, operaciones estadísticas, control impositivo y filtrado avanzado mediante el uso de la librería **Pandas** y **NumPy** en Python.

El análisis se lleva a cabo sobre un Dataset expandido que incluye el listado de productos tecnológicos y de oficina, precios base, stock de inventario, costos de envío y categorías, importado directamente de forma remota.

---

## 👥 Integrantes del Equipo
* *Dairon Valencia Campaz*
* *Nombre del Integrante 2*
* *Nombre del Integrante 3*
* *Nombre del Integrante 4*

*(Equipo conformado bajo los criterios de asistencia del 25 de mayo de 2026)*

---

## 💻 Datos e Importación
El dataset original fue extendido con los 54 productos tecnológicos requeridos. En el Notebook, la información se consume en tiempo real directamente desde el repositorio oficial mediante la URL del archivo Excel:
* **Archivo Fuente:** `productos tecnologicos IA_panda.xlsx`

---

## 📊 Estructura del Notebook y Puntos Resueltos

El proyecto está estructurado de manera lineal siguiendo estrictamente el taller asignado:

### 1. Creación y Exploración del DataFrame
* Importación de librerías esenciales (`pandas` y `numpy`).
* Carga del archivo Excel remoto mediante `pd.read_excel()`.
* Exploración preliminar de la estructura de datos:
  * Visualización de las primeras 5 filas (`.head()`) y las últimas 10 filas (`.tail(10)`).
  * Identificación de los tipos de datos de las columnas (`.dtypes`).
  * Dimensión total del DataFrame (`.shape`), mostrando el volumen total de registros.
  * Resumen estadístico intrínseco de las variables numéricas (`.describe()`).

### 2. Operaciones Matemáticas entre Columnas
* **`Total_Venta`**: Columna calculada multiplicando el precio unitario por la cantidad estipulada de productos (`Precio` × `Cantidad`).
* **`Costo_Total`**: Columna que consolida la venta más los recargos logísticos (`Total_Venta` + `Costo_Envio`).
* Cálculo del promedio general de ingresos monetarios (`.mean()`).
* Identificación exacta de los productos con el rendimiento comercial más alto (`idxmax()`) y más bajo (`idxmin()`).

### 3. Porcentaje y Análisis
* **IVA (19%)**: Deducción impositiva aplicada individualmente sobre el `Total_Venta`.
* **Ganancia Estimada (25%)**: Margen proyectado de utilidad sobre la venta.
* **Pérdida Estimada (0.05%)**: Cálculo de riesgo financiero operativo por producto.
* **Porcentaje de Ventas**: Peso porcentual representativo de cada producto frente al valor del total general acumulado (`sum()`).
* *Análisis de umbral:* Filtrado de productos con participación superior al 15%. *(Nota del análisis: El DataFrame expandido distribuye las ventas de forma homogénea, por lo cual ningún producto individual supera el 15% de la regla)*.

### 4. Estadística Descriptiva
* Análisis de tendencia central para la columna `Precio`: Cálculo de la **Media**, **Mediana** y **Moda** (extrayendo el valor más frecuente mediante `.mode()[0]`).
* Medida de dispersión: **Desviación Estándar** para evaluar la variabilidad en el stock de la columna `Cantidad`.
* Extracción de los valores analíticos absolutos máximos y mínimos de la columna `Total_Venta`.

### 5. Filtrado y Exportación
* Segmentación aislada de los artículos de la categoría **"Tecnología"**.
* Agrupación y ordenamiento descendente de las ventas totales de los productos empleando `.groupby()` junto con `.sort_values(ascending=False)`.
* **Punto Adicional:** Exportación automatizada del DataFrame final con todas las métricas calculadas hacia un archivo físico local llamado `resultado_final.xlsx`.

---

## 🛠️ Tecnologías Utilizadas
* **Python 3.x**
* **Pandas** (Manipulación y análisis de estructuras de datos)
* **NumPy** (Soporte matemático)
* **OpenPyXL** (Motor de escritura para archivos Excel)
* **Jupyter Notebook / Google Colab**

---
*Fecha límite de entrega: Viernes 29 de mayo de 2026 - 10:00 pm***
