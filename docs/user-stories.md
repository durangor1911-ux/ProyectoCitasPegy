# User Stories — CitasPeggy

## Épica 1: Catálogo y Selección de Servicios

### Historia 1.1: Búsqueda y Filtrado de Negocios

**Como** cliente de la plataforma
**Quiero** ver y filtrar la lista de negocios registrados por categoría (restaurantes, consultorios, spas, barberías)
**Para** encontrar y elegir fácilmente el establecimiento donde deseo agendar mi cita

**Criterios de aceptación:**

- Barra de búsqueda funcional por nombre y selector por categoría
- Tarjetas con nombre, dirección, imagen y puntuación

### Historia 1.2: Consulta del Catálogo de Servicios

**Como** cliente
**Quiero** ver la lista detallada de servicios que ofrece un negocio específico
**Para** conocer precios, duración estimada y detalles antes de reservar

**Criterios de aceptación:**

- Listado completo de servicios con nombre, precio y tiempo de duración
- Botón directo "Agendar"

### Historia 1.3: Ver detalle de un servicio

**Como** cliente
**Quiero** ver el detalle completo de un servicio antes de elegirlo
**Para** confirmar que es lo que necesito

**Criterios de aceptación:**

- Se muestra una descripción del servicio
- Se muestra la duración aproximada
- Se muestra qué especialistas ofrecen ese servicio

### Historia 1.4: Registrar y administrar servicios

**Como** dueño de negocio
**Quiero** agregar, editar o eliminar los servicios que ofrezco
**Para** mantener mi catálogo actualizado

**Criterios de aceptación:**

- Puedo crear un nuevo servicio con nombre, descripción, duración y precio
- Puedo editar los datos de un servicio existente
- Puedo desactivar un servicio sin perder el historial de citas pasadas

---

## Épica 2: Agendamiento y Disponibilidad en Tiempo Real

### Historia 2.1: Selección de Especialista y Horario Libre

**Como** cliente
**Quiero** ver los especialistas disponibles y sus franjas horarias libres según el servicio seleccionado
**Para** elegir al profesional de mi preferencia y la hora que mejor se acomode a mi tiempo

**Criterios de aceptación:**

- Permitir opción "Cualquier especialista disponible"
- Deshabilitar automáticamente las horas pasadas u ocupadas

### Historia 2.2: Seleccionar fecha y hora

**Como** cliente
**Quiero** seleccionar una fecha y hora específica
**Para** reservar mi cita en el momento que necesito

**Criterios de aceptación:**

- El horario queda temporalmente reservado mientras se completa el proceso
- Si no se confirma en 5 minutos, el horario se libera automáticamente
- Se muestra un resumen antes de confirmar (servicio, especialista, fecha, hora)

### Historia 2.3: Cancelar o reprogramar una cita

**Como** cliente
**Quiero** cancelar o cambiar la fecha/hora de mi cita ya agendada
**Para** ajustar mis planes si algo cambia

**Criterios de aceptación:**

- Puedo cancelar hasta 2 horas antes de la cita
- Al cancelar, el horario se libera automáticamente para otros clientes

---

## Épica 3: Validación y Confirmación Automática

### Historia 3.1: Bloqueo Temporal Anti-Colisión

**Como** cliente
**Quiero** que el sistema valide y bloquee mi horario seleccionado durante el proceso de reserva
**Para** evitar que otro usuario reserve la misma casilla simultáneamente

**Criterios de aceptación:**

- Bloqueo de la casilla por 5 minutos durante la sesión
- Re-validación final en base de datos al dar clic en "Confirmar"

### Historia 3.2: Confirmación automática al cliente y al negocio

**Como** cliente
**Quiero** recibir una confirmación inmediata al agendar mi cita
**Para** tener la certeza de que mi reserva fue exitosa

**Criterios de aceptación:**

- Mensaje de éxito en pantalla con los detalles de la cita
- El negocio recibe notificación inmediata de la nueva cita

---

## Épica 4: Comprobantes y Recordatorios

### Historia 4.1: Emisión de Comprobante Digital

**Como** cliente
**Quiero** recibir un comprobante digital de mi reserva (vía correo / WhatsApp)
**Para** conservar la información de respaldo con la fecha, hora y código de reserva

**Criterios de aceptación:**

- El comprobante se envía automáticamente al confirmar la cita
- Incluye fecha, hora, servicio, especialista y código de reserva

### Historia 4.2: Recordatorios Automáticos

**Como** cliente
**Quiero** recibir alertas de recordatorio previas a mi cita (24h y 2h antes)
**Para** planificar mi asistencia o reprogramar a tiempo

**Criterios de aceptación:**

- Se envía un recordatorio 24 horas antes de la cita
- Se envía un segundo recordatorio 2 horas antes de la cita

---

## Épica 5: Métricas y Reducción de Inasistencias

### Historia 5.1: Panel de Control de Inasistencias (Rol Administrador)

**Como** administrador del negocio
**Quiero** consultar un panel analítico con métricas de asistencia e inasistencias (no-shows)
**Para** tomar decisiones operativas y políticas que aseguren la ocupación del establecimiento

**Criterios de aceptación:**

- Muestra número y porcentaje de inasistencias en el período seleccionado
- Se puede filtrar por rango de fechas

### Historia 5.2: Registrar el estado final de una cita

**Como** negocio / especialista
**Quiero** marcar una cita como Atendida, No asistió o Cancelada
**Para** que las métricas reflejen la realidad de lo ocurrido

**Criterios de aceptación:**

- El sistema permite actualizar el estado después de la hora de la cita
- Si no se actualiza en cierto tiempo, se marca automáticamente como "No asistió"
