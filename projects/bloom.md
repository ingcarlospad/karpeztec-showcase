# Bloom · Producto desarrollado por Karpeztec, en operación

**Bloom es un producto desarrollado por Karpeztec y en operación para un cliente.** Bloom es la marca de ese negocio. Esta ficha presenta nuestro desarrollo y su evolución; no atribuye a Karpeztec la marca del cliente. Nuestra oferta propia para otros negocios es [Microapps Karpeztec](microapps.md).

[← Portafolio](../README.md)

## Recorrido animado

[Ver en la web](https://karpeztec.com/#demostraciones) · [Video MP4](https://karpeztec.com/assets/demos/bloom-demo.mp4?v=20261011-layouts2) · [GIF](https://karpeztec.com/assets/demos/bloom-demo.gif?v=20261011-layouts2)

Animación ilustrativa de 32 segundos: agenda, servicios, stock y límites del asistente. Datos ficticios y respuestas preparadas, sin ejecutar Claude. No es una grabación de la aplicación de producción; las capturas reales del piloto local se distinguen por separado en esta ficha.

**Estado:** software utilizado en un salón real, según confirmación de Carlos Padilla. La integración de Claude es un piloto local, pendiente de validación real y despliegue.

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

## Una jornada de trabajo con Bloom

El personal organiza las citas y registra los servicios realizados. Las ventas de productos y los abonos quedan en Tienda; los gastos y las comisiones se revisan junto al balance diario y mensual. Esta es una descripción de funciones del producto, no una medición de ahorro ni una demostración de resultados comerciales.

**Uso actual:** un salón real, confirmado por Carlos Padilla. No se ha publicado una cifra de ingresos, usuarios activos ni licencias pagadas. **Oferta propia:** Microapps Karpeztec, con identidad y alcance acordados para cada negocio. Se preparan Single y Enterprise; no se ofrece la marca del cliente ni se presume una licencia de su producto.

**Desarrollador:** Karpeztec, Carlos Padilla, Cali, Colombia. Operaciones desde marzo de 2025. Inscripción de Karpeztec S.A.S. en preparación; matrícula y constitución legal pendientes. [Web corporativa](https://karpeztec.com/).

## Piloto de asistente con Claude

Flujo implementado: administrador → backend autenticado → Claude → herramienta permitida → resultado limitado → respuesta. El modelo no recibe acceso directo a la base de datos ni permiso para ejecutar SQL.

Herramientas: consultar servicios y precios; consultar productos y existencias; consultar espacios disponibles. El piloto no reserva, cobra ni modifica registros. Los resultados de herramientas omiten nombres y teléfonos de clientes. La pregunta del administrador se transmite a Anthropic al activar la API; por ello, la interfaz advierte que no debe incluir datos personales.

Capturas: [escritorio](../assets/bloom-claude-desktop.png) y [móvil](../assets/bloom-claude-mobile.png). Ambas usan datos ficticios y respuestas simuladas.

Validación local: 13 pruebas automatizadas aprobadas, revisión de tipos TypeScript, ESLint e inspección visual en escritorio y móvil. Se cubrieron autenticación, permisos, denegación de herramientas, disponibilidad, privacidad de resultados, reintentos y límites por usuario. Esta evidencia no demuestra rendimiento ni precisión del modelo real.

Siguiente paso: configurar una clave privada y créditos de API, seleccionar un modelo vigente, evaluar respuestas reales y desplegar un piloto controlado. Los límites e idempotencia actuales viven en memoria de un proceso; requieren adaptación antes de escalar a varios procesos.

## Producto en operación y evolución

[Acceso a Bloom en operación](https://app.bloomsalonypeluqueria.com/login?next=%2F). Requiere una cuenta autorizada del negocio; no es una demo pública con acceso libre.

Carlos sitúa la evolución hacia gestión asistida por IA como concepto del producto y propuesta al cliente. Claude se presenta como una integración en evolución: existe piloto local de consulta con simulación; la API real y el despliegue siguen pendientes. No se afirma que Claude haya operado desde el primer día ni que el cliente haya aprobado o contratado el piloto.
