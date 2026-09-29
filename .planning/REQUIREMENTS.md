# Requisitos

Cada requisito tiene un código para rastrearlo en la hoja de ruta. Los marcados *(a confirmar)* dependen de respuestas del dueño.

## Turnos (TURN)

- **TURN-01** Catálogo de servicios con nombre, descripción, precio y duración.
- **TURN-02** La duración y el precio pueden variar según el tamaño del vehículo *(a confirmar)*.
- **TURN-03** Horario de trabajo configurable: días, horas, cortes, feriados y días bloqueados.
- **TURN-04** Cálculo de horarios disponibles para un servicio según su duración y la agenda ocupada, sabiendo que trabaja una sola persona.
- **TURN-05** Servicios que ocupan más de una jornada: el auto queda en el taller *(a confirmar)*.
- **TURN-06** Crear, reprogramar y cancelar turnos sin superposiciones.
- **TURN-07** Reglas del dueño: anticipación mínima y máxima para reservar, margen entre trabajos, seña y política de cancelación *(a confirmar)*.
- **TURN-08** Registro de clientes y sus vehículos (marca, modelo, patente).

## Panel del dueño (PANEL)

- **PANEL-01** Agenda del día y de la semana, cómoda desde el celular.
- **PANEL-02** Confirmar, reprogramar, cancelar y marcar un turno como terminado.
- **PANEL-03** Bloquear horarios o días completos.
- **PANEL-04** Acceso protegido: solo entra el dueño.

## WhatsApp (WA)

- **WA-01** Confirmación del turno al cliente.
- **WA-02** Recordatorio antes del turno.
- **WA-03** Aviso de auto listo para retirar.
- **WA-04** Aviso al dueño cuando entra una reserva nueva.

## Landing page (WEB)

- **WEB-01** Presentación del taller: servicios, precios, fotos de trabajos, ubicación y horarios.
- **WEB-02** Reserva online que consulta la disponibilidad real.
- **WEB-03** Botón de contacto por WhatsApp.

## Stock (STOCK)

- **STOCK-01** Alta de productos: nombre, código, costo, precio de venta y stock mínimo.
- **STOCK-02** Movimientos de stock: ingreso de mercadería, venta, uso interno y ajuste.
- **STOCK-03** Alerta de stock bajo.

## Tienda online (TIENDA)

- **TIENDA-01** Catálogo online que muestra el stock real.
- **TIENDA-02** Carrito y pedido.
- **TIENDA-03** Pago con Mercado Pago o coordinación por WhatsApp *(a confirmar)*.
- **TIENDA-04** Retiro en el taller o envío *(a confirmar)*.

## Para más adelante (v2)

- Descontar insumos del stock automáticamente según los servicios realizados.
- Historial por vehículo con fotos del antes y el después.
- Reportes de facturación y de servicios más vendidos.

## Trazabilidad

| Requisitos | Fase |
|---|---|
| TURN-01 a TURN-08 | 1 |
| PANEL-01 a PANEL-04 | 2 |
| WA-01 a WA-04 | 3 |
| WEB-01 a WEB-03 | 4 |
| STOCK-01 a STOCK-03 | 5 |
| TIENDA-01 a TIENDA-04 | 6 |
