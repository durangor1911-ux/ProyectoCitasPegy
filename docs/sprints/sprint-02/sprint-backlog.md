# Epic Proyecto Integrador Citas Peggy

**Épica 1:** Catálogo y Selección de Servicios

**Feature:** "Como cliente, quiero buscar y elegir un servicio de un negocio para saber qué puedo agendar"

CA: Filtro por categoría, muestra precio y duración, buscador por nombre de negocio

**Historia 2: Ver catálogo de servicios para diferentes negocios**

**Como** cliente
**Quiero** ver los servicios que ofrece un negocio específico
**Para** saber qué puedo agendar ahí

**Épica 2:** Agendamiento y Disponibilidad en Tiempo Real

**Feature: Reserva de horario disponible**

"Como cliente, quiero seleccionar un horario disponible en el calendario para asegurar mi cita"

CA: Bloquea horarios ocupados, reserva temporal de 5 min, libera si no se confirma

**Épica 3:** Validación y Confirmación Automática

**Feature: Confirmación**

"Como sistema, quiero validar y confirmar la cita en tiempo real para evitar que se crucen dos reservas"

CA: Revalida antes de confirmar, notifica a cliente y negocio, rechaza si el horario ya fue tomado

**Épica 4:** Comprobantes y Recordatorios

Como Cliente

Quiero recibir mis comprobantes digitales y recordatorio de mi cita por medio de mensajes

---

# Viviendo nuestro primer Sprint

**Proyecto Integrador:** Citas Peggy (Plataforma de Agendamiento en Tiempo Real)

## 1. Listado Inicial de Actividades

Listado bruto de funcionalidades e historias clave identificadas por el equipo para la plataforma Citas Peggy, redactadas antes del proceso de estructuración en Épicas:

1. Buscar y listar negocios registrados (barberías, spas, consultorios, restaurantes).
2. Filtrar negocios por categoría o tipo de servicio.
3. Ver el catálogo completo de servicios ofertados por un negocio específico con precios y tiempos.
4. Consultar profesionales/especialistas asignados a cada servicio.
5. Visualizar la agenda y horarios disponibles en tiempo real.
6. Seleccionar un horario específico y bloquear la casilla temporalmente para evitar reserva doble (anti-colisión).
7. Confirmar la cita de agendamiento y registrar los datos del cliente.
8. Generar y enviar comprobante digital de reserva con código QR por correo electrónico o WhatsApp.
9. Enviar notificaciones automáticas de recordatorio 24 horas y 2 horas antes de la cita.
10. Permitir al cliente cancelar o reprogramar su cita desde la notificación o plataforma.
11. Visualizar un dashboard/panel de control para administradores con métricas de inasistencias (no-shows) y asistencias.
12. Actualizar inmediatamente el catálogo de disponibilidades cuando se cancela una cita.

## 2. Product Backlog Priorizado (Clase 2)

A continuación se detallan las **5 Épicas** organizadas por orden estricto de prioridad de negocio, incluyendo sus Historias de Usuario desarrolladas bajo el estándar *Como / Quiero / Para* y sus criterios de aceptación.

### Épica 1: Catálogo y Selección de Servicios (Prioridad 1)

**Justificación de Prioridad:** Es el punto de entrada de la plataforma. Sin una interfaz donde el cliente pueda descubrir los comercios y sus ofertas, no es posible generar tráfico ni iniciar la intención de reserva.

**Historia 1.1: Búsqueda y Filtrado de Negocios**

**Como** cliente de la plataforma,
**Quiero** ver y filtrar la lista de negocios registrados por categoría (restaurantes, consultorios, spas, barberías),
**Para** encontrar y elegir fácilmente el establecimiento donde deseo agendar mi cita.

*Criterios de Aceptación:*
- Barra de búsqueda funcional por nombre y selector por categoría.
- Tarjetas con nombre, dirección, imagen y puntuación.

**Historia 1.2: Consulta del Catálogo de Servicios**

