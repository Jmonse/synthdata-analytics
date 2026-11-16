# 📊 Análisis de Ventas y Marketing — SynthData 2024

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![pandas](https://img.shields.io/badge/pandas-3.0-lightgrey?logo=pandas)
![Plotly](https://img.shields.io/badge/Plotly-6.6-brightgreen?logo=plotly)
![Status](https://img.shields.io/badge/Estado-Completo-success)

**Autor:** Jonathan Monserrat ([@Jmonse](https://github.com/Jmonse))  
**Stack:** Python · pandas · NumPy · Matplotlib · Seaborn · Plotly · Power BI Desktop  
**Datos:** 3 datasets sintéticos · 3.035 transacciones · 90 campañas · 567 clientes

---

## 📌 Descripción

Análisis exploratorio y estadístico end-to-end de ventas, campañas de marketing y perfiles demográficos de clientes de una empresa de retail simulada en Argentina (2024).

```text
Carga → Diagnóstico de calidad → Limpieza documentada → EDA
→ Estadística descriptiva → Correlación → Visualización
→ Atribución temporal de campañas → Conclusiones accionables

```

---

## 🗂️ Estructura del Proyecto

```text
synthdata-analytics/
├── dashboard/
│   └── SynthData_Dashboard.pbix       # Dashboard ejecutivo interactivo (Power BI)
├── data/
│   ├── ventas.csv                     # 3.035 transacciones de ventas (2024)
│   ├── marketing.csv                  # 90 campañas en canales TV, RRSS y Email
│   └── clientes.csv                   # 567 perfiles de clientes
├── docs/
│   └── img/                           # Visualizaciones estáticas exportadas (.png)
├── notebooks/
│   └── 01_SynthData_Analytics.ipynb   # Notebook principal con el análisis completo
├── outputs/
│   └── dashboard_interactivo.html     # Dashboard interactivo exportado (Plotly)
├── .gitignore
├── README.md
└── requirements.txt

```

---

## 📈 Principales Hallazgos

| Métrica | Valor |
| --- | --- |
| **Ingreso total anual** | $1.467.094 |
| **Total de transacciones válidas** | 2.998 (tras depurar 35 duplicados y 2 nulos) |
| **Ticket promedio** | $489,36 |
| **Categoría líder** | Electrodomésticos (34,4%) |
| **Producto con mayor ingreso** | Lámpara de mesa |
| **Mes pico de ventas** | Mayo ($143.727) |

* **Distribución equilibrada por categoría:** Electrodomésticos (34,4%), Electrónica (32,9%) y Decoración (32,7%) mantienen participaciones homogéneas, reduciendo el riesgo de concentración.
* **Sin correlación precio-cantidad ($r = -0,002$):** El precio unitario no penaliza el volumen comprado por transacción.
* **Estacionalidad semestral:** El primer semestre concentra los picos de facturación, con desaceleración sostenida entre junio y octubre.
* **Perfil demográfico:** El segmento de 46 a 60 años registra el mayor ingreso promedio declarado (~$36.500).
* **Atribución de campañas de marketing:** Se atribuyeron $381.469 en ingresos dentro de ventanas activas (prorrateando campañas simultáneas); **Email** lidera el retorno bruto (ROAS 968,3x), aunque los bajos costos registrados exigen incorporar CAC y conversión para decidir presupuesto.
* **Visualización multi-herramienta:** Además del dashboard interactivo en Plotly (`outputs/dashboard_interactivo.html`), el proyecto incluye un tablero ejecutivo en Power BI Desktop (`dashboard/SynthData_Dashboard.pbix`).

---

## 🚀 Cómo Ejecutar el Proyecto

```bash
# 1. Clonar el repositorio
git clone https://github.com/Jmonse/synthdata-analytics.git
cd synthdata-analytics

# 2. Crear y activar entorno virtual
python -m venv .venv
source .venv/Scripts/activate   # Windows (Git Bash)
source .venv/bin/activate       # Linux / macOS

# 3. Instalar dependencias
pip install -r requirements.txt

# 4. Ejecutar el notebook
jupyter notebook notebooks/01_SynthData_Analytics.ipynb

```
