# País

## Definición

Un país representa una configuración territorial utilizada por Senttinela para registrar información asociada a personas, empresas y otros tipos de sujetos.

Además de información general del país, esta configuración puede definir cómo se identifica cada tipo de sujeto dentro de ese país.

## Información del país

Un país puede contener información como:

- Nombre.
- Nombre normalizado.
- Código telefónico.
- Extensión de dominio.
- Estado.
- Fecha de creación.

## Tipos de sujeto

Cada país puede definir qué tipos de sujeto utiliza.

Por ejemplo, Chile puede utilizar:

- Persona.
- Empresa.
- Grupo.

La configuración del tipo de sujeto dentro del país puede incluir información relacionada con su identificación.

## Identificación por país

La forma de identificar un sujeto depende del país.

Por ejemplo, para Chile:

- Una persona puede utilizar RUN.
- Una empresa puede utilizar RUT.
- Un grupo puede no utilizar un identificador.

La configuración se realiza dentro del país y no dentro del tipo de sujeto global.

## Identificador

Cuando un tipo de sujeto utiliza un identificador dentro de un país, la configuración puede indicar:

- Tipo de identificador.
- Nombre mostrado al usuario.
- Patrón esperado.
- Si el identificador es opcional.

Por ejemplo, una configuración puede indicar que una empresa en Chile utiliza RUT.

## Identificador opcional

Un identificador puede configurarse como opcional.

Esto permite registrar sujetos aunque el usuario no conozca o no disponga del identificador al momento del registro.

Por ejemplo, un usuario puede registrar una empresa únicamente con su nombre y completar posteriormente el identificador.

La posibilidad de utilizar un identificador y la obligatoriedad del mismo son conceptos diferentes.

## Responsabilidad del país

Country es responsable de definir las reglas que dependen del país.

El tipo de sujeto solamente proporciona el concepto general.

Esto permite utilizar el mismo tipo de sujeto en distintos países sin asociarlo permanentemente a una identificación determinada.

## Administración

Los países son administrados por el rol Super Administrator.

La configuración realizada por este rol posteriormente es utilizada por otros contextos de Senttinela.

El Owner no necesita conocer ni configurar estas reglas.