**Como** cliente,
**Quiero** ver la lista detallada de servicios que ofrece un negocio específico,
**Para** conocer precios, duración estimada y detalles antes de reservar.

*Criterios de Aceptación:*
- Listado completo de servicios con nombre, precio y tiempo de duración.
- Botón directo "Agendar".

### Épica 2: Agendamiento y Disponibilidad en Tiempo Real (Prioridad 2)

**Justificación de Prioridad:** Es el núcleo operativo de la solución. Permite al cliente conectar la intención de compra con una franja horaria y un profesional concreto.

**Historia 2.1: Selección de Especialista y Horario Libre**

**Como** cliente,
**Quiero** ver los especialistas disponibles y sus franjas horarias libres según el servicio seleccionado,
**Para** elegir al profesional de mi preferencia y la hora que mejor se acomode a mi tiempo.

*Criterios de Aceptación:*
- Permitir opción "Cualquier especialista disponible".
- Deshabilitar automáticamente las horas pasadas u ocupadas.

### Épica 3: Validación y Confirmación Automática (Prioridad 3)

**Justificación de Prioridad:** Garantiza la consistencia técnica de la base de datos y la confianza del usuario, previniendo el mayor problema operativo del negocio: la reserva duplicada.

**Historia 3.1: Bloqueo Temporal Anti-Colisión**

**Como** cliente,
**Quiero** que el sistema valide y bloquee mi horario seleccionado durante el proceso de reserva,
**Para** evitar que otro usuario reserve la misma casilla simultáneamente.

*Criterios de Aceptación:*
- Bloqueo de la casilla por 5 minutos durante la sesión.
- Re-validación final en base de datos al dar clic en "Confirmar".

### Épica 4: Comprobantes y Recordatorios (Prioridad 4)

**Justificación de Prioridad:** Aporta valor post-venta y comunicación automatizada, mejorando la experiencia del usuario una vez la cita ya está reservada.

**Historia 4.1: Emisión de Comprobante Digital**

**Como** cliente,
**Quiero** recibir un comprobante digital de mi reserva (vía correo / WhatsApp),
**Para** conservar la información de respaldo con la fecha, hora y código de reserva.

**Historia 4.2: Recordatorios Automáticos**

**Como** cliente,
**Quiero** recibir alertas de recordatorio previas a mi cita (24h y 2h antes),
**Para** planificar mi asistencia o reprogramar a tiempo.

### Épica 5: Métricas y Reducción de Inasistencias (Prioridad 5)

**Justificación de Prioridad:** Aunque es vital para la rentabilidad a largo plazo, requiere que la plataforma ya tenga usuarios y transacciones operando para generar datos significativos.

**Historia 5.1: Panel de Control de Inasistencias (Rol Administrador)**

**Como** administrador del negocio,
**Quiero** consultar un panel analítico con métricas de asistencia e inasistencias (no-shows),
**Para** tomar decisiones operativas y políticas que aseguren la ocupación del establecimiento.

**Historia 5.2: Cancelación / Reprogramación Rápida (Rol Cliente)**

**Como** cliente,
**Quiero** cancelar o reprogramar mi cita de forma sencilla,
**Para** liberar el horario del establecimiento si no puedo asistir.

## 3. Bitácora de Uso e Integración de IA (Clase 2)

| Elemento | Detalle del Registro |
|---|---|
| **Herramienta Utilizada** | Gemini (Google) / ChatGPT |
| **Prompt Inicial Formulado** | *"Actúa como un Agile Coach y Product Owner experto. Tengo un proyecto integrador llamado 'Citas Peggy', una plataforma de agendamiento en tiempo real para barberías, spas y consultorios. Agrupa este listado de 12 actividades en épicas lógicas con nombres profesionales de negocio e indica las historias de usuario clave."* |
| **Evaluación Crítica del Equipo** | La IA propuso inicialmente agrupaciones puramente técnicas (ej. "Módulo de Frontend", "Módulo de Base de Datos"). Además, colocó los reportes analíticos de inasistencias dentro del rol de cliente. |
| **Ajustes y Decisiones del Equipo** | 1. Se reformularon las Épicas hacia valor de negocio (Catálogo, Agendamiento, Validación, Comprobantes, Métricas).<br>2. Se corrigió el rol de la Épica 5 (Métricas), separando las vistas de Administrador de las del Cliente.<br>3. Se realizó la priorización (E1 > E2 > E3 > E4 > E5) 100% por criterio del equipo sin intervención de la IA. |

