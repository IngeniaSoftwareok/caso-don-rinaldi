# Decisiones seleccionadas

## Separar presentación y datos

Next.js compone la experiencia de navegación y consume la API. La persistencia queda detrás del backend; no se conecta la interfaz pública directamente con la base.

## Revalidar disponibilidad

Un horario mostrado puede quedar ocupado antes de confirmar una reserva. La implementación revisada vuelve a comprobar la disponibilidad y contempla conflictos e identificación de solicitudes para manejar reintentos.

## Usar contratos compartidos

El monorepo conserva contratos y reglas en paquetes separados. Esto ayuda a mantener coherencia entre las aplicaciones sin duplicar las definiciones de cada lado.

## Separar implementación y uso productivo

El proyecto fue un trabajo para cliente, pero no se puso en servidor. Las capturas y el video muestran la experiencia visual construida; no acreditan reservas ni pagos reales. No se presenta el catálogo visual como un checkout comercial activo.
