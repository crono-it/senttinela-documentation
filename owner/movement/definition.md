# Movement

## Definición

Movement representa un hecho registrado dentro de una organización.

Un movimiento describe una entrada o una salida y permite registrar información sobre aquello que participa en el hecho.

El significado de la entrada o salida depende del tipo de movimiento.

## Tipos de movimiento

Movement utiliza el tipo para determinar qué representa el elemento que se mueve.

Actualmente existen dos tipos:

* `entity`: representa un movimiento económico respecto de una entidad.
* `item`: representa la entrada o salida de un artículo de la organización.

### Movimiento de entidad

Un movimiento de tipo `entity` representa un movimiento económico desde la perspectiva de la organización.

* `income` representa dinero que ingresa a la organización.
* `outcome` representa dinero que sale de la organización.

La entidad representa la contraparte respecto de la cual ocurre el movimiento.

### Movimiento de artículo

Un movimiento de tipo `item` representa el movimiento de un artículo dentro de la organización.

* `income` representa un artículo que ingresa a la organización.
* `outcome` representa un artículo que sale de la organización.

La cantidad representa cuánto del artículo participa en el movimiento.

Los movimientos de artículos constituyen la información base para obtener posteriormente las existencias de los artículos.

## Relación entre movimientos

Un mismo hecho puede generar más de un movimiento.

Por ejemplo, una compra puede generar:

* un movimiento de entidad `outcome`, porque el dinero sale de la organización respecto del proveedor;
* uno o más movimientos de artículo `income`, porque los artículos adquiridos ingresan a la organización.

Una venta puede generar:

* un movimiento de entidad `income`, porque el dinero ingresa a la organización respecto del cliente;
* uno o más movimientos de artículo `outcome`, porque los artículos vendidos salen de la organización.

Esta relación permite representar diferentes efectos de un mismo hecho sin mezclar sus significados.

## Artículos

Un movimiento puede involucrar uno o más artículos.

Cuando un artículo participa en un movimiento económico, se registra la cantidad correspondiente y, cuando corresponde, el precio unitario utilizado en ese hecho.

El valor total de un artículo se obtiene multiplicando su cantidad por su precio unitario.

El valor total del movimiento económico corresponde a la suma de los valores de sus artículos.

Un artículo puede corresponder a un producto o a un servicio.

La unidad de medida pertenece al artículo y se utiliza para interpretar su cantidad cuando corresponde.

## Registro

El registro de un movimiento debe representar el hecho ocurrido en el momento en que se registra.

La información almacenada debe permitir reconstruir posteriormente los efectos del movimiento sin depender de que la información actual de otros registros permanezca sin cambios.

El movimiento representa el hecho registrado. Las interpretaciones posteriores sobre esa información corresponden a otras capacidades de Senttinela.

## Evolución

Los movimientos constituyen una fuente de información para futuras capacidades de Senttinela.

Entre ellas pueden encontrarse:

* existencias e inventario;
* producción;
* análisis;
* resúmenes;
* visualizaciones;
* otras interpretaciones de la actividad de la organización.

Estas capacidades pueden utilizar los movimientos sin modificar el significado fundamental del registro.

## Principio

Movement debe representar lo que ocurrió desde la perspectiva de la organización.

El registro del hecho debe mantenerse separado de las interpretaciones posteriores que puedan realizarse sobre él.

Esta separación permite que nuevas capacidades utilicen los movimientos como fuente de información sin modificar el significado original de los hechos registrados.
