# ETL End-to-End con Datos Sucios y Carga Final a Cloud
### Prueba Corta 3 — TI6900 Inteligencia de Negocios

---

## Descripción del proyecto

Este proyecto implementa un proceso ETL completo sobre el dataset de Kaggle **"Retail Store Sales: Dirty for Data Cleaning"** (12.575 filas, 11 columnas), con carga final en un ambiente Cloud. El objetivo principal fue aplicar conceptos de almacenes de datos (dimensiones, hechos, medidas, esquemas dimensionales y operaciones OLAP) comparando dos enfoques de implementación: uno manual y uno asistido por IA generativa.

El resultado final es un **modelo estrella** en Delta Lake Gold con 11.362 transacciones de venta limpias, tres dimensiones (`dim_customer`, `dim_item`, `dim_date`) y una tabla de hechos (`fact_sales`), todo orquestado mediante Databricks Workflows.

---

## Stack técnico

| Fase ETL | Herramienta |
|---|---|
| Extracción / ingesta | Python (pandas) |
| Almacenamiento Bronze | Delta Lake — Unity Catalog |
| Transformación | PySpark + Notebooks |
| Orquestación | Databricks Workflows |
| Carga final Cloud | Delta Lake Silver / Gold |

**Ambiente Cloud:** Databricks Free Edition con Unity Catalog.

---

## Estructura del repositorio

```
/
├── sin_ia/          # Implementación 1: ETL sin uso de IA generativa
│   ├── notebook_1_bronze.ipynb
│   ├── notebook_2_silver.ipynb
│   └── notebook_3_gold.ipynb
│
├── con_ia/          # Implementación 2: ETL asistido con IA generativa (Claude)
│   ├── notebook_1_bronze.ipynb
│   ├── notebook_2_silver.ipynb
│   └── notebook_3_gold.ipynb
│
└── README.md
```

---

## Lo que se hizo

### 1. Perfilamiento inicial
Se identificaron **10 hallazgos de calidad de datos** en el dataset original: nulos en `Discount Applied` (33,4%), `Item` (9,6%), métricas numéricas (4,8%), tipo de dato incorrecto en fechas y booleanos, entre otros.

### 2. Reglas de transformación y limpieza
Se definieron reglas explícitas antes de programar: imputación matemática de precios, eliminación de filas irrecuperables, conversión de tipos, estandarización de dominios. La capa Silver resultó en **11.362 filas limpias**.

### 3. Implementación 1 — Sin IA generativa
ETL construido completamente con documentación oficial, manuales y foros. Tiempo total efectivo: **~2 horas** (sin contar investigación: ~8 horas).

### 4. Implementación 2 — Con IA generativa (Claude)
Mismo ETL rehecho desde cero apoyándose en IA para diseño, código, depuración y guía operativa de Databricks. Tiempo total efectivo: **~51 minutos**.

### 5. Validaciones de carga
10 validaciones automatizadas en notebook de cierre: integridad referencial, unicidad de PKs, consistencia de medidas, dominios válidos y cobertura del calendario. Todas con resultado ✅.

---

## Comparación de tiempos

| Fase | Sin IA | Con IA |
|---|---|---|
| Silver (limpieza) | 1h 02 min | 5 min |
| Investigación / docs | ~6 horas | ~20 min |
| **Total efectivo** | **1h 58 min** | **51 min** |
| **Total con investigación** | **~8 horas** | **~1h 11 min** |

---

## Integrantes

- Esteban Josué Brenes Montoya
- Joseph Marcell Lugo Brown
- Isaac David Elizondo Espinoza

**Curso:** TI6900 Inteligencia de Negocios — Instituto Tecnológico de Costa Rica  
**Profesor:** Michael Lizandro Sánchez Soto  
**Fecha de entrega:** 29/04/2026

---

## Repositorio

🔗 [https://github.com/marcell6449/BI-Prueba-Corta3](https://github.com/marcell6449/BI-Prueba-Corta3/blob/main/readme.md)
