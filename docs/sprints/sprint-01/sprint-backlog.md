# Sprint Backlog — Sprint 01

## Meta del Sprint (Sprint Goal)

Implementar la navegación principal del catálogo de comercios y la vista detallada de los servicios ofertados (Épica 1 completa: Catálogo y Selección de Servicios).

## Información del Sprint

- **Duración:** 2 semanas
- **Inicio:** [Fecha de inicio]
- **Fin:** [Fecha de fin]
- **Equipo:** Dev Team

---

## Historias de Usuario Seleccionadas y Criterios de Aceptación

### US-01 — Búsqueda y Filtrado de Negocios
**Como** usuario cliente  
**Quiero** buscar por nombre o filtrar por categoría los negocios disponibles  
**Para** encontrar rápidamente el comercio de mi interés (Spa, Barbería, Consultorio, etc.).

#### Criterios de Aceptación:
- [ ] La pantalla principal debe desplegar un listado de comercios en formato de tarjetas.
- [ ] La barra de búsqueda debe permitir filtrar en tiempo real por el nombre del comercio.
- [ ] Debe existir un selector/filtro de categorías (ej. Spa, Barbería, Consultorio).
- [ ] Si la búsqueda o filtro no produce resultados, la interfaz debe mostrar un mensaje claro informándolo.
- [ ] **Prioridad:** Alta | **Estimación:** 5 puntos

---

### US-02 — Consulta del Catálogo de Servicios
**Como** usuario cliente  
**Quiero** seleccionar un comercio específico  
**Para** visualizar la lista completa de sus servicios disponibles con sus precios y duraciones.

#### Criterios de Aceptación:
- [ ] Al hacer clic en una tarjeta de negocio, la aplicación debe redirigir a la vista de catálogo del comercio seleccionado.
- [ ] La vista debe mostrar el nombre, imagen e información básica del negocio.
- [ ] La lista de servicios debe detallar claramente el nombre del servicio, precio en moneda local y duración estimada.
- [ ] **Prioridad:** Alta | **Estimación:** 3 puntos

---

### US-03 — Ver Detalle de un Servicio
**Como** usuario cliente  
**Quiero** hacer clic en un servicio específico  
**Para** ver la descripción completa, especialistas asignados y especificaciones antes de agendar.

#### Criterios de Aceptación:
- [ ] Debe existir una pantalla o modal con el detalle individual del servicio seleccionado.
- [ ] La vista debe incluir: descripción detallada del servicio, precio, duración exacta y lista de especialistas disponibles.
- [ ] Debe incluir un botón visible de acción ("Agendar" / "Seleccionar fecha") para el flujo del siguiente Sprint.
- [ ] Debe permitir regresar a la vista general del catálogo del negocio de manera intuitiva.
- [ ] **Prioridad:** Media | **Estimación:** 3 puntos

---

## Desglose de Tareas

| Historia de Usuario | Tarea Específica de Trabajo | Responsable | Estado |
|---|---|---|---|
| **US-01: Búsqueda y Filtrado** | Diseñar interfaz UI/UX de la pantalla de catálogo con tarjetas de negocios y barra de búsqueda. | Frontend Team | Pendiente |
| **US-01: Búsqueda y Filtrado** | Crear estructura JSON / datos ficticios con negocios de categorías (Spa, Barbería, Consultorio). | Backend Team | Pendiente |
| **US-01: Búsqueda y Filtrado** | Implementar la lógica de barra de búsqueda por nombre y selector por categoría. | Frontend Team | Pendiente |
| **US-02: Catálogo de Servicios** | Maquetar la vista de detalle de un negocio mostrando la lista de servicios con precios y duraciones. | Frontend Team | Pendiente |
| **US-02: Catálogo de Servicios** | Conectar la vista de catálogo con la estructura de datos del negocio seleccionado. | Backend Team | Pendiente |
| **US-03: Detalle de Servicio** | Crear la pantalla/modal de detalle individual (descripción, duración, especialistas) con botón de acción. | Frontend Team | Pendiente |

---

## Definición de "Terminado" (Definition of Done)

- [ ] El código está integrado en la rama `develop` mediante Pull Request revisado[cite: 1].
- [ ] La interfaz ha sido probada localmente y cumple con los diseños establecidos.
- [ ] No existen errores o advertencias en la consola durante la navegación del catálogo.
- [ ] El Product Owner valida que la funcionalidad cumple todos los criterios de aceptación de cada Historia de Usuario[cite: 1].

---

## Notas del Equipo

_(Espacio reservado para registrar decisiones durante el Sprint, acuerdos tomados en las reuniones diarias o impedimentos resueltos)_
