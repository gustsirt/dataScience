
# Proyecto de Data Science: Análisis de Ventas Online

`Dataset: Datos.csv`

Este proyecto de data science se enfoca en el análisis de una base de datos alterada de una empresa comercial que realiza ventas online. La base de datos, cuidadosamente falsificada, no guarda relación con la realidad ni toma en cuenta efemérides, lo que permite analizar las ventas en un contexto controlado y simulado, proporcionando información valiosa para realizar inferencias sin comprometer la integridad de datos reales.

## Objetivo de análisis:

El objetivo principal del proyecto es analizar la composición y distribución de las ventas contenidas en el dataset, generando gráficos y análisis numéricos para responder preguntas de interés y validar o refutar hipótesis comerciales. Este análisis permitirá generar un informe detallado para el área comercial de la empresa.

El análisis se enfoca en las siguientes hipótesis iniciales:

1. **Distribución geográfica**: Dado que la sede principal de la empresa se encuentra en Córdoba, se espera que al menos el 70% de las ventas provengan de esta localidad.
2. **Concentración de ventas en tiendas**: El 60% de las operaciones deberían estar concentradas en tres de las tiendas principales (Tiendas 1, 2 y 3).
3. **Comportamiento temporal de las ventas**: Se asume que la mayoría de las ventas ocurren durante los fines de semana.
4. **Patrones horarios**: Se estima que una cantidad considerable de ventas se realizan en horarios de siesta.

### Gráficos y análisis de variables:

Para dar respuesta a estas hipótesis, se crearán gráficos que incluyan al menos tres variables clave, como **ubicación geográfica**, **horario de la transacción**, y **categoría del producto**. Estos gráficos permitirán realizar un diagnóstico visual de cómo se comportan las ventas en función de las preguntas de interés. Además, el análisis numérico complementará los gráficos, brindando información cuantitativa precisa sobre las tendencias observadas.

### Identificación de valores perdidos:

Durante el proceso de análisis, se identificarán los valores perdidos en el dataset, lo que permitirá evaluar su impacto en los resultados. Se implementarán técnicas para gestionar estos valores, garantizando que no afecten de forma significativa las conclusiones del análisis.

## Diccionario de datos:

Para facilitar la comprensión y análisis del dataset, se incluye un diccionario de datos que detalla los campos más relevantes. Este diccionario abarca variables como el **origen del pedido** (marketplace o fulfillment), el **documento del cliente**, la **ciudad** y **estado** desde donde se realizó el pedido, el **tipo de dirección de entrega**, así como detalles sobre las **promociones aplicadas**, el **código de referencia del SKU**, el **precio de venta del SKU**, entre otros.


## Diccionario

* **Origin**:  indica si el origen del pedido es marketplace o fulfillment.
* **Sequence**: es la secuencia numérica de la transacción del pedido.
* **Creation Date**:  es la fecha y hora en que el cliente realizó el pedido.
* **Client Document**:  es el número de identificación fiscal del cliente que realizó el pedido.
* **UF**:  es el estado, provincia, región o departamento desde el que el cliente realizó el pedido.
* **City**:  es la ciudad desde la que el cliente realizó el pedido.
* **Address Type**:  es el tipo de dirección de entrega (domicilio o recogida).
* **Postal Code**:  es el código postal de la dirección de entrega.
* **Courier**:  es la transportadora responsable de la entrega.
* **Status**:  es el status del pedido en el momento de exportación la plantilla.
* **Coupon**:  es el ID del cupón del pedido, si lo hay.
* **Quantity_SKU**:  es la cantidad de ítems del mismo SKU.
* **Category Ids Sku**:  son los ID de las categorías en los que se encuentra el SKU. Esta información se presenta siguiendo el árbol de departamento/categoría/subcategoría. Por ejemplo, si el valor es /1000003/1000016/, eso significa que el SKU está en la categoría 1000016, que a su vez forma parte del departamento 1000003.
* **Reference Code**:  es el código de referencia del SKU.
* **SKU Selling Price**:  es el precio al que se vendió el SKU realmente, ya con los descuentos o promociones aplicados.
* **SKU Total Price**:  es el valor total del SKU en el pedido, considerando todos os ítems del SKU.
* **Total Value**:  es el valor total del pedido. Atención porque este es el valor cobrado por la operación y no toma en cuenta que una operación puede tener as de una linea
* **Discounts Names**:  son las promociones aplicadas al pedido.
* **Canceled By**:  es el email del usuario que realizó la cancelación del pedido.
* **Corporate Document**:  es el número de registro de persona jurídica, cuando el pedido es realizado por una empresa.
* **SalesChannel**:  es el ID de la política comercial del pedido. (Identifica la tienda)