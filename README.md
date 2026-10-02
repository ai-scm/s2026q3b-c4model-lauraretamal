# Modelo C4 - Control de Dailies en Microsoft Teams

## Introducción al C4 Model

El C4 Model permite representar la arquitectura de un sistema mediante diferentes niveles de detalle. En este ejercicio se utilizan los tres primeros niveles: Contexto, Contenedores y Componentes.

### C1 - Contexto

El nivel C1 muestra el sistema desde una perspectiva general. Permite identificar el sistema que se está construyendo, los usuarios que interactúan con él y los sistemas externos con los que se relaciona.

### C2 - Contenedores

El nivel C2 muestra cómo está estructurado internamente el sistema, dividiéndolo en contenedores que representan las principales partes de la solución y sus responsabilidades.

### C3 - Componentes

El nivel C3 profundiza en los contenedores, mostrando sus principales componentes y cómo estos se relacionan para cumplir las responsabilidades definidas en el nivel anterior.

## Lógica de estructuración del sistema

La solución se estructuró alrededor de un sistema de control de dailies integrado con Microsoft Teams. En C1 se identificaron los actores principales, Scrum Master y Scrum Team Member, junto con Microsoft Teams como sistema externo. En C2, el sistema se dividió en Teams App, Daily Reports API, Scheduler y Reports Database, separando la interacción con los usuarios, el procesamiento de los reportes, las tareas programadas y el almacenamiento de la información.

En C3 se detallaron los contenedores que requieren mayor nivel de descomposición. Teams App contiene los componentes relacionados con la captura e interacción de los reportes; Daily Reports API concentra el procesamiento, validación y detección de temas repetidos; y Scheduler contiene las tareas encargadas de los recordatorios y la revisión de reportes faltantes. Reports Database se mantiene como un contenedor de almacenamiento sin una descomposición adicional.
