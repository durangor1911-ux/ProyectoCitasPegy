# Sprint 3 — Backlog

**Proyecto:** CitasPeggy
**Épica:** 3. Validación y Confirmación Automática
**Duración del sprint:** [fecha inicio] – [fecha fin]
**Equipo:** Estiven Bentancur (PO), Yony Lopez (SM), Gabriela Duran (Dev), Paola Durango (Dev)

---

## Sprint Goal

Al finalizar el sprint, el sistema debe validar automáticamente la disponibilidad de horario al momento de agendar y enviar una confirmación al cliente, evitando que se generen citas duplicadas o en conflicto con otra ya existente.

---

## Historias de usuario seleccionadas

**3.1** — Como cliente, quiero recibir una confirmación automática al agendar mi cita, para tener la certeza de que quedó registrada correctamente.

Criterios de aceptación:

- Dado que el cliente completa el agendamiento, cuando confirma los datos, entonces el sistema genera un código de confirmación (bookingCode) único para la cita.
- Dado que la cita quedó confirmada, cuando se genera el código, entonces el estado de la cita cambia a "Confirmada".

**3.2** — Como negocio, quiero que el sistema valide que no haya cruce de horarios antes de confirmar una cita, para evitar dobles reservas de un mismo especialista.

Criterios de aceptación:

- Dado que un cliente intenta agendar, cuando el horario seleccionado ya está ocupado por el mismo especialista, entonces el sistema rechaza la reserva y muestra un mensaje de horario no disponible.
- Dado que el horario está libre, cuando se valida la disponibilidad, entonces la cita puede continuar al paso de confirmación.

**3.3** — Como cliente, quiero poder cancelar mi cita antes de la fecha agendada, para liberar el horario si ya no puedo asistir.

Criterios de aceptación:

- Dado que el cliente tiene una cita confirmada, cuando selecciona cancelar, entonces el estado de la cita cambia a "Cancelada" y el horario queda disponible nuevamente.
- Dado que la cita fue cancelada, cuando el negocio consulta la agenda, entonces esa franja horaria aparece libre.

---

## Tareas del sprint

| Historia | Tarea                                                                                                              | Responsable | Estado    |
| -------- | ------------------------------------------------------------------------------------------------------------------ | ----------- | --------- |
| 3.1      | Definir el formato y algoritmo de generación del bookingCode                                                       | Estiven     | Pendiente |
| 3.1      | Implementar en OrdenDelDiaServiceImpl la lógica de confirmación (estado inicial PENDIENTE → CONFIRMADA)            | Paola       | Pendiente |
| 3.1      | Mostrar en OrdenDelDiaView el código de confirmación generado                                                      | Paola       | Pendiente |
| 3.2      | Implementar validación de disponibilidad por especialista y franja horaria en el service                           | Gabriela    | Pendiente |
| 3.2      | Mostrar mensaje de error claro cuando el horario no está disponible                                                | Gabriela    | Pendiente |
| 3.2      | Revisar con el equipo los casos borde (mismo horario, especialista distinto; mismo especialista, horario distinto) | Yony        | Pendiente |
| 3.3      | Agregar el enum EstadoCita con el valor CANCELADA y el método para cambiar estado                                  | Paola       | Pendiente |
| 3.3      | Implementar la opción "Cancelar cita" en el menú de Orden del día                                                  | Gabriela    | Pendiente |
| 3.3      | Validar que al cancelar, el horario quede libre para nuevas reservas                                               | Estiven     | Pendiente |
| —        | Coordinar Daily Scrum y actualizar el Sprint Backlog                                                               | Yony        | En curso  |

---

## Definition of Done

- El código compila y corre sin errores (`main()` probado localmente).
- Las 3 historias cumplen sus criterios de aceptación.
- La validación de disponibilidad y la cancelación quedan probadas con al menos un caso de éxito y uno de error.
- Cambios subidos a GitHub (commit + push) en la rama correspondiente.
- Pull Request revisado por al menos un compañero antes de hacer merge a main.

---

## Notas

- Este sprint depende de que Negocio, Servicio, Cliente y Especialista (Sprint 1 y 2) ya estén implementados, porque Orden del día los referencia a los tres.
- La Épica 4 (Comprobantes y Recordatorios) queda para el Sprint 4, una vez la confirmación automática esté funcionando.
