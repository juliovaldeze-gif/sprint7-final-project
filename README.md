# 📊 ConnectaTel - Análisis de Clientes y Patrones de Consumo

## 📌 Objetivo del Proyecto

El objetivo de este proyecto es analizar el comportamiento de los clientes de ConnectaTel, una empresa de telecomunicaciones en Latinoamérica, utilizando información de usuarios y consumo registrada durante 2024.

A través de técnicas de limpieza, exploración y análisis de datos, se busca identificar patrones de uso, segmentos de clientes y oportunidades de negocio que permitan optimizar la oferta de planes y mejorar la toma de decisiones.

---

## 📂 Datasets Utilizados

### users_latam.csv

Contiene información demográfica de los clientes:

* user_id
* age
* city
* plan
* signup_date

### usage.csv

Contiene los registros de uso de los servicios:

* id
* user_id
* type (call o text)
* duration
* event_date

### plans.csv

Contiene la información de los planes ofrecidos por ConnectaTel.

---

## 🔎 Etapas del Análisis

### 1. Exploración de Datos (EDA)

* Revisión de estructura de los datasets.
* Validación de tipos de datos.
* Identificación de valores nulos.
* Análisis descriptivo inicial.

### 2. Limpieza de Datos

* Corrección de valores inválidos y sentinels.
* Tratamiento de valores ausentes.
* Estandarización de nombres de ciudades.
* Conversión de fechas al formato adecuado.
* Validación de rangos de edad.

### 3. Integración de Datos

* Consolidación de la información de usuarios y consumo.
* Creación del dataset analítico `user_profile`.

### 4. Análisis de Consumo

* Cálculo de mensajes enviados por usuario.
* Cálculo de llamadas realizadas por usuario.
* Cálculo de minutos totales consumidos.
* Generación de histogramas y estadísticas descriptivas.

### 5. Detección de Outliers

* Construcción de boxplots.
* Identificación de valores atípicos mediante IQR.
* Evaluación del impacto de usuarios de alto consumo.

### 6. Segmentación de Clientes

* Segmentación por grupos de edad:

  * Joven
  * Adulto
  * Adulto Mayor

* Segmentación por nivel de uso:

  * Bajo Uso
  * Uso Medio
  * Alto Uso

### 7. Análisis Ejecutivo

* Identificación de clientes de alto valor.
* Detección de patrones de consumo.
* Generación de recomendaciones para nuevos planes y estrategias comerciales.

---

## 🚀 Cómo Ejecutar el Proyecto

### Opción 1: Google Colab

1. Descarga el archivo `.ipynb`.
2. Ingresa a Google Colab:
   https://colab.research.google.com
3. Selecciona **Archivo → Subir Notebook**.
4. Carga el notebook del proyecto.
5. Sube los archivos CSV requeridos.
6. Ejecuta las celdas en orden.

### Opción 2: Jupyter Notebook

```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook
```

Abre el notebook y ejecuta todas las celdas secuencialmente.

---

## 📋 Guía de Reproducción

1. Cargar los datasets.
2. Explorar la calidad de los datos.
3. Corregir valores nulos e inconsistencias.
4. Crear variables agregadas de consumo por usuario.
5. Generar histogramas y boxplots.
6. Identificar outliers mediante IQR.
7. Crear segmentos por edad y nivel de uso.
8. Analizar los resultados y elaborar recomendaciones de negocio.

---

## 🛠️ Tecnologías Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 🎯 Principales Hallazgos

* La mayoría de los clientes pertenece al segmento de uso medio.
* Se detectaron usuarios con consumos significativamente superiores al promedio.
* Los clientes de alto uso representan una oportunidad para planes premium y estrategias de fidelización.
* La segmentación por edad y uso permite identificar oportunidades para ofertas más personalizadas.
