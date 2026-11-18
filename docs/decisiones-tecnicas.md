# Decisiones técnicas

## Separar presentación y operaciones

Usé Next.js para la web y una API para procesar las operaciones. De esta manera, las reglas de turnos y el acceso a los datos quedan concentrados en el backend.

## Volver a comprobar la disponibilidad

Entre consultar un horario y confirmar una reserva, otra persona puede ocupar ese turno. La confirmación vuelve a validar la disponibilidad y maneja ese conflicto.

## Reconocer solicitudes repetidas

La aplicación identifica las solicitudes de reserva para manejar reintentos sin crear una segunda reserva por el mismo envío.

## Compartir contratos en el monorepo

Mantuve los contratos y las reglas comunes en paquetes compartidos. Así, los cambios de tipos e interfaces se pueden aplicar de forma coherente en el frontend y en la API.
