# Movimiento de entidad

## Definición

El movimiento de entidad representa el registro de un movimiento económico de una organización respecto de una entidad.

El movimiento pertenece a la organización y la entidad representa la contraparte respecto de la cual ocurre.

## Perspectiva

El movimiento se interpreta siempre desde la perspectiva de la organización.

Un ingreso representa dinero que la organización recibe respecto de una entidad.

Un egreso representa dinero que la organización entrega respecto de una entidad.

Esta perspectiva permite mantener una interpretación consistente del movimiento independientemente de la naturaleza de la operación que lo originó.

## Artículos

Un movimiento puede involucrar uno o más artículos.

Los artículos forman parte de la información que describe el hecho económico, pero no determinan por sí mismos la naturaleza del movimiento.

Un mismo artículo puede participar tanto en un ingreso como en un egreso.

## Separación entre hecho e interpretación

El movimiento de entidad se ocupa de representar el hecho económico registrado.

La interpretación posterior de ese hecho pertenece a otras capacidades del sistema y no forma parte de la responsabilidad inicial del módulo.

Esta separación permite que el movimiento conserve una representación independiente de las interpretaciones que puedan realizarse posteriormente sobre la información registrada.

## Registro auxiliar de entidades y artículos

El módulo puede permitir el registro de entidades y artículos durante el flujo de trabajo de un movimiento.

Esta capacidad existe para evitar que la organización deba abandonar el contexto actual cuando la entidad o el artículo que necesita todavía no se encuentra registrado.

El registro realizado desde movimiento de entidad no implica que las entidades o artículos pertenezcan conceptualmente al módulo. Estos mantienen su carácter transversal dentro de Senttinela y pueden ser gestionados también desde capacidades independientes.

Movimiento de entidad utiliza estos registros como información necesaria para representar el hecho económico, procurando que su creación interfiera lo menos posible con el flujo del usuario.

## Evolución

La información registrada por los movimientos podrá servir posteriormente como base para otras capacidades de Senttinela.

Entre ellas pueden encontrarse análisis, resúmenes, visualizaciones u otras formas de presentar información relevante para la organización.

Estas capacidades no forman parte de la definición actual del módulo.

## Principio

El movimiento de entidad busca que la organización pueda registrar lo que ocurrió sin tener que determinar previamente una interpretación posterior sobre ese hecho.

Senttinela debe partir del hecho registrado y permitir que su significado pueda construirse posteriormente a partir de la información disponible.

### Registro de entidades

Movimiento de entidad permite registrar una nueva entidad sin abandonar el flujo actual cuando la contraparte necesaria para registrar el movimiento todavía no existe.

Las entidades registradas desde este flujo mantienen su carácter transversal dentro de Senttinela y no pertenecen exclusivamente a la organización ni al módulo de movimiento de entidad.

El registro debe solicitar únicamente la información necesaria para identificar la entidad y permitir su utilización posterior en movimientos.

La identificación de una entidad se realiza considerando su país y su identificación fiscal, mientras que el nombre normalizado se utiliza principalmente para facilitar su búsqueda.

### Identificación de entidades según el país

La identificación de una entidad depende del país al que pertenece.

El registro de país contiene la denominación del identificador que debe utilizarse en la interfaz. Por ejemplo, Chile utiliza `RUT`.

El formulario de registro de entidad utiliza esta información para mostrar dinámicamente el nombre del campo de identificación.

La obligatoriedad del identificador también depende de la configuración del país. Cuando el país define un identificador, el campo es obligatorio.

El documento de entidad utiliza `identifier` como propiedad general y `searchIdentifier` como representación normalizada destinada a facilitar búsquedas y detección de registros duplicados.

La unicidad del identificador se evalúa dentro del contexto del país, por lo que el mismo valor de identificación puede existir en países diferentes sin representar necesariamente a la misma entidad.


### Artículos dentro de un movimiento

Un movimiento puede contener uno o más artículos.

Cada artículo incluido en el movimiento representa una parte del hecho económico registrado y contiene la información necesaria para determinar su participación en dicho movimiento.

La cantidad representa cuánto del artículo participa en el movimiento.

El precio representa el valor unitario utilizado para ese artículo dentro del movimiento.

El valor total de un artículo se obtiene multiplicando su cantidad por su precio unitario.

El valor total del movimiento corresponde a la suma de los valores de todos sus artículos.

Un artículo puede corresponder a un producto o a un servicio. La unidad de medida se determina a partir de la información registrada para el artículo y no forma parte de la definición del movimiento como una configuración independiente.

### Registro de movimientos

El registro de un movimiento se realiza mediante una instancia temporal de formulario.

El formulario permite seleccionar un artículo, indicar su cantidad y establecer su precio. Cada artículo agregado pasa a formar parte de la colección de artículos del movimiento.

El movimiento solo puede registrarse cuando contiene al menos un artículo.

La cantidad debe ser mayor que cero.

El precio no puede ser negativo.

La información del movimiento representa el estado registrado en el momento del evento. La interpretación contable del movimiento corresponde a otras capacidades del sistema y no forma parte de esta responsabilidad.

