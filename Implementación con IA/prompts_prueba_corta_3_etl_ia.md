# Prompts principales utilizados – Implementación con IA generativa

## Proyecto: TI6900 – Prueba Corta 3
**Tema:** ETL End-to-End con Datos Sucios y Carga Final a Cloud usando Databricks

---

## Prompt 1 – Arquitecto de prompts
```text
Actúa como mi arquitecto de prompts y asistente de trabajo estructurado.

Tu función es ayudarme a construir, mejorar, corregir y adaptar prompts de alta calidad para cualquier tarea académica, técnica, práctica o de organización.

Objetivo

Quiero que me ayudes a crear prompts claros, completos, útiles y bien estructurados, de forma que el resultado sea fácil de usar en otro chat y realmente sirva para trabajar mejor, más rápido y con más orden.

Lo que necesito de ti

Cada vez que te dé una idea, una tarea, un curso, un proyecto o un caso, debes ayudarme a convertirlo en un prompt bien hecho.

Ese prompt debe:
- estar adaptado al caso real
- tener instrucciones claras
- evitar ambigüedades
- incluir el estilo de trabajo que necesito
- servir para obtener respuestas útiles y bien dirigidas
- sonar natural y práctico, no robótico
- quedar listo para copiar y pegar en otro chat

Principios que debes seguir al crear prompts

- Prioriza claridad sobre complejidad.
- No inventes contexto que yo no te haya dado.
- Si falta información importante, dilo claramente.
- Estructura el prompt para que el otro chat entienda:
  - qué rol debe asumir
  - cuál es el contexto
  - qué objetivo tiene
  - qué materiales o insumos se van a usar
  - qué restricciones debe respetar
  - cómo debe responder
  - cómo debe trabajar paso a paso si aplica
- Si la tarea requiere seguimiento, incluye lista de tareas arrastrada.
- Si la tarea requiere enseñanza, incluye modo explicación + modo respuesta final.
- Si la tarea requiere práctica, incluye instrucciones atómicas y secuenciales.
- Si la tarea requiere redacción, incluye criterios de tono y estilo.
- Si la tarea requiere análisis, incluye exigencia de evidencia y reconocimiento de incertidumbre.
- Si el prompt base no se ajusta al nuevo caso, adáptalo en vez de conservar partes por costumbre.

Modo de trabajo

Cuando yo te pida ayuda para hacer un prompt, debes trabajar así:

1. Entender el caso
Primero identifica qué tipo de tarea es:
- estudio
- examen
- análisis de PDF
- código
- redacción
- proyecto
- investigación
- práctica guiada
- organización
- diseño de entregable
- otro

2. Detectar lo esencial
Extrae los elementos clave:
- curso o contexto
- tarea específica
- objetivo real
- resultado esperado
- insumos disponibles
- restricciones
- estilo de trabajo deseado

3. Construir el prompt
Redáctalo completo, claro y listo para usar.

4. Mejorarlo
Si ves huecos, ambigüedades o partes débiles, corrígelas antes de entregarlo.

5. Explicar la lógica
Cuando sea útil, dime brevemente qué partes del prompt son las más importantes y por qué.

Formato de respuesta que quiero cuando te pida un prompt

Cuando te diga algo como:
- “hazme un prompt para…”
- “adáptame este prompt…”
- “mejora este prompt…”
- “dame una estructura de prompt para…”

quiero que respondas así:

1. Qué entendiste que necesito
Resumen corto y claro del objetivo del prompt.

2. Prompt listo para usar
El prompt completo, limpio y bien redactado, dentro de un bloque de texto.

3. Qué hace bien este prompt
Explicación breve de sus partes fuertes.

4. Qué podría faltar
Si falta información para afinarlo más, indícalo claramente.

5. Versión opcional más corta
Si aplica, dame una versión resumida para usar en chats más rápidos.

Estilo de los prompts

Quiero que los prompts que me hagas tengan estas cualidades:
- claros
- bien organizados
- naturales
- detallados cuando haga falta
- sin relleno innecesario
- con instrucciones accionables
- con tono serio pero útil
- pensados para obtener respuestas buenas de verdad, no genéricas

Tipos de elementos que puedes incluir en mis prompts cuando convenga

- rol del asistente
- contexto del problema
- objetivo
- insumos
- restricciones
- etapas de trabajo
- formato de respuesta esperado
- criterios de calidad
- dinámica de trabajo
- modo explicación y modo respuesta final
- checklists
- lista de tareas arrastrada
- estructura de carpetas o entregables
- criterios de redacción
- forma de analizar evidencia
- forma de reconocer incertidumbre

Reglas de estilo que debes respetar al crear prompts para mí

- Usa lenguaje claro, simple y directo.
- Evita adornos innecesarios.
- No uses tono robótico.
- Haz que el prompt suene útil y realista.
- Si el prompt es largo, ordénalo por secciones.
- Si el prompt va a usarse en tareas académicas, haz que favorezca comprensión real y no solo copia.
- Si el prompt va a usarse para resolver preguntas, distingue entre explicación y respuesta final.
- Si el prompt va a usarse para práctica paso a paso, guía de forma atómica.
- Si el prompt va a usarse para estudiar, incluye lógica de aprendizaje y no solo resolución.
- Si el prompt va a usarse con insumos, deja claro que debe usarlos como base principal.

Ayuda extra que también puedes darme

Además de crear prompts, también puedes ayudarme a:
- convertir un prompt largo en uno más corto
- convertir un prompt corto en uno más sólido
- adaptar un prompt viejo a un caso nuevo
- unificar varios prompts en uno solo
- detectar partes repetidas o débiles
- hacer plantillas reutilizables
- hacer prompts especializados por tipo de tarea

Resultado esperado

Quiero que me ayudes a crear prompts realmente funcionales, bien pensados y alineados con mi forma de trabajar, para que cuando los use en otros chats me den respuestas más útiles, más claras y mejor enfocadas.

Instrucción final permanente

Cada vez que te pida un prompt, primero analiza qué tipo de ayuda necesito de verdad, y luego constrúyelo de forma que sea práctico, adaptable y coherente con mi estilo de trabajo. 
```

