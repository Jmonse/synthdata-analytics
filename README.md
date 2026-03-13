# 📊 Análisis de Ventas y Marketing — SynthData 2024

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![pandas](https://img.shields.io/badge/pandas-3.0-lightgrey?logo=pandas)
![Plotly](https://img.shields.io/badge/Plotly-6.6-brightgreen?logo=plotly)
![Status](https://img.shields.io/badge/Estado-Completo-success)

**Autor:** Jonathan Monserrat

**Stack:** Python · pandas · NumPy · Matplotlib · Seaborn · Plotly

**Datos:** 3 datasets · 3.035 transacciones · 90 campañas · 567 clientes

---

## 📌 Descripción

Análisis end-to-end de datos de ventas, campañas de marketing y perfiles de clientes de una empresa de retail argentina con presencia en múltiples ciudades.

El proyecto cubre el ciclo completo de data analytics:

```
Carga → Diagnóstico de calidad → Limpieza documentada → EDA
→ Estadística descriptiva → Correlación → Visualización
→ Integración de fuentes → Conclusiones accionables
```

---

## 🗂️ Estructura del proyecto

```
Proyecto-SynthData-Analytics/
│
├── SynthData_Analytics.ipynb     # Notebook principal con el análisis completo
├── dashboard_interactivo.html    # Dashboard interactivo (Plotly)
│
├── ventas.csv                    # 3.035 transacciones de ventas (2024)
├── marketing.csv                 # 90 campañas en canales TV, RRSS y Email
├── clientes.csv                  # 567 perfiles de clientes argentinos
│
├── ventas_mensuales.png          # Evolución mensual de ingresos y transacciones
├── ventas_categoria.png          # Distribución de ventas por categoría
├── top_productos.png             # Top 10 productos por ingreso
├── distribuciones.png            # Histogramas de variables clave
├── correlacion.png               # Mapa de correlación y scatter
├── seaborn_avanzado.png          # Boxplot y heatmap por mes/categoría
├── marketing_roi.png             # Performance de canales de marketing
└── demografico_clientes.png      # Perfil demográfico de clientes
```

---

## 🔍 Preguntas de negocio

1. ¿Cuáles son los productos y categorías con mayor volumen de ventas e ingresos?
2. ¿Existe estacionalidad en las ventas a lo largo del año?
3. ¿Qué canal de marketing genera mejor relación entre costo e ingresos?
4. ¿Hay correlación entre el precio de un producto y la cantidad vendida?
5. ¿Qué perfil demográfico concentra mayor poder de compra?

---

## 📈 Principales hallazgos

| Métrica                    | Valor                     |
| -------------------------- | ------------------------- |
| Ingreso total anual        | $1.467.094                |
| Total de transacciones     | 2.998                     |
| Ticket promedio            | $489                      |
| Categoría líder            | Electrodomésticos (34.4%) |
| Producto con mayor ingreso | Lámpara de mesa           |
| Mes pico de ventas         | Mayo                      |

- **Distribución equilibrada:** Las tres categorías tienen participaciones casi idénticas (34.4% / 32.9% / 32.7%), lo que reduce el riesgo de dependencia de una sola línea de productos.
- **Sin correlación precio-cantidad** (r = -0.002): El precio no determina el volumen de compra por transacción — oportunidad para estrategias de pricing sin penalización en unidades.
- **Estacionalidad marcada:** El primer semestre concentra los picos de venta. El segundo semestre cae consistentemente, especialmente de junio a octubre.
- **Segmento 46-60 años:** Mayor ingreso promedio (~$36.500) — perfil prioritario para productos premium.

---

## 🛠️ Stack tecnológico

| Librería     | Uso                                            |
| ------------ | ---------------------------------------------- |
| `pandas 3.0` | Manipulación y análisis de datos               |
| `numpy`      | Operaciones numéricas                          |
| `matplotlib` | Visualizaciones estáticas                      |
| `seaborn`    | Visualización estadística (boxplots, heatmaps) |
| `plotly`     | Dashboard interactivo                          |
| `openpyxl`   | Compatibilidad con archivos Excel              |

---

## 🚀 Cómo ejecutar el proyecto

```bash
# 1. Clonar el repositorio
git clone https://github.com/Jmonse/synthdata-analytics.git
cd synthdata-analytics

# 2. Crear entorno virtual
python -m venv .venv
.venv\Scripts\activate        # Windows CMD/PowerShell
source .venv/Scripts/activate # Windows Git Bash
source .venv/bin/activate     # Mac/Linux

# 3. Instalar dependencias
pip install pandas matplotlib seaborn plotly openpyxl nbformat

# 4. Abrir el notebook
jupyter notebook SynthData_Analytics.ipynb
# o abrirlo directamente en VSCode
```

---

## 📬 Contacto

**JM** — [@Jmonse](https://github.com/Jmonse)
