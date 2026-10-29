# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Fecha | [dd/mm/aaaa] |
| Versión | [Versión de trabajo] |
| Estado | Borrador |

## Fuentes comunes

- [Acta de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.
- [Catálogo de requisitos](catalogo-requisitos.md), UR-08 y FR pertinentes.
- [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), UC-21.

## Épica de búsqueda

Como usuario registrado, quiero buscar recetas siguiendo diferentes criterios, para gestionar mi dieta y controlar los síntomas de mi enfermedad.

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

Dividir la búsqueda en 3 historias, una por criterio, nos facilita la medición y comprobación de resultados obtenibles.

## US-01

**Título:** Buscar recetas por ingrediente incluido

Como usuario registrado, quiero un sistema que permita buscar recetas que contengan un ingrediente, para obtener un listado de recetas que dispongan de ese ingrediente.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que existen varias recetas con un mismo ingrediente, cuando el usuario busque ese ingrediente, entonces el sistema mostrará todas las recetas que contengan ese ingrediente.
- **CA-02.** Dado que no existe un ingrediente en la base de datos, cuando el usuario busca ese ingrediente, entonces el sistema muestra un mensaje que comunique que no se ha encontrado el ingrediente.
- **CA-03.** Dado que existe un ingrediente, pero ninguna receta lo contiene, cuando el usuario busca ese ingrediente, entonces el sistema muestra un mensaje que comunique que no se ha encontrado la receta.

## US-02

**Título:** Buscar recetas por palabra o frase clave.

Como usuario registrado, quiero buscar recetas por palabra clave, para obtener un listado de recetas que cumplan mis criterios.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que hay recetas que contienen la frase clave "sin gluten", cuando el usuario realiza una búsqueda por la frase clave "sin gluten", entonces el sistema muestra esas recetas
- **CA-02.** Dado que no existe una frase clave, cuando el usuario busca esa frase, entonces el sistema muestra un mensaje que comunique que no se ha encontrado el ingrediente.
- **CA-03.** Dado [situación], cuando [acción], entonces [resultado observable].

## US-03

**Título:** Buscar recetas por ingrediente excluido

Como usuario registrado, quiero buscar recetas sin un ingrediente por palabra clave, para obtener un listado de recetas que no contenga ese ingrediente.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que hay recetas que no contengan la frase clave, cuando el usuario busque esa frase , entonces el sistema muestra un listado de recetas sin ese ingrediente.
- **CA-02.** Dado que no existen recetas sin ese ingrediente, cuando el usuario busque esa frase, entonces el sistema muestra un mensaje de error .
- **CA-03.** Dado [situación], cuando [acción], entonces [resultado observable].

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |

## Dudas pendientes

[Cuestiones pendientes de aclaración. Si no quedan cuestiones, indicar «Ninguna».]