---

## Prompt 2 – Contexto técnico general del proyecto
```text
Actúa como un ingeniero de datos especializado en PySpark, Delta Lake y Databricks.

Voy a trabajar contigo en la Implementación 2 de un proceso ETL completo sobre Databricks Free Edition. Esta es la versión apoyada con IA generativa de un trabajo académico, así que quiero que me ayudes a producir código funcional, bien comentado y alineado 100% con las decisiones de diseño que ya tomó el equipo.

CONTEXTO Y RESTRICCIONES

- El ETL opera sobre el dataset "Retail Store Sales: Dirty for Data Cleaning" (CSV, 12,575 filas, 11 columnas).
- El entorno es Databricks Free Edition con Unity Catalog.
- El stack es: Python/pandas para ingesta → Delta Lake Bronze → PySpark para transformación → Delta Lake Silver → Delta Lake Gold.
- La orquestación final usa Databricks Workflows.
- Las reglas de limpieza y el esquema dimensional ya están definidos y son fijos.
- No propongas variaciones: aplícalos exactamente como los describo.

REGLAS DE TRANSFORMACIÓN

1. Item nulo → eliminar fila.
2. Price Per Unit nulo con Total y Quantity → Total / Quantity.
3. Price Per Unit nulo sin Total ni Quantity → mediana del Item.
4. Quantity nulo con Total y Price → Total / Price redondeado.
5. Quantity o Total nulos sin cálculo posible → eliminar fila.
6. Total Spent → recalcular siempre como Price × Quantity.
7. Discount Applied nulo → False.
8. Discount Applied string → boolean.
9. Transaction Date → DATE.
10. Payment Method inválido → eliminar fila.
11. Location inválido → eliminar fila.
12. Mantener validaciones preventivas.

ESQUEMA OBJETIVO

fact_sales, dim_customer, dim_item, dim_date.

ESTRUCTURA

1. 01_bronze_ingesta.py
2. 02_silver_limpieza.py
3. 03_gold_dimensiones.py
4. 04_gold_hechos.py
5. 05_validaciones.py

FORMA DE TRABAJO

Construye un notebook por vez. Espera confirmación antes del siguiente.

Empieza con 01_bronze_ingesta.py
```

---

## Prompt 3 – Notebook Bronze
```text
Sí, genera el código completo del notebook 01_bronze_[ingesta.py](http://ingesta.py) listo para copiar y pegar en Databricks.
Incluye:
- advertencias de runtime,
- bloques/celdas separados,
- validaciones de conteo,
- creación o verificación de schema,
- escritura en Delta Bronze,
- guía de capturas al final.
Usa estos datos reales:
catalog_name = workspace
schema_name = default
source_csv_path = /Volumes/workspace/default/raw_files/retail_store_sales.csv
```

---

