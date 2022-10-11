

# Datathon

## Descripción del problema

Somos parte de una empresa de logística que trabaja para un portal importante de E-Commerce, y nuestro Team Leader nos da la tarea de implementar un modelo que nos permita predecir si un envío llegará a tiempo o no, según la información contenida en el dataset puesto a disposición para poder prestar atención y mejor seguimiento a aquellos envíos que pueden llegar a dar problemas.

## Métrica a utilizar

Como método de evaluación del desempeño del modelo, se utilizará Exhaustividad (Recall) de la matriz de confusión (Confusion Matrix)

$$ Recall=\frac{TP}{TP+FN}$$

siendo $TP$ los verdaderos positivos, $TN$ verdaderos negativos y $FN$ los falsos negativos.

## Archivos provistos

Se proveen los archivos:
- 'E-Commerce_train.xlsx', con 8998 observaciones y 12 dimensiones, incluyendo información sobre si el envío llegó a tiempo o no en el momento del registro. 
- 'E-Commerce_test.xlsx', con 2000 observaciones y 11 dimensiones, sin incluir información sobre si el envío llegó a tiempo o no en el momento del registro.

## Descripción de las dimensiones

- ID: identificador del registro de orden (valor entero).
- Warehouse_block: Almacén de distribución de donde salió la orden (A a F).
- Mode_of_Shipment: Medio de transporte (Flight, Road, Ship).
- Customer_care_calls: Número de llamadas a atención al cliente que hubo por esa orden. (valores enteros del 2 al 7)
- Customer_rating: Puntaje del cliente (valores enteros 1 al 5).
- Cost_of_the_Product: Costo del producto (valor numérico entero de 96 a 310).
- Prior_purchases: Número de compras previas realizadas por el cliente (valor numérico entero de 2 a 10).
- Product_importance: Nivel de importancia del producto (low, medium, high).
- Gender: Género del comprador (F, M).
- Discount_offered: Porcentaje de descuento ofrecido por esa compra (valor numérico entero de 1 a 65):
- Weight_in_gms: Peso del paquete de la orden, en gramos (valor numérico entero de 1001 a 7846).
- Reached.on.Time_Y.N: Información sobre la llegada del paquete a destino (1 si llegó a tiempo, 0 si no llegó a tiempo).



