# Análisis en los Hábitos de Compra en los Usuarios de Instacart

Proyecto de análisis exploratorio y de comportamiento enfocado en **comprender los hábitos de compra de los usuarios** de la plataforma de comestibles **Instacart**. El análisis estudia patrones de pedidos, productos y reordenes, así como el comportamiento temporal de los clientes, con la finalidad de responder a múltiples preguntas de negocio para su posterior uso en estrategias comerciales y de marketing.

<p align="center">
    <img src="figures/instacart_delivery.png" width="500">
    <br>
    <em>Repartidor de Instacart.</em>
</p>

## Contexto del problema

Las plataformas de e‑commerce de comestibles dependen fuertemente de la frecuencia de compra y la lealtad del cliente. Comprender **cómo, cuándo y qué compran los usuarios** es clave para, por ejemplo:

- Optimizar la experiencia de compra.
- Diseñar estrategias de retención.
- Mejorar sistemas de recomendación.
- Incrementar el valor de vida del cliente.

Instacart, como marketplace de alto volumen, genera grandes cantidades de datos transaccionales que permiten analizar estos comportamientos con detalle.

## Objetivo del análisis

Se presentan múltiples preguntas y respuestas respaldadas con datos alrededor de los siguientes temas:

- Frecuencia y recurrencia de pedidos de los clientes.
- Identificación de los productos más comprados y más reordenados.
- Estudio de patrones temporales de compra por día de la semana y hora del día.
- Evaluación de hábitos de recompra y lealtad a productos.

## Datasets

El proyecto utiliza múltiples datasets relacionados con la operación de Instacart, entre ellos:

- **orders**: información de pedidos como usuario, día de la semana, hora y orden relativa.
- **order_products**: relación entre pedidos y productos comprados.
- **products**: catálogo de productos.
- **aisles** y **departments**: categorización de productos.

## Metodología aplicada

1. Preparación y limpieza de datos.
2. Análisis exploratorio.
3. Análisis de productos:
   - Productos más comprados.
   - Productos con mayor tasa de reorden.
   - Análisis por departamento y pasillo.
4. Análisis de recompra:
   - Cálculo de tasas de reorden por producto y por cliente.
   - Segmentación de usuarios según comportamiento de recompra.
   - Identificación de patrones de lealtad.

## Resultados clave y recomendaciones de negocio

- Las **horas pico para realizar pedidos se concentran entre las 9 a.m. y 5 p.m.**, mientras que los días con **más demanda son los domingos y lunes**, lo que podría se usado para lanzar publicidad u ofertas que **aumenten el ticket de compra**.
- Gran proporción de los usuarios **repiten sus compras cada 1, 7 o 30 días**, indicando que los clientes suelen hacer compras diarias, semanales o mensuales, con lo que se podrían elaborar **paquetes especiales** para aquellos usuarios que siguen este patrón seguro de compra. 
- Los productos más vendidos y frecuentemente reordenados son principalmente **frutas y verduras**, con los plátanos liderando de manera significativa. Estos productos podrían **probarse su ofrecimiento en combo** con algunos otros productos relacionados para aumentar los ingresos aprovechando la alta demanda que tienen. 
- La tasa de repetición de los clientes muestra que un **62% tiene una fidelidad moderada o alta a los productos que han comprado anteriormente**. Por lo que hay aún área de oportunidad para mejorar la tasa analizando los intereses del gripo fuera de esta proporción

## Cómo ejecutar el proyecto

1. Crear un entorno virtual:
   ```bash
   python -m venv .venv
   ```

2. Activar el entorno:
   - Windows:
     ```bash
     .\.venv\Scripts\activate
     ```
   - macOS / Linux:
     ```bash
     source .venv/bin/activate
     ```

3. Instalar dependencias:
   ```bash
   pip install -r requirements.txt
   ```

4. Ejecutar el notebook:
   - Abrir el archivo dentro de la carpeta `notebooks`
   - Seleccionar el kernel del entorno virtual
   - Ejecutar todas las celdas en orden

---

## Tecnologías usadas

- Python.
- Pandas.
- NumPy.
- Matplotlib y Seaborn.
- Jupyter Notebook
