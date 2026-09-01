# Especificación de Requerimientos

## 1. Descripción del sistema

## 2. Integrantes

- Nombre:
- Nombre:
- Nombre:
- Nombre:
- Nombre:

## 3. Requerimientos Funcionales

### RF-01 - [Nombre del requerimiento]

#### Resumen

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|

#### Reglas o condiciones

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|

#### Resultado esperado


### RF-02 - Consulta de Tutorías Disponibles

#### Resumen

Permite a un estudiante consultar las tutorías disponibles indicando la fecha de interés y, de manera opcional, una asignatura o tema, para conocer las opciones existentes y sus cupos disponibles.

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|
| fecha | Date | Fecha para la cual se desea consultar tutorías disponibles |
| tema | String (opcional) | Asignatura o tema de interés para filtrar la búsqueda |

#### Reglas o condiciones

- La fecha de consulta es obligatoria.
- El tema o asignatura es un criterio de búsqueda opcional.
- Si no existen tutorías que coincidan con la búsqueda, el sistema debe informar al estudiante.

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|
| idTutoria | Integer | Identificador de la tutoría encontrada |
| tema | String | Tema de la tutoría |
| profesor | String | Profesor responsable de la tutoría |
| fecha | Date | Fecha de la tutoría |
| horaInicio | Time | Hora de inicio de la tutoría |
| cuposDisponibles | Integer | Cantidad de cupos que aún se encuentran disponibles |

#### Resultado esperado

El estudiante recibe el listado de tutorías que coinciden con los criterios de búsqueda, incluyendo los cupos disponibles en cada una; si no hay coincidencias, recibe un mensaje informándolo.

### RF-03 - [Nombre del requerimiento]

#### Resumen

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|

#### Reglas o condiciones

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|

#### Resultado esperado


### RF-04 - [Nombre del requerimiento]

#### Resumen

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|

#### Reglas o condiciones

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|

#### Resultado esperado


## 4. Gestión de Versiones

### Ramas utilizadas

### Proceso de integración

### Conflictos encontrados