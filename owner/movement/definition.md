# Movimiento

## Definición

Un movimiento representa un hecho ocurrido dentro de una organización. Permite registrar entradas y salidas relacionadas con dinero o artículos sin exigir al usuario conocimientos contables.

## Tipo y evento

Un movimiento utiliza dos dimensiones principales.

El tipo indica qué se mueve:

- `entity`: relación económica con una entidad.
- `item`: entrada o salida de un artículo.

El evento indica la dirección:

- `income`: entrada.
- `outcome`: salida.

Una venta puede generar un ingreso asociado a una entidad y una salida de artículos. Una compra puede generar un egreso asociado a una entidad y una entrada de artículos.

## Entidades

Una entidad representa una persona, empresa o grupo con el que una organización registra movimientos.

Las entidades son transversales y no pertenecen exclusivamente a una organización. Su tipo depende de los tipos de sujeto configurados para el país.

Cuando corresponde, una entidad puede utilizar un identificador. Senttinela aplica las reglas conocidas para ese identificador sin exigir al usuario conocer su implementación técnica.

## Artículos

Un artículo representa algo que puede participar en un movimiento.

Actualmente se distinguen tipos como producto y servicio. Un producto utiliza una unidad de medida; un servicio no requiere una unidad física.

Los artículos forman un catálogo transversal para reducir registros repetidos y facilitar su reutilización entre organizaciones.

## Estado y pagos

Los movimientos de entidad pueden registrar su estado de pago y los pagos efectivamente realizados. Los pagos permiten representar el flujo efectivo de ingresos y egresos de la organización.

## Evolución

Movement concentra actualmente el registro de movimientos, entidades y artículos. Estos conceptos pueden evolucionar hacia contextos independientes cuando exista una necesidad real del producto.
