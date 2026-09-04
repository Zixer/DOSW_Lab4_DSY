# 📄 Planeación del Sistema

## Desglose de trabajo: Épicas, Historias de Usuario y Tareas

---

## 1. Épica

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-5 |
| **Título** | Gestión de torneos |
| **Descripción** | TechCup necesita permitir la creación y administración de torneos para centralizar su información y gestionar correctamente su estado durante su ciclo de vida. |
| **Stakeholder** | Organizador del torneo |

---

## 2. Historias de usuario

### 2.1 Historia de Usuario 1

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-6 |
| **Título** | Crear torneo |
| **Descripción** | Como organizador quiero crear un torneo ingresando su información básica, fecha, costo de inscripción y reglas para registrar un nuevo torneo dentro de TechCup. |

| Prioridad | Justificación |
| ------ | ------ |
|  Alta  | Es la funcionalidad principal de la épica, ya que debe existir un torneo antes de que puedan realizarse las demás operaciones de gestión.|

**Estimación Planning Poker:**
* **Story Points:** 8
* **Video de la dinámica:** [Ver grabación aquí](https://drive.google.com/file/d/1Q3ee1zECmCmxjsLe8nZsjqO9mCTWPirY/view?usp=sharing)

---

### 2.2 Historia de Usuario 2

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-7 |
| **Título** | Actualizar información del torneo |
| **Descripción** | Como organizador quiero actualizar la información de un torneo para mantener sus datos correctos y actualizados cuando sea necesario. |

| Prioridad | Justificación |
| ------ | ------ |
| Media  | Es importante para corregir o modificar la información de un torneo, pero el sistema puede funcionar inicialmente si los datos ingresados durante la creación son correctos. |

**Estimación Planning Poker:**
* **Story Points:** 3

---

### 2.3 Historia de Usuario 3

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-8 |
| **Título** | Cambiar estado del torneo |
| **Descripción** | Como organizador quiero cambiar el estado de un torneo para reflejar correctamente la etapa en la que se encuentra. |

| Prioridad | Justificación |
| ------ | ------ |
| Medio  | Los estados permiten controlar el ciclo de vida del torneo y determinar las operaciones que pueden realizarse en cada momento. |

**Estimación Planning Poker:**
* **Story Points:** 2

---

### 2.4 Historia de Usuario 4

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-9 |
| **Título** | Activar torneo |
| **Descripción** | Como organizador quiero activar un torneo para permitir que los equipos puedan iniciar su proceso de inscripción. |

| Prioridad | Justificación |
| ------ | ------ |
| Alta   | Solo los equipos del torneo activo pueden realizar su proceso de inscripción y, según las reglas de negocio, únicamente puede existir un torneo activo al mismo tiempo. |

**Estimación Planning Poker:**
* **Story Points:** 5

---

## 3. Tareas

### 3.1 Tareas de HU-01 – Crear torneo

#### Tarea 1

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-17 |
| **Título** | Crear interfaz de creación de torneo |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Diseñar e implementar el formulario que permita al organizador ingresar la información necesaria para crear un torneo. |
| **Tareas requisito** | Ninguna |

#### Tarea 2

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-18 |
| **Título** | Implementar almacenamiento de torneos |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Crear la estructura necesaria para almacenar la información de los torneos en el sistema. |
| **Tareas requisito** | Ninguna |

#### Tarea 3

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-19 |
| **Título** | Implementar lógica de creación de torneos |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Implementar la lógica para registrar un torneo y validar las reglas de negocio relacionadas con su creación, incluyendo el ID único de cinco dígitos y la duración máxima de un día. |
| **Tareas requisito** | TR-02 |

#### Tarea 4

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-20 |
| **Título** | Integrar creación de torneo |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Integrar la interfaz de creación con la lógica y el almacenamiento de torneos. |
| **Tareas requisito** | SCRUM-17, SCRUM-19 |

---

### 3.2 Tareas de HU-02 – Actualizar información del torneo

#### Tarea 5

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-21 |
| **Título** | Crear interfaz de edición de torneo |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Diseñar e implementar la interfaz que permita al organizador modificar la información de un torneo existente. |
| **Tareas requisito** | Ninguna |

#### Tarea 6

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-22 |
| **Título** | Implementar lógica de actualización |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Implementar la lógica necesaria para validar y actualizar la información modificable de un torneo. |
| **Tareas requisito** | Ninguna |

#### Tarea 7

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-23 |
| **Título** | Integrar actualización de torneo |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Integrar la interfaz de edición con la lógica de actualización y guardar los cambios realizados por el organizador. |
| **Tareas requisito** | SCRUM-21, SCRUM-22 |

---

### 3.3 Tareas de HU-03 – Cambiar estado del torneo

#### Tarea 8

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-24 |
| **Título** | Crear control de cambio de estado |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Diseñar e implementar la interfaz que permita al organizador seleccionar un nuevo estado para el torneo. |
| **Tareas requisito** | Ninguna |

#### Tarea 9

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-25 |
| **Título** | Implementar validación de estados |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Implementar la lógica para validar los estados permitidos del torneo: Pending, Active, In Progress, Closed y Cancelled. |
| **Tareas requisito** | Ninguna |

#### Tarea 10

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-26 |
| **Título** | Actualizar estado del torneo |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Implementar la actualización y almacenamiento del nuevo estado seleccionado por el organizador. |
| **Tareas requisito** | SCRUM-24, SCRUM-25 |

---

### 3.4 Tareas de HU-04 – Activar torneo

#### Tarea 11

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-27 |
| **Título** | Consultar torneo activo |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Implementar la consulta que permita determinar si actualmente existe otro torneo con estado Active. |
| **Tareas requisito** | Ninguna |

#### Tarea 12

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-28 |
| **Título** | Validar activación del torneo |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Implementar la regla de negocio que impida activar un torneo cuando ya exista otro torneo activo. |
| **Tareas requisito** | SCRUM-27 |
