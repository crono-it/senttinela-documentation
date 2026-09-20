# País

## Definición

Un país representa una configuración territorial utilizada por Senttinela.

Además de sus datos generales, define qué tipos de sujeto pueden utilizarse en ese país y si el identificador de cada tipo es obligatorio u opcional.

## Información general

Actualmente un país puede contener:

- Nombre.
- Nombre normalizado.
- Código telefónico.
- Extensión de dominio.
- Tipos de sujeto disponibles.
- Estado.
- Fecha de creación.

## Tipos de sujeto

Cada país conserva los tipos de sujeto habilitados para su contexto. Por ejemplo, Chile puede utilizar Persona, Empresa y Grupo.

Cuando un tipo de sujeto admite identificador, el país puede indicar si ese identificador es opcional.

## Separación de responsabilidades

El país no exige al administrador conocer expresiones regulares ni algoritmos matemáticos de validación. Los detalles técnicos necesarios para interpretar identificadores se mantienen en la aplicación.

Esto permite que la configuración administrativa permanezca comprensible y que los formularios de uso cotidiano puedan aplicar las reglas correspondientes automáticamente.
