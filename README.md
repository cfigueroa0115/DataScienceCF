# DataScienceCF

# 📘 README - Análisis de rendimiento de tiendas para Toma de decisiones estratégicas

# 🧠 Descripción General
* Este proyecto tiene como objetivo apoyar al Señor Juan, propietario de cuatro tiendas en Colombia, a decidir cuál tienda cerrar para reinvertir en un nuevo negocio. A través de técnicas de análisis de datos con Python y visualizaciones gráficas, se evalúa el desempeño de cada tienda bajo cinco criterios clave.

# 🧾 Fuentes de Datos
Se utilizaron archivos CSV públicos correspondientes a cada tienda, provenientes del repositorio de Alura Latam:
url1 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/main/base-de-datos-challenge1-latam/tienda_1%20.csv"
url2 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/main/base-de-datos-challenge1-latam/tienda_2.csv"
url3 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/main/base-de-datos-challenge1-latam/tienda_3.csv"
url4 = "https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/main/base-de-datos-challenge1-latam/tienda_4.csv"

* Los archivos contienen variables como:
Producto, Categoría del Producto, Precio, Costo de envío, Fecha de compra, Vendedor, Lugar de compra, Calificación, Método de pago, Cantidad de cuotas, lat, lon.

# 🔎 Proceso de Análisis
 * Importación y preparación de datos
Se importaron los CSV utilizando pandas y se almacenaron en variables por tienda. Se realizó la inspección inicial con .head().

# Análisis de Facturación
Se calculó la suma total de ingresos por tienda utilizando la columna Precio.

# 📌 Resultados:
# Tienda   | Ingreso Total
 Tienda 1  | 1,150,880,000
 Tienda 2  | 1,116,344,000
 Tienda 3  | 1,090,020,000
 Tienda 4  | 1,038,376,000

🔻 Tienda con menor facturación: Tienda 4

# Ventas por Categoría
Se evaluaron las categorías más populares usando .value_counts() por tienda.

📌 Resultado: La categoría predominante en todas las tiendas es Muebles, destacando especialmente en Tienda 3.

# Calificación Promedio por Tienda
Se calculó el promedio de calificación por tienda usando la columna Calificación.

# 📌 Resultados:
# Tienda  | Calificación Promedio
 Tienda 1 | 3.98
 Tienda 2 | 4.04
 Tienda 3 | 4.05
 Tienda 4 | 4.00

# Productos más y menos vendidos
Se utilizaron .value_counts() y .idxmax() / .idxmin() para extraer los top y bottom 5 productos por tienda.

# 📌 Ejemplos:

# Tienda 1
 * Más vendido: Microondas – 60 ventas
 * Menos vendido: Auriculares con micrófono – 33 ventas

# Tienda 4
 * Más vendido: Cama box – 61 ventas
 * Menos vendido: Carrito de control remoto – 53 ventas

# 📉 Tienda 4 presenta menor diferenciación en rotación de productos.


# Costo Promedio de Envío
Se usó .mean() sobre la columna Costo de envío para cada tienda.

# 📌 Resultados:
#  Tienda | Costo Promedio
 Tienda 1 | $26,818.61
 Tienda 2 | $24,512.24
 Tienda 3 | $24,885.68
 Tienda 4 | $23,459.46

Aunque Tienda 4 tiene menor costo de envío, esto no compensa su bajo ingreso y rendimiento general.

# Distribución Geográfica
Se integraron latitud y longitud para visualizar:
 * Mapa de dispersión geográfica por tienda
 * Mapa de calor de concentración de ventas

📍 Esto permite evidenciar zonas de mayor impacto comercial, siendo Medellín y Bogotá las más activas.

# 📌 Conclusión
# ✅ Recomendación Estratégica:

Cerrar Tienda 4, ya que presenta:
 * Menor facturación total.
 * Menor calificación media en comparación con líderes.
 * Menor dinamismo en rotación de productos.
 * Aunque su envío es más barato, no se traduce en mayor volumen de ventas.
 * Baja competitividad frente a otras tiendas.

# 🛠 Herramientas Utilizadas
 * Lenguaje: Python
 * Librerías: pandas, matplotlib, seaborn
 * Visualización: Gráficos de barras, pastel, dispersión y mapa de calor
 * Plataforma: Google Colab

# 👨‍💼 Autor
 * Nombre: Carlos Alberto Figueroa Martinez
 * Fecha de análisis: 16/04/2025
 * Proyecto: Challenge Data Science - Alura Latam


