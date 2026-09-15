# Arquitectura

```text
UI (App Router + componentes)
        ↓
Lógica de negocio y validación
        ↓
Servicios y Server Actions
        ↓
Supabase (PostgreSQL, Auth, RLS y Storage)
```

La aplicación usa módulos por dominio y componentes organizados por función. Las reglas de negocio permanecen fuera de los componentes visuales. Los Server Actions forman el límite entre la aplicación y la persistencia.

La estrategia permite cambiar una pantalla sin mezclar consultas, permisos y presentación. También facilita probar los cálculos y flujos de forma aislada.

## Calidad

- TypeScript estricto y ESLint.
- Pruebas unitarias con Vitest.
- Flujos críticos y responsive con Playwright.
- Build de producción antes de cada entrega.
