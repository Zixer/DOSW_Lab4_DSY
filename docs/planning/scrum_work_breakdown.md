# 📄 Planeación del Sistema

## Desglose de trabajo: Épicas, Historias de Usuario y Tareas

La implementación de los requerimientos identificados de TechCup se desglosa de la siguiente manera:

## 1. Épica

| Campo | Descripción |
|------|-------------|
| **ID** | EP-01 |
| **Título** | Gestión de torneos e inscripciones |
| **Descripción** | TechCup necesita gestionar de manera centralizada la creación de torneos y el proceso de inscripción de los equipos, incluyendo el pago y la aprobación de su participación. |
| **Stakeholder** | Organizadores del torneo y capitanes de equipo |

---

## 2. Historias de usuario

### 2.1 Crear torneo

| Campo | Descripción |
|------|-------------|
| **ID** | HU-01 |
| **Título** | Crear torneo |
| **Descripción** | Como organizador quiero crear un torneo ingresando su información básica, fecha, costo de inscripción y reglas para gestionar y habilitar un nuevo torneo en TechCup |
| **Prioridad** | Alta |
| **Estimación** | 5 puntos de historia |

### 2.2 Realizar pago de inscripción

| Campo | Descripción |
|------|-------------|
| **ID** | HU-02 |
| **Título** | Realizar pago de inscripción |
| **Descripción** | Como capitán de equipo quiero realizar el pago de inscripción mediante PSE para que mi equipo pueda participar en el torneo activo |
| **Prioridad** | Alta |
| **Estimación** | 8 puntos de historia |

### 2.3 Aprobar inscripción

| Campo | Descripción |
|------|-------------|
| **ID** | HU-03 |
| **Título** | Aprobar inscripción de un equipo |
| **Descripción** | Como organizador quiero revisar y aprobar la inscripción de un equipo para confirmar su participación en el torneo activo. |
| **Prioridad** | Alta |
| **Estimación** | 5 puntos de historia |

---

## 3. Tareas

### 3.1 Tareas asociadas a HU-01 – Crear torneo

#### Tarea 1

| Campo | Descripción |
|------|-------------|
| **ID** | TR-01 |
| **Título** | Crear interfaz de creación de torneo |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Diseñar e implementar la interfaz que permita al organizador ingresar la información necesaria para crear un torneo. |
| **Tareas requisito** | Ninguna |

#### Tarea 2

| Campo | Descripción |
|------|-------------|
| **ID** | TR-02 |
| **Título** | Implementar almacenamiento de torneos |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Implementar la estructura necesaria en la base de datos para almacenar la información de los torneos. |
| **Tareas requisito** | Ninguna |

#### Tarea 3

| Campo | Descripción |
|------|-------------|
| **ID** | TR-03 |
| **Título** | Implementar lógica de creación de torneos |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Implementar en el backend la lógica para crear un torneo y validar sus reglas de negocio, incluyendo el ID de cinco dígitos y su duración máxima de un día. |
| **Tareas requisito** | TR-02 |

#### Tarea 4

| Campo | Descripción |
|------|-------------|
| **ID** | TR-04 |
| **Título** | Integrar creación de torneo |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Integrar la interfaz de creación de torneo con la lógica implementada en el backend. |
| **Tareas requisito** | TR-01, TR-03 |

---

### 3.2 Tareas asociadas a HU-02 – Realizar pago de inscripción

#### Tarea 5

| Campo | Descripción |
|------|-------------|
| **ID** | TR-05 |
| **Título** | Crear interfaz de pago |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Diseñar e implementar la interfaz desde la cual el capitán pueda iniciar el pago de inscripción de su equipo. |
| **Tareas requisito** | Ninguna |

#### Tarea 6

| Campo | Descripción |
|------|-------------|
| **ID** | TR-06 |
| **Título** | Implementar integración con PSE |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Implementar la comunicación entre TechCup y el servicio PSE para procesar el pago de inscripción. |
| **Tareas requisito** | Ninguna |

#### Tarea 7

| Campo | Descripción |
|------|-------------|
| **ID** | TR-07 |
| **Título** | Registrar información del pago |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Implementar el almacenamiento de la información y el estado de las transacciones realizadas mediante PSE. |
| **Tareas requisito** | TR-06 |

#### Tarea 8

| Campo | Descripción |
|------|-------------|
| **ID** | TR-08 |
| **Título** | Integrar flujo de pago |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Integrar la interfaz de pago con PSE y mostrar al capitán el resultado de la transacción realizada. |
| **Tareas requisito** | TR-05, TR-06, TR-07 |

---

### 3.3 Tareas asociadas a HU-03 – Aprobar inscripción

#### Tarea 9

| Campo | Descripción |
|------|-------------|
| **ID** | TR-09 |
| **Título** | Crear interfaz de inscripciones pendientes |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Diseñar e implementar la interfaz que permita al organizador consultar los equipos que tienen una inscripción pendiente de aprobación. |
| **Tareas requisito** | Ninguna |

#### Tarea 10

| Campo | Descripción |
|------|-------------|
| **ID** | TR-10 |
| **Título** | Implementar consulta de pagos |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Implementar la consulta de la información del pago asociado a cada equipo para que pueda ser revisada por el organizador. |
| **Tareas requisito** | TR-07 |

#### Tarea 11

| Campo | Descripción |
|------|-------------|
| **ID** | TR-11 |
| **Título** | Implementar aprobación de inscripción |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Implementar la lógica que permita aprobar la inscripción del equipo después de verificar el pago correspondiente. |
| **Tareas requisito** | TR-10 |

#### Tarea 12

| Campo | Descripción |
|------|-------------|
| **ID** | TR-12 |
| **Título** | Integrar aprobación de inscripción |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Integrar la interfaz de inscripciones pendientes con la lógica de aprobación y actualizar el estado de la inscripción del equipo. |
| **Tareas requisito** | TR-09, TR-11 |