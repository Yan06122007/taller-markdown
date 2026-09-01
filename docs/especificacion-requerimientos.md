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