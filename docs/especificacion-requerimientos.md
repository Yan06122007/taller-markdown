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


### RF-04 - Cancelación de Inscripción

#### Resumen

Permite a un estudiante previamente inscrito cancelar su participación en una tutoría, utilizando su código estudiantil y el identificador de la tutoría, siempre que la tutoría aún no haya comenzado.

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|
| codigoEstudiante | String | Código del estudiante que desea cancelar su inscripción |
| idTutoria | Integer | Identificador de la tutoría de la cual se desea cancelar la inscripción |

#### Reglas o condiciones

- Debe existir una inscripción previa del estudiante en esa tutoría.
- La tutoría aún no debe haber comenzado.

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|
| mensajeConfirmacion | String | Mensaje que confirma la cancelación exitosa o informa el motivo por el cual no fue posible realizarla |
| cuposDisponiblesActualizados | Integer | Cantidad de cupos disponibles luego de liberar el cupo cancelado |

#### Resultado esperado

Si se cumplen las condiciones, se elimina la inscripción y se libera nuevamente el cupo correspondiente en la tutoría. Si no es posible realizar la cancelación, se informa al estudiante el motivo.