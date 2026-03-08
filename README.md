# Python-para-Data-Science-Challenge-Alura-Store-1-
Python para Data Science: Challenge Alura Store (ejercicio 1)

# 🏪 Alura Store Latam — Análisis de Rendimiento de Tiendas

> Análisis exploratorio para apoyar la toma de decisiones estratégicas del Sr. Juan sobre qué tienda de su cadena **Alura Store** debe vender para iniciar un nuevo emprendimiento.

---

## 📌 Propósito del análisis

El Sr. Juan es dueño de una cadena de 4 tiendas llamada **Alura Store**. Necesita decidir cuál de ellas vender con el objetivo de liberar capital e invertirlo en un nuevo proyecto. Para tomar esa decisión de forma objetiva y basada en datos, este análisis evalúa el **rendimiento comparativo** de cada tienda a través de 5 métricas clave:

| # | Métrica | Descripción |
|---|---------|-------------|
| 1 | 💰 **Facturación total** | Ingresos acumulados por tienda |
| 2 | 🛒 **Ventas por categoría** | Categorías de productos más populares |
| 3 | ⭐ **Calificación promedio** | Nivel de satisfacción del cliente (escala 1–5) |
| 4 | 📦 **Productos más y menos vendidos** | Identificación de productos estrella y rezagados |
| 5 | 🚚 **Costo promedio de envío** | Eficiencia logística de cada tienda |

Al final del análisis se genera una **recomendación formal** dirigida al Sr. Juan.

---

## 🗂️ Estructura del proyecto

```
AluraStoreLatam/
│
├── 📓 AluraStoreLatam_vf.ipynb   # Notebook principal con todo el análisis
├── 📄 README.md                        # Este archivo
│
└── 📊 datos/                           # Fuentes de datos (acceso remoto vía URL)
    ├── tienda_1.csv                    # Datos históricos — Tienda 1
    ├── tienda_2.csv                    # Datos históricos — Tienda 2
    ├── tienda_3.csv                    # Datos históricos — Tienda 3
    └── tienda_4.csv                    # Datos históricos — Tienda 4
```

> 📡 Los archivos CSV se cargan directamente desde el repositorio oficial de Alura en GitHub, por lo que **no es necesario descargarlos manualmente**.

### Organización del notebook

El notebook está dividido en **7 secciones** ordenadas lógicamente:

```
0. Importación de librerías y datos
1. Análisis de facturación
2. Ventas por categoría
3. Calificación promedio de las tiendas
4. Productos más y menos vendidos por cada tienda
5. Costo promedio de envío por cada tienda
6. Dashboard comparativo
7. Recomendación final (conclusión)
```

---


---

## 🚀 Instrucciones para ejecutar el notebook

### Opción A — Google Colab (recomendado, sin instalación)

1. Abre [Google Colab](https://colab.research.google.com/)
2. Ve a **Archivo → Subir notebook**
3. Carga el archivo `AluraStoreLatam_vf.ipynb`
4. Haz clic en **Entorno de ejecución → Ejecutar todo** (`Ctrl + F9`)
5. ¡Listo! Los datos se descargan automáticamente desde GitHub

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

---

### Opción B — Ejecución local con Jupyter

**Requisitos previos:**

```bash
Python >= 3.8
```

**Instalación de dependencias:**

```bash
pip install pandas matplotlib numpy jupyter
```

**Ejecución:**

```bash
# Clona o descarga el proyecto
git clone https://github.com/tu-usuario/alura-store-latam.git
cd alura-store-latam

# Inicia Jupyter Notebook
jupyter notebook AluraStoreLatam_Analisis.ipynb
```

---

## 🔍 Fuentes de datos

Los datos provienen del repositorio oficial del Challenge de Alura Latam:

```
https://github.com/alura-es-cursos/challenge1-data-science-latam
```

Cada archivo CSV contiene las siguientes columnas:

| Columna | Tipo | Descripción |
|---------|------|-------------|
| `Producto` | string | Nombre del producto vendido |
| `Categoría del Producto` | string | Categoría (Electrónicos, Muebles, etc.) |
| `Precio` | float | Precio de venta en COP |
| `Costo de envío` | float | Costo de despacho en COP |
| `Fecha de Compra` | string | Fecha de la transacción (DD/MM/AAAA) |
| `Vendedor` | string | Nombre del vendedor |
| `Lugar de Compra` | string | Ciudad de la transacción |
| `Calificación` | int | Puntuación del cliente (1–5) |
| `Método de pago` | string | Forma de pago utilizada |
| `Cantidad de cuotas` | int | Número de cuotas del pago |
| `lat` / `lon` | float | Coordenadas geográficas del lugar de compra |

---

## 🎯 Conclusión del análisis

Después de evaluar las 4 tiendas con criterios objetivos y ponderados:

> **✅ Recomendación:** El Sr. Juan debería vender la tienda con el puntaje más bajo, ya que concentra los peores indicadores en facturación, satisfacción del cliente y eficiencia de envío. Liberar este activo le permitirá capitalizar su inversión y redirigirla hacia un nuevo emprendimiento con mayor potencial de crecimiento.

---

## 👤 Autor

Proyecto desarrollado como parte del **Challenge 1 de Data Science — Alura Latam**.

---

*📅 Última actualización: 2026*
