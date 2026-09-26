# Arquitectura de Senttinela

## 1. Filosofía arquitectónica

Senttinela es una aplicación monolítica modular que toma conceptos de la arquitectura de microfrontends para organizar sus módulos.

Cada módulo debe poder evolucionar de forma independiente respecto de los demás.

Se acepta cierta duplicación de código cuando dicha duplicación permite mantener la independencia y reducir el acoplamiento entre módulos.

La reutilización de código no debe introducirse únicamente para eliminar duplicación. Antes de reutilizar código se debe evaluar el nivel de dependencia y acoplamiento que dicha reutilización generaría.

## 2. Módulos independientes

Los módulos funcionales de Senttinela deben mantenerse desacoplados entre sí.

Un módulo no debe depender directamente de otro módulo funcional para implementar su comportamiento.

La existencia de funcionalidades similares entre módulos no implica que deban compartir necesariamente su implementación.

Cada módulo puede tener sus propios componentes, servicios, estado, rutas y lógica de presentación.

La duplicación es aceptable cuando contribuye a mantener la independencia del módulo.

## 3. Infraestructura de la aplicación

La infraestructura necesaria para iniciar y ejecutar Senttinela pertenece al nivel de aplicación y no a un módulo funcional específico.

Entre esta infraestructura se encuentran los mecanismos necesarios para inicializar:

- Angular Router.
- Firebase.
- Firebase Authentication.
- Firestore.
- NgRx Store.
- NgRx Effects.
- Otros proveedores globales que sean necesarios para ejecutar la aplicación.

Los módulos pueden utilizar las capacidades proporcionadas por esta infraestructura mediante los mecanismos de inyección de dependencias de Angular.

Los módulos no deben depender de otros módulos funcionales para acceder a esta infraestructura.

## 4. Principio de evolución

La arquitectura de Senttinela debe favorecer cambios pequeños y progresivos.

Las decisiones arquitectónicas deben buscar que un cambio realizado en un módulo tenga el menor impacto posible sobre otros módulos.

La arquitectura debe evolucionar junto con las necesidades reales de la aplicación, evitando introducir abstracciones o estructuras que todavía no sean necesarias.

## 5. Privacidad y separación de organizaciones

La información operacional de una organización debe permanecer separada de las demás organizaciones.

Entidades, artículos y movimientos pertenecen a la organización que los registra. El acceso se limita al contexto de dicha organización y no se habilita automáticamente al rol Super Administrador.

Esta separación busca reducir exposición innecesaria de información y acompaña la evolución de Senttinela hacia la protección de datos desde el diseño, considerando la Ley N.º 19.628 modificada por la Ley N.º 21.719.
