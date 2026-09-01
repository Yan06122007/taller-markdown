# Especificación de Requerimientos

## 1. Descripción del sistema

## 2. Integrantes

- Nombre: Yandriani Castañeda (A00416489)
- Nombre:
- Nombre:
- Nombre:
- Nombre:

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


## 4. Gestión de Versiones

### Ramas utilizadas

### Proceso de integración

### Conflictos encontrados