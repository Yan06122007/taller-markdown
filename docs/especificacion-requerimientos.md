# Especificación de Requerimientos

## 1. Descripción del sistema

La Universidad busca y desea implementar una Plataforma de Tutorías Académicas que permita centralizar la organización de las tutorías ofrecidas por los profesores. El sistema permite a los profesores registrar tutorías indicando tema, fecha, hora y cupo máximo; a los estudiantes consultar las tutorías disponibles según la fecha que se tenga y, opcionalmente, tema, en donde pueda inscribirse a una tutoría de su interés, y cancelar una inscripción previamente realizada.

## 2. Integrantes

- Nombre: Yandriani Castañeda (A00416489)
- Nombre: Alejandro Ávila (A00416224)
- Nombre: Samuel Sepúlveda (A00031296)
- Nombre: Juan Acosta (A00421737)
- Nombre: Joshua García (A00418614)

## 3. Requerimientos Funcionales

### RF-01 - Registro de Tutoría

#### Resumen

Permite a un profesor registrar una nueva tutoría indicando el tema, la fecha, la hora de inicio y la cantidad máxima de estudiantes que podrá atender, para que posteriormente los estudiantes puedan encontrarla y solicitar su inscripción.

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|
| codigoProfesor | String | Código que identifica al profesor que registra la tutoría |
| tema | String | Tema o asignatura de la tutoría |
| fecha | Date | Fecha en la que se realizará la tutoría |
| horaInicio | Time | Hora de inicio de la tutoría |
| cupoMaximo | Integer | Cantidad máxima de estudiantes que podrán inscribirse |

#### Reglas o condiciones

- La fecha de la tutoría no puede ser anterior a la fecha actual.
- El cupo máximo debe estar entre 1 y 10 estudiantes.
- El código de profesor debe corresponder a un profesor válido registrado en el sistema.

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|
| idTutoria | Integer | Identificador único asignado a la tutoría creada |
| mensajeConfirmacion | String | Mensaje que informa al profesor que la tutoría fue creada correctamente |

#### Resultado esperado

Se crea un nuevo registro de tutoría en el sistema con un identificador único, quedando disponible para que los estudiantes puedan consultarla y solicitar su inscripción.


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

### RF-03 - Inscripción a Tutoría

#### Resumen

Permite a un estudiante inscribirse en una tutoría de su interés indicando su código estudiantil y el identificador de la tutoría, siempre que se cumplan las condiciones necesarias para completar la inscripción.

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|
| codigoEstudiante | String | Código que identifica al estudiante que desea inscribirse |
| idTutoria | Integer | Identificador de la tutoría en la que se desea inscribir |

#### Reglas o condiciones

- El estudiante debe encontrarse activo en la Universidad.
- La tutoría debe existir.
- La tutoría debe tener al menos un cupo disponible.
- El estudiante no puede encontrarse previamente inscrito en la misma tutoría.

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|
| mensajeConfirmacion | String | Mensaje que confirma la inscripción exitosa o informa el motivo del rechazo |
| cuposDisponiblesActualizados | Integer | Cantidad de cupos disponibles luego de registrar la inscripción |

#### Resultado esperado

Si se cumplen todas las condiciones, se registra la inscripción del estudiante y se reduce en uno la cantidad de cupos disponibles de la tutoría. Si alguna condición no se cumple, la inscripción no se realiza y se informa al estudiante el motivo.


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

- main
- develop
- feature/rf01-registro-tutoria
- feature/rf02-consulta-tutorias
- feature/rf03-inscripcion-tutoria
- feature/rf04-cancelacion-inscripcion

### Proceso de integración

```text
main
   ↓
develop
   ↓
feature/rf01, feature/rf02, feature/rf03, feature/rf04
   ↓
develop (Pull Request por cada feature)
   ↓
main (Pull Request final)
```

### Conflictos encontrados

No se presentaron conflictos durante la integración.