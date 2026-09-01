# 📄 Planeación del Sistema

## Desglose de trabajo: Épicas, Historias de Usuario y Tareas

---

## 1. Épica

| Campo | Descripción |
|------|-------------|
| **ID** | EP-01 |
| **Título** | Gestión de torneos |
| **Descripción** | TechCup necesita permitir la creación y administración de torneos para centralizar su información y gestionar correctamente su estado durante su ciclo de vida. |
| **Stakeholder** | Organizador del torneo |

---

## 2. Historias de usuario

### 2.1 Historia de Usuario 1

| Campo | Descripción |
|------|-------------|
| **ID** | HU-01 |
| **Título** | Crear torneo |
| **Descripción** | Como organizador quiero crear un torneo ingresando su información básica, fecha, costo de inscripción y reglas para registrar un nuevo torneo dentro de TechCup. |
| **Prioridad** | Alta |
| **Justificación de prioridad** | Es la funcionalidad principal de la épica, ya que debe existir un torneo antes de que puedan realizarse las demás operaciones de gestión. |

---

### 2.2 Historia de Usuario 2

| Campo | Descripción |
|------|-------------|
| **ID** | HU-02 |
| **Título** | Actualizar información del torneo |
| **Descripción** | Como organizador quiero actualizar la información de un torneo para mantener sus datos correctos y actualizados cuando sea necesario. |
| **Prioridad** | Media |
| **Justificación de prioridad** | Es importante para corregir o modificar la información de un torneo, pero el sistema puede funcionar inicialmente si los datos ingresados durante la creación son correctos. |

---

### 2.3 Historia de Usuario 3

| Campo | Descripción |
|------|-------------|
| **ID** | HU-03 |
| **Título** | Cambiar estado del torneo |
| **Descripción** | Como organizador quiero cambiar el estado de un torneo para reflejar correctamente la etapa en la que se encuentra. |
| **Prioridad** | Alta |
| **Justificación de prioridad** | Los estados permiten controlar el ciclo de vida del torneo y determinar las operaciones que pueden realizarse en cada momento. |

---

### 2.4 Historia de Usuario 4

| Campo | Descripción |
|------|-------------|
| **ID** | HU-04 |
| **Título** | Activar torneo |
| **Descripción** | Como organizador quiero activar un torneo para permitir que los equipos puedan iniciar su proceso de inscripción. |
| **Prioridad** | Alta |
| **Justificación de prioridad** | Solo los equipos del torneo activo pueden realizar su proceso de inscripción y, según las reglas de negocio, únicamente puede existir un torneo activo al mismo tiempo. |

---

## 3. Tareas

### 3.1 Tareas de HU-01 – Crear torneo

#### Tarea 1

| Campo | Descripción |
|------|-------------|
| **ID** | TR-01 |
| **Título** | Crear interfaz de creación de torneo |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Diseñar e implementar el formulario que permita al organizador ingresar la información necesaria para crear un torneo. |
| **Tareas requisito** | Ninguna |

#### Tarea 2

| Campo | Descripción |
|------|-------------|
| **ID** | TR-02 |
| **Título** | Implementar almacenamiento de torneos |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Crear la estructura necesaria para almacenar la información de los torneos en el sistema. |
| **Tareas requisito** | Ninguna |

#### Tarea 3

| Campo | Descripción |
|------|-------------|
| **ID** | TR-03 |
| **Título** | Implementar lógica de creación de torneos |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Implementar la lógica para registrar un torneo y validar las reglas de negocio relacionadas con su creación, incluyendo el ID único de cinco dígitos y la duración máxima de un día. |
| **Tareas requisito** | TR-02 |

#### Tarea 4

| Campo | Descripción |
|------|-------------|
| **ID** | TR-04 |
| **Título** | Integrar creación de torneo |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Integrar la interfaz de creación con la lógica y el almacenamiento de torneos. |
| **Tareas requisito** | TR-01, TR-03 |

---

### 3.2 Tareas de HU-02 – Actualizar información del torneo

#### Tarea 5

| Campo | Descripción |
|------|-------------|
| **ID** | TR-05 |
| **Título** | Crear interfaz de edición de torneo |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Diseñar e implementar la interfaz que permita al organizador modificar la información de un torneo existente. |
| **Tareas requisito** | Ninguna |

#### Tarea 6

| Campo | Descripción |
|------|-------------|
| **ID** | TR-06 |
| **Título** | Implementar lógica de actualización |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Implementar la lógica necesaria para validar y actualizar la información modificable de un torneo. |
| **Tareas requisito** | Ninguna |

#### Tarea 7

| Campo | Descripción |
|------|-------------|
| **ID** | TR-07 |
| **Título** | Integrar actualización de torneo |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Integrar la interfaz de edición con la lógica de actualización y guardar los cambios realizados por el organizador. |
| **Tareas requisito** | TR-05, TR-06 |

---

### 3.3 Tareas de HU-03 – Cambiar estado del torneo

#### Tarea 8

| Campo | Descripción |
|------|-------------|
| **ID** | TR-08 |
| **Título** | Crear control de cambio de estado |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Diseñar e implementar la interfaz que permita al organizador seleccionar un nuevo estado para el torneo. |
| **Tareas requisito** | Ninguna |

#### Tarea 9

| Campo | Descripción |
|------|-------------|
| **ID** | TR-09 |
| **Título** | Implementar validación de estados |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Implementar la lógica para validar los estados permitidos del torneo: Pending, Active, In Progress, Closed y Cancelled. |
| **Tareas requisito** | Ninguna |

#### Tarea 10

| Campo | Descripción |
|------|-------------|
| **ID** | TR-10 |
| **Título** | Actualizar estado del torneo |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Implementar la actualización y almacenamiento del nuevo estado seleccionado por el organizador. |
| **Tareas requisito** | TR-08, TR-09 |

---

### 3.4 Tareas de HU-04 – Activar torneo

#### Tarea 11

| Campo | Descripción |
|------|-------------|
| **ID** | TR-11 |
| **Título** | Consultar torneo activo |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Implementar la consulta que permita determinar si actualmente existe otro torneo con estado Active. |
| **Tareas requisito** | Ninguna |

#### Tarea 12

| Campo | Descripción |
|------|-------------|
| **ID** | TR-12 |
| **Título** | Validar activación del torneo |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Implementar la regla de negocio que impida activar un torneo cuando ya exista otro torneo activo. |
| **Tareas requisito** | TR-11 |

#### Tarea 13

| Campo | Descripción |
|------|-------------|
| **ID** | TR-13 |
| **Título** | Implementar activación del torneo |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Implementar la actualización del estado del torneo a Active cuando se cumplan las condiciones establecidas. |
| **Tareas requisito** | TR-12 |

#### Tarea 14

| Campo | Descripción |
|------|-------------|
| **ID** | TR-14 |
| **Título** | Integrar activación del torneo |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Integrar la opción de activación de la interfaz con las validaciones y la lógica correspondiente. |
| **Tareas requisito** | TR-08, TR-12, TR-13 |