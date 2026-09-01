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


### RF-02 - [Nombre del requerimiento]

#### Resumen

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|

#### Reglas o condiciones

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|

#### Resultado esperado


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

### Proceso de integración

### Conflictos encontrados