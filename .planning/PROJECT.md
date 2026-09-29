# Taller de Detailing — Dilan Calchei

## Qué es

Sistema de administración para un taller de detailing en Loma Hermosa (Partido de Tres de Febrero, Buenos Aires). El taller lo lleva una sola persona, su dueño Dilan Calchei, que atiende, trabaja los autos y administra.

## Valor central

Que los clientes solo puedan reservar turnos que el taller puede cumplir, respetando la duración de cada servicio y que Dilan trabaja solo, y que la comunicación con el cliente vaya por WhatsApp sin trabajo manual.

## Alcance

| Módulo | Qué resuelve |
|---|---|
| Turnos (Python) | Catálogo de servicios con sus duraciones, horario del taller, cálculo de disponibilidad, reservas sin superposiciones |
| Panel del dueño | Agenda del día y de la semana desde el celular, confirmar, reprogramar, cancelar, bloquear días |
| WhatsApp | Confirmaciones, recordatorios, aviso de auto listo, aviso al dueño de reservas nuevas |
| Landing page | Presentación del taller, servicios, trabajos realizados, ubicación y reserva online |
| Stock | Productos, ingresos, ventas, uso interno, alertas de stock bajo |
| Tienda online | Venta de productos con stock real, pedido y pago |

## Fuera de alcance (por ahora)

- Facturación electrónica (ARCA).
- Varios empleados o sucursales.
- App móvil nativa: el panel es web y se usa desde el navegador del celular.

## Restricciones y contexto

- **Operación unipersonal:** la capacidad es de una persona. El motor de turnos tiene que modelar eso y no ofrecer horarios que Dilan no puede cumplir.
- **Lenguaje:** el backend es en Python, por pedido del cliente.
- **Mercado:** Argentina. Precios en pesos, zona horaria `America/Argentina/Buenos_Aires`, WhatsApp como canal principal y Mercado Pago como medio de pago más probable.
- **Repositorio público:** `Hcalchei/Catalogo` es público y publica con GitHub Pages. Los datos de clientes nunca se suben al repo. Queda por decidir dónde viven la información interna del negocio y el backend (ver fase 1).
- **Hosting:** GitHub Pages solo sirve archivos estáticos. La landing puede vivir acá, pero el backend Python necesita un servidor aparte (se decide en la fase 7).

## Decisiones clave

| Decisión | Motivo | Estado |
|---|---|---|
| Backend en Python con FastAPI y SQLite | Pedido del cliente. SQLite alcanza para el volumen de un taller unipersonal y simplifica backups | Propuesta |
| El motor de turnos es una librería pura, sin web ni base de datos | Se puede probar a fondo con tests y después se reusa desde la API, el panel y la landing | Propuesta |
| WhatsApp: primero enlaces `wa.me` con mensaje armado, después la API oficial de WhatsApp Business | Los enlaces no cuestan nada ni requieren configuración. La API oficial requiere verificar el negocio en Meta y aprobar plantillas | A decidir en la fase 3 |
| Landing estática en este repo | Mismo esquema que los otros sitios del repo | Propuesta |

---
*Creado: 2026-09-29*
