# Arquitectura del caso

```mermaid
flowchart LR
  W["Frontend · Next.js"] --> A["API HTTP"]
  A --> D["Reglas de negocio"]
  A --> S["Adaptador de persistencia"]
  S --> Q["SQLite / D1 según entorno"]
  C["Contratos compartidos"] -.-> W
  C -.-> A
```

El frontend no accede directamente a la base. La API aplica reglas y utiliza un adaptador de persistencia. Los contratos compartidos mantienen tipos e interfaces entre las partes.

El monorepo permite desplegar frontend y API por separado. Esta posibilidad técnica no significa que el proyecto se haya publicado: el desarrollo para cliente quedó sin puesta en producción.
