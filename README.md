# 🧪 A/B Test – Optimización de Conversiones en una App Fintech
**Portafolio Data Analyst | 2025**  
Evaluación del impacto de un nuevo flujo de registro sobre las tasas de conversión

---

## 🎯 1. Objetivo del proyecto
Realizar un experimento A/B para determinar si un **nuevo flujo de registro** en una app de préstamos mejora:

- CTR (Click-Through Rate)  
- View Content Rate  
- Search Rate  
- Add to Cart Rate  
- Purchase Rate  

El objetivo es comparar el **grupo Control** vs. **grupo Test** para identificar si el nuevo flujo incrementa conversiones y en qué etapas del embudo impacta.

---

## 📁 2. Dataset
El experimento se realizó con dos archivos:

- 🅰️ **control_group.csv** — Usuarios expuestos al flujo original  
- 🅱️ **test_group.csv** — Usuarios expuestos al nuevo flujo

Cada archivo contiene:

- ID de usuario  
- Etapa alcanzada (impressions, clicks, search, view content, add to cart, purchase)  
- Fechas  
- Resultados por etapa

---

## 🛠️ 3. Herramientas utilizadas
- 🐍 Python (Pandas, NumPy, SciPy)  
- 📈 Estadística: proporciones, diferencias de medias, tests z  
- 📊 Power BI (visualización del embudo y métricas)  
- 📓 Jupyter Notebook  
- 🗂️ GitHub  

---

## 🔎 4. Proceso analítico

### 🧹 4.1 Preparación
- Integración de ambos datasets  
- Limpieza y estandarización de columnas  
- Cálculo de tasas por etapa del embudo  
- Identificación de outliers y valores anómalos  

### 📈 4.2 Métricas calculadas
Para ambos grupos se midieron:

- **CTR**  
- **View Content Rate**  
- **Search Rate**  
- **Add to Cart Rate**  
- **Purchase Rate**  
- **Diferencias absolutas y relativas**

### 🧪 4.3 Pruebas estadísticas
- Test de proporciones (z-test)  
- Evaluación de significancia estadística (α = 0.05)  
- Comparación de intervalos de confianza  
- Validación del tamaño de muestra  

### 📊 4.4 Dashboard en Power BI
Incluye visualizaciones de:

- CTR Control vs Test  
- Embudo de conversión completo  
- Variación por etapa  
- Purchase Rate por día  
- Grupo ganador  

---

## 📌 5. Principales hallazgos

Los valores del dashboard muestran:  
- 🔼 **CTR mejoró significativamente: 4.86% → 8.09%** (📈 +3.23 pp)  
- 🔽 **View Content Rate disminuyó** (-10.70%)  
- 🔽 **Search Rate disminuyó** (-1.65%)  
- 🔽 **Add to Cart Rate cayó** (-19.43%)  
- 🔽 **Purchase Rate cayó** (-1.18%)  
- 🏁 **Ganador final:** *Grupo Control* (mayor Purchase Rate y estabilidad)

El nuevo flujo generó más clics, pero **empeoró la conversión en etapas medias y finales**, reduciendo la compra.

---

## 💡 6. Insights accionables

- La mejora del CTR indica que el nuevo flujo es más atractivo, pero **genera fricción** en etapas posteriores.  
- Se recomienda realizar un análisis UX de las etapas "View Content" y "Add to Cart".  
- El Test podría evaluarse nuevamente ajustando solo las etapas conflictivas.  
- El diseño actual del flujo Test **no es viable** para despliegue final debido al descenso en Purchase Rate.  
- A futuro, probar variaciones incrementales (multivariado o A/B secuencial).

---

## 📊 7. Dashboard
Disponible en el archivo:  
`Proyecto 04.pdf`  

Incluye embudo comparativo, métricas por etapa y tendencia diaria de conversión.

---

## 📂 8. Estructura del repositorio
├── 04_ab_test_fintech.ipynb
├── Proyecto_04.pdf
├── control_group.csv
├── test_group.csv
└── README.md

---

## 👤 9. Autor
**Josué Téllez**  
Data Analyst — Portafolio 2025
