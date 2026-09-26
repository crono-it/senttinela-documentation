# Movimientos

## Definición

Un movimiento representa un hecho que produce una entrada o salida para una organización.

Senttinela busca registrar estas operaciones de forma simple, sin exigir conocimientos contables a sus usuarios.

## Entidad

La entidad relacionada con un movimiento es opcional.

Cuando se conoce, permite representar a la persona, empresa o grupo relacionado con la operación. Cuando no se conoce, el movimiento puede registrarse sin crear una entidad ficticia.

Las entidades pertenecen a la organización que las registra y no se comparten con otras organizaciones.

## Artículos

Un movimiento puede contener uno o más artículos que describen aquello que originó la operación.

Los artículos pertenecen a la organización que los registra y pueden representar productos, servicios o conceptos según las capacidades disponibles.

Cuando un producto utiliza unidades de medida, el artículo define una magnitud y la unidad concreta se selecciona al registrar el movimiento. Por ejemplo, Harina puede utilizar la magnitud masa y registrarse en gramos o kilogramos.

## Cantidad y monto

Por cada artículo el usuario registra:

- cantidad;
- unidad de medida, cuando corresponda;
- monto total.

El monto total representa el valor final de esa línea, incluidos impuestos cuando corresponda. Senttinela deriva el valor unitario a partir de la cantidad y del monto total.

Senttinela no realiza actualmente una separación tributaria entre monto neto e impuestos. La gestión tributaria permanece fuera del alcance actual.

## Pagos

Un movimiento puede registrarse como pendiente o pagado.

Los movimientos pendientes pueden recibir uno o más pagos posteriormente. Cada pago conserva el monto y las fechas necesarias para representar cuándo ocurrió y cuándo fue registrado.

La suma de los pagos determina si el movimiento continúa pendiente o se considera pagado. Un pago puede superar el saldo pendiente cuando la operación real incluye intereses, cargos u otros acuerdos.

## Flujo de dinero

Los pagos representan el movimiento efectivo del dinero. Su fecha permite ubicar el ingreso o egreso en el período en que realmente ocurrió, independientemente de cuándo fue registrado en Senttinela.

## Privacidad

Los movimientos, entidades y artículos son información privada de la organización.

Senttinela aplica separación entre organizaciones y minimiza los datos personales copiados dentro de los movimientos. Estas decisiones forman parte de la evolución del producto hacia la protección de datos desde el diseño, considerando la Ley N.º 19.628 modificada por la Ley N.º 21.719.
