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

Como usuario de la plataforma, quiero buscar recetas mediante palabras clave, ingredientes, tiempos de preparación y características específicas, para encontrar alternativas gastronómicas que se ajusten con precisión a mis gustos, disponibilidad de ingredientes y tiempo.

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

[Justificación de los resultados útiles que separa la división.]

## US-01

**Título:** Búsqueda de recetas por nombre o palabra clave

Como usuario de la plataforma, quiero buscar recetas introduciendo palabras clave, frases o el autor específico en un campo dedicado, para obtener un listado de resultados relevantes ordenados adecuadamente con su vista previa detallada.

**Fuentes:** UR-08; UC-21; FR-85; acta, apartado 3.1.

### Criterios de aceptación

- **CA-01.** Dado una receta publicada y validada como "tomate", cuando la persona busca "tomate", entonces esa receta aparece en todos los resultados
- **CA-02.** Dado recetas con "salmón" en el título o la descripción breve, cuando el usuario busca "salmón", entonces entonces esa receta aparece en todos los resultados 
- **CA-03.** Dado que el usuario ingresa el nombre de un creador en la casilla de búsqueda, cuando confirma la consulta, entonces el sistema filtra y devuelve únicamente las recetas pertenecientes a dicho autor o creador específico.

## US-02

**Título:** Filtrado e inclusión/exclusión de ingredientes y alérgenos

Como usuario o cocinero, quiero seleccionar ingredientes para incluir o excluir en la búsqueda, para filtrar las recetas según los alimentos que tengo disponibles o evitar aquellos que causan alergias o no son de mi agrado.

**Fuentes:** UR-08; UC-21; FR-86; acta, 3.2

### Criterios de aceptación

- **CA-01.** Dado que el usuario marca una lista de ingredientes seleccionados, cuando ejecuta la búsqueda, entonces el sistema devuelve únicamente aquellas recetas que contengan la totalidad de los ingredientes indicados.
- **CA-02.** Dado que el usuario indica ingredientes a excluir de la consulta, cuando aplica el filtro, entonces el sistema elimina del listado cualquier receta que contenga dichos elementos no deseados o alérgenos.
- **CA-03.** Dado que el usuario tiene configuradas sus alergias e intolerancias alimentarias en su perfil de usuario, cuando inicia una búsqueda, entonces el sistema aplica automáticamente la restricción para no mostrar recetas con dichos componentes alérgenos.

## US-03

**Título:** Filtrado por tipo de comida, tiempo de preparación y dificultad

Como usuario con agenda apretada, quiero filtrar el catálogo por tipo de comida, tiempo estimado y nivel de dificultad,
para encontrar de forma eficiente platillos acordes al momento del día y al tiempo del que dispongo para cocinar.

**Fuentes:** UR-08; UC-21; FR-090; acta, 3.3

### Criterios de aceptación

- **CA-01.** Dado que el usuario accede al panel de filtros, cuando realiza una selección múltiple sobre los tipos de comida (desayuno, almuerzo, cena), entonces el sistema muestra las recetas asociadas a cualquiera de las categorías seleccionadas.
- **CA-02.** Dado que el usuario marca un rango de tiempo de preparación (menos de 15 minutos, 30 minutos, más de una hora), cuando aplica el filtro, entonces el sistema restringe los resultados a las recetas cuya duración se ajuste al criterio seleccionado.
- **CA-03.** Dado que el usuario selecciona un nivel de dificultad específico (fácil, intermedio, avanzado), cuando actualiza los resultados, entonces el sistema muestra las recetas clasificadas exactamente en dicho nivel.

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | Si | Sí | [Historias y motivo] |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | Sí | Sí | [Historias y motivo] |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | Sí | Sí | [Historias y motivo] |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | Sí | Sí | [Historias y motivo] |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | Sí | Sí | [Historias y motivo] |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | Sí | Sí | [Historias y motivo] |

## Dudas pendientes

[Cuestiones pendientes de aclaración. Si no quedan cuestiones, indicar «Ninguna».]
