# Bloom · Gestión de SPA y peluquería

[← Portafolio](../README.md)

**Estado:** software utilizado en un salón real, según confirmación del fundador. La integración de Claude es un piloto local, pendiente de validación real y despliegue.

## Problema y solución

La operación de un salón combina citas, servicios, cobros, inventario, gastos y pagos a profesionales. Bloom reúne estos procesos en una aplicación web para reducir la dispersión de registros y facilitar el seguimiento diario.

| Área | Función implementada en el producto |
| --- | --- |
| Agenda | Citas, bloqueos y prevención de traslapes |
| Ingresos | Registro de servicios y distribución Bloom/profesional |
| Tienda | Inventario, ventas, abonos, devoluciones y cartera |
| Nómina | Comisiones, avances, cortes y pagos a profesionales |
| Caja y reportes | Gastos, balance y seguimiento diario y mensual |
| Administración | Usuarios, permisos y auditoría |

Stack: Next.js 14, React, TypeScript y Tailwind; FastAPI y SQLite. El código, los registros operativos y la infraestructura del negocio no forman parte de esta publicación.

## Piloto de asistente con Claude

Flujo implementado: administrador → backend autenticado → Claude → herramienta permitida → resultado limitado → respuesta. El modelo no recibe acceso directo a la base de datos ni permiso para ejecutar SQL.

Herramientas: consultar servicios y precios; consultar productos y existencias; consultar espacios disponibles. El piloto no reserva, cobra ni modifica registros. Los resultados de herramientas omiten nombres y teléfonos de clientes. La pregunta del administrador se transmite a Anthropic al activar la API; por ello, la interfaz advierte que no debe incluir datos personales.

Capturas: [escritorio](../assets/bloom-claude-desktop.png) y [móvil](../assets/bloom-claude-mobile.png). Ambas usan datos ficticios y respuestas simuladas.

Validación local: 13 pruebas automatizadas aprobadas, revisión de tipos TypeScript, ESLint e inspección visual en escritorio y móvil. Se cubrieron autenticación, permisos, denegación de herramientas, disponibilidad, privacidad de resultados, reintentos y límites por usuario. Esta evidencia no demuestra rendimiento ni precisión del modelo real.

Siguiente paso: configurar una clave privada y créditos de API, seleccionar un modelo vigente, evaluar respuestas reales y desplegar un piloto controlado. Los límites e idempotencia actuales viven en memoria de un proceso; requieren adaptación antes de escalar a varios procesos.