## 4. Configuración del Repositorio de Código (Clase 3)

El equipo ha establecido el control de versiones formal en GitHub como evidencia de trabajo y entrega continua:

- **URL del Repositorio GitHub:** https://github.com/equipo-citas-peggy/citas-peggy-app

- **Comandos ejecutados para la inicialización:**

```bash
git init
git add .
git commit -m "Initial commit: Estructura base del proyecto Citas Peggy y documentación Scrum"
git branch -M main
git remote add origin https://github.com/equipo-citas-peggy/citas-peggy-app.git
git push -u origin main
```

## 5. Asignación de Roles Scrum (Clase 3)

| Rol Scrum | Integrante del Equipo | Responsabilidades Principales en el Sprint |
|---|---|---|
| **Product Owner (PO)** | [Nombre del Integrante 1] | Define la visión del producto, valida que los entregables cumplan con la necesidad del negocio y aclara dudas sobre los criterios de aceptación. |
| **Scrum Master (SM)** | [Nombre del Integrante 2] | Facilita el flujo de trabajo, organiza el Daily Scrum y elimina bloqueos del equipo de desarrollo. |
| **Equipo de Desarrollo (Dev Team)** | [Integrantes 3 y 4] | Diseño de wireframes/interfaz y maquetación de las historias seleccionadas para el Sprint 1. |

## 6. Plan del Sprint 1 (Sprint Planning - Clase 3)

**Meta del Sprint (Sprint Goal):** Implementar la navegación principal del catálogo de comercios y la vista detallada de los servicios ofertados (Épica 1 completa).

| Historia de Usuario | Tarea Específica de Trabajo | Responsable | Estado |
|---|---|---|---|
| Historia 1.1: Búsqueda y Filtrado | Diseñar interfaz UI/UX de la pantalla de catálogo con tarjetas de negocios y barra de búsqueda. | Dev Team / Frontend | En Progreso |
| Historia 1.1: Búsqueda y Filtrado | Crear estructura JSON / Datos ficticios con negocios de categorías (Spa, Barbería, Consultorio). | Dev Team / Backend | Completado |
| Historia 1.2: Catálogo de Servicios | Maquetar la vista de detalle de un negocio seleccionado mostrando lista de servicios con precios y duraciones. | Dev Team / Frontend | En Progreso |

### Registro de Daily Scrum de Práctica

- **¿Qué hice desde la última vez?** Levantamiento de las 12 actividades del proyecto y configuración del repositorio remoto en GitHub con el primer commit.
- **¿Qué haré hoy?** Diseñar y maquetar las vistas principales del catálogo de servicios para la Historia 1.1 e Historia 1.2.
- **¿Hay algún obstáculo?** Sin bloqueos técnicos inmediatos; ajustando coordinación de estilos CSS para los botones de agendamiento.

## 7. Matriz de Evaluación del Taller

| Elemento Evaluado | % Asignado | Descripción del Cumplimiento |
|---|---|---|
| **Conocimiento** | 20% | Diferenciación clara entre actividad puntual, historia de usuario y épica. Sustentación fluida sin lectura de IA. |
| **Desempeño - Uso de IA** | 25% | Prompt contextualizado, revisión crítica y bitácora detallada de cambios realizados por el equipo. |
| **Desempeño - Scrum y Equipo** | 25% | Roles asignados y respetados, repositorio inicializado con git commit, Daily Scrum realizado. |
| **Producto** | 30% | Documento con listado inicial, backlog priorizado, bitácora de IA, comandos Git y plan del Sprint 1. |
