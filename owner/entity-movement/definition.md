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