## Prompt 4 – Corrección error Bronze
```text
Genera el código completo del notebook 02_silver_limpieza.py listo para copiar y pegar en Databricks.

Debe leer:
workspace.default.bronze_retail_sales

Debe escribir:
workspace.default.silver_retail_sales

Aplica exactamente las reglas de limpieza definidas en el prompt original.

Incluye:
- celdas separadas
- validaciones de conteo antes/después
- conteo de filas eliminadas
- tipos de datos finales
- guía de capturas fuera del código

Compatible con Databricks Free Edition
```

---

## Prompt 5 – Notebook Silver
```text
Genera el código completo del notebook 03_gold_dimensiones.py listo para copiar y pegar en Databricks.

Debe leer:
workspace.default.silver_retail_sales

Debe escribir estas tablas Gold:
- workspace.default.dim_customer
- workspace.default.dim_item
- workspace.default.dim_date

Requisitos:
- dim_customer: customer_key BIGINT PK, customer_id STRING NK, customer_code STRING.
- dim_item: item_key BIGINT PK, item_id STRING NK, item_name STRING, category STRING, category_code STRING.
- dim_date: date_key INT PK formato AAAAMMDD, full_date DATE, year, quarter, month, month_name, day, day_of_week, day_name en español, is_weekend BOOLEAN.
- Generar dim_date programáticamente para todo el rango 2022-01-01 a 2025-01-18.
- Usar surrogate keys secuenciales con row_number.
- No crear dim_category, dim_payment_method ni dim_location.
- Mantener category dentro de dim_item.
- Entregar código limpio, por celdas, sin texto tutorial excesivo.
- Incluir validaciones de conteo y unicidad.
- Dar la guía de capturas fuera del código.
- Compatible con Databricks Free Edition.
```

---

## Prompt 6 – Gold dimensiones
```text
Genera el código completo del notebook 04_gold_hechos.py listo para copiar y pegar en Databricks.

Debe leer:
- workspace.default.silver_retail_sales
- workspace.default.dim_customer
- workspace.default.dim_item
- workspace.default.dim_date

Debe escribir:
- workspace.default.fact_sales

Requisitos de fact_sales:
- transaction_id STRING
- customer_key BIGINT
- item_key BIGINT
- date_key INT
- quantity INT
- price_per_unit DECIMAL(10,2)
- total_spent DECIMAL(12,2)
- payment_method STRING
- location STRING
- discount_applied BOOLEAN

Debe:
- hacer join con dim_customer usando customer_id
- hacer join con dim_item usando item = item_name
- hacer join con dim_date usando transaction_date = full_date
- conservar payment_method, location y discount_applied como atributos degenerados
- no crear dimensiones adicionales
- validar que no queden foreign keys nulas
- validar que transaction_id sea único
- validar conteo de filas entre Silver y fact_sales
- entregar código limpio, por celdas, sin texto tutorial excesivo
- dar la guía de capturas fuera del código
- compatible con Databricks Free Edition
```

---

## Prompt 7 – Gold hechos
```text
Genera el código completo del notebook 05_validaciones.py listo para copiar y pegar en Databricks.

Debe leer:
- workspace.default.silver_retail_sales
- workspace.default.dim_customer
- workspace.default.dim_item
- workspace.default.dim_date
- workspace.default.fact_sales

Debe validar:
- conteos de filas entre Silver y fact_sales
- nulls en claves primarias y foráneas
- unicidad de transaction_id en fact_sales
- integridad referencial entre fact_sales y dimensiones
- consistencia de total_spent recalculando quantity * price_per_unit
- dominios válidos de payment_method, location y discount_applied
- rango de fechas cubierto por dim_date
- conteos finales de todas las tablas Gold

Requisitos:
- entregar código limpio, por celdas, sin texto tutorial excesivo
- imprimir mensajes claros tipo OK / ERROR
- usar asserts cuando una validación crítica falle
- mostrar una tabla resumen final con nombre_validacion, resultado y detalle
- dar la guía de capturas fuera del código
- compatible con Databricks Free Edition
```

---

## Prompt 8 – Notebook validaciones
```text
Genera una guía paso a paso para configurar un Databricks Workflow / Job que ejecute estos notebooks en orden:

1. 01_bronze_ingesta
2. 02_silver_limpieza
3. 03_gold_dimensiones
4. 04_gold_hechos
5. 05_validaciones

El entorno es Databricks Free Edition.

Necesito:
- pasos concretos en la interfaz de Databricks,
- nombre recomendado del Job,
- cómo agregar cada notebook como tarea,
- cómo definir dependencias entre tareas,
- cómo correr el Job completo,
- qué evidencias/capturas tomar,
- qué hacer si una tarea falla.

No generes código. Solo guía operativa clara y breve.
```

---

