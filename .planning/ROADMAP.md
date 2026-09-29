# Hoja de ruta

## Fase 1 — Motor de turnos (Python)

**Objetivo:** una librería Python que sepa qué servicios ofrece el taller, cuánto dura cada uno y qué horarios puede ofrecer sin que Dilan quede sobrecargado.

**Requisitos:** TURN-01 a TURN-08

**Terminada cuando:**
1. Los servicios, las duraciones y el horario se cargan desde un archivo de configuración que el dueño puede leer.
2. Si se pide un servicio y un día, el motor devuelve solo horarios que se pueden cumplir.
3. No se puede reservar un turno que se superpone con otro ni fuera del horario.
4. Las reglas del dueño (anticipación, margen, trabajos de varios días) están cubiertas por tests automáticos.

## Fase 2 — API y panel del dueño

**Objetivo:** Dilan maneja su agenda desde el celular.

**Requisitos:** PANEL-01 a PANEL-04

## Fase 3 — WhatsApp

**Objetivo:** el cliente recibe confirmación, recordatorio y aviso de auto listo sin que Dilan escriba a mano.

**Requisitos:** WA-01 a WA-04

## Fase 4 — Landing page con reserva online

**Objetivo:** un cliente nuevo conoce el taller y reserva solo.

**Requisitos:** WEB-01 a WEB-03

## Fase 5 — Control de stock

**Objetivo:** Dilan sabe qué productos tiene, cuánto le cuestan y cuándo reponer.

**Requisitos:** STOCK-01 a STOCK-03

## Fase 6 — Tienda online

**Objetivo:** vender productos online con el stock real.

**Requisitos:** TIENDA-01 a TIENDA-04

## Fase 7 — Puesta en producción

**Objetivo:** el sistema funciona en internet, con dominio, backups y el número de WhatsApp del taller.
