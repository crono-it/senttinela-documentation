# Tipo de sujeto

## Definición

Un tipo de sujeto representa una categoría general utilizada por Senttinela para describir qué clase de sujeto puede participar en distintos contextos.

Actualmente se utilizan:

- Persona.
- Empresa.
- Grupo.

## Identificación

Un tipo de sujeto puede indicar si conceptualmente admite un identificador mediante `hasIdentifier`.

Esta propiedad no define el nombre, formato ni algoritmo de un identificador concreto. Esas reglas pueden depender del país y de la implementación utilizada por Senttinela.

## Alcance

Los tipos de sujeto son transversales. Pueden ser utilizados tanto por organizaciones como por entidades sin crear tipos independientes para cada contexto.
