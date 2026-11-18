# Calculadora de distribución de frecuencias

Para usarla, abre `index.html` en el navegador (necesita internet la primera vez para cargar las librerías de gráficos y de Excel).

## Archivos

- `index.html`: estructura de la página (12 secciones).
- `estilos.css`: diseño visual (también el formato para imprimir / guardar en PDF).
- `estadistica.js`: **todos los cálculos**, separados de lo visual. Siguen las fórmulas del Excel de clase.
- `app.js`: lee los datos y muestra las tablas, las explicaciones y los gráficos, y genera la descarga de Excel.
- `datos_ejemplo.csv`: 100 datos de unidades vendidas (los mismos del Excel).

## Qué calcula

1. Pasos de la tabla: Sturges `k = REDONDEAR.MAS(1 + 3,322·log10(n))`, longitud `L = REDONDEAR.MAS((máx − mín)/k)` con los decimales de los datos, intervalos `mayor = menor + L − unidad`.
2. Tabla: Ci, menor, mayor, fi, Fi, hi, Hi, %, Mi, fi·Mi.
3. Tendencia central: media, media agrupada, mediana, moda (amodal / unimodal / multimodal), moda de Czuber, media geométrica, media armónica.
4. Posición: P10, Q1, mediana, Q3, P90 (PERCENTIL.INC) y una calculadora para cualquier percentil.
5. Dispersión: rango, varianza y desviación (poblacional y muestral), coeficiente de variación, RIC, desviación media, error típico.
6. Forma: asimetría (COEFICIENTE.ASIMETRIA), asimetría de Pearson, curtosis (CURTOSIS).
7. Gráficos con los mismos colores en todos: histograma, pastel, polígono, ojiva y diagrama de caja.
8. Regresión: lineal, exponencial, logarítmica, potencial y polinómica, con R², R² ajustado y r de Pearson.
9. Calculadoras de promedio ponderado, media geométrica y media armónica (con los ejemplos de clase).

Cada resultado muestra la fórmula, los números reemplazados y una explicación en palabras sencillas.
