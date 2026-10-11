![Karpeztec: software y automatización](assets/karpeztec.svg)

# Karpeztec · Portafolio de proyectos

Desarrollamos **Bloom, software de gestión para salones y SPA**, desde Cali, Valle del Cauca, Colombia. Fundador: **Carlos Padilla**. Karpeztec comenzó a operar en **marzo de 2025**, a partir de una idea nacida durante la universidad en 2016. Emprendimiento autofinanciado, sin inversión externa.

**Web corporativa:** [karpeztec.com](https://karpeztec.com/). **Estado registral:** inscripción como **Karpeztec S.A.S.** en preparación ante la Cámara de Comercio de Cali; la matrícula y constitución legal no están completadas. Marzo de 2025 es el inicio operativo, no una fecha de registro jurídico.

Esta presentación reúne productos, prototipos y evidencia de desarrollo. El código de los productos y los datos del negocio se mantienen privados.

| Proyecto | Propósito | Estado al 11 de octubre de 2026 |
| --- | --- | --- |
| [Bloom](projects/bloom.md) | Gestión de SPA y peluquería: agenda, ingresos, tienda y comisiones | En uso en un salón real, según su fundador. Asistente Claude en pruebas locales. |
| [Karpez IA](projects/karpez-ia.md) | Entorno para trabajar con modelos locales y adaptadores de proveedores | En desarrollo; integración comercial y validación de proveedores pendientes. |
| [CasaPyG](projects/casapyg.md) | Monitorización y automatización del hogar | Prototipo; integración y validación con dispositivos pendientes. |

## Bloom: de la gestión diaria a un asistente conectado

Bloom combina **Next.js, TypeScript, FastAPI y SQLite** para organizar las operaciones del salón. Estamos preparando una integración con Claude para consultar servicios y precios, productos y disponibilidad de agenda mediante herramientas controladas por permisos.

La integración está implementada localmente para administradores y en modo de consulta. Las pruebas utilizaron respuestas simuladas de Claude y datos ficticios. **La llamada real a la API y el despliegue del asistente siguen pendientes.**

### Captura real del piloto local · escritorio

![Asistente Bloom en un entorno local con datos ficticios y respuesta simulada](assets/bloom-claude-desktop.png)

### Captura real del piloto local · móvil

<img src="assets/bloom-claude-mobile.png" alt="Asistente Bloom en móvil, entorno de prueba con datos ficticios" width="390">

Las capturas corresponden a la interfaz implementada, no a una demostración de uso real de la API. Se verificaron permisos, restricciones de herramientas, idempotencia, límites de uso y omisión de nombres y teléfonos de clientes en resultados de herramientas; 13 pruebas automatizadas, TypeScript y ESLint aprobados.

## Demostraciones animadas

[Ver los tres recorridos en la web](https://karpeztec.com/#demostraciones). Cada video dura 32 segundos e incluye un rótulo permanente de simulación, datos ficticios y respuestas preparadas. Son interfaces ilustrativas, no grabaciones de ejecución real de los productos, de Claude o de dispositivos. Se generaron con un script propio, sin consumir créditos ni publicar código privado.

| Proyecto | Video | GIF | Recorrido |
| --- | --- | --- | --- |
| Bloom | [MP4](https://karpeztec.com/assets/demos/bloom-demo.mp4) | [GIF](https://karpeztec.com/assets/demos/bloom-demo.gif) | Agenda, catálogo, stock y límites del asistente de consulta. |
| Karpez IA | [MP4](https://karpeztec.com/assets/demos/karpez-ia-demo.mp4) | [GIF](https://karpeztec.com/assets/demos/karpez-ia-demo.gif) | Elección de modo, contexto ficticio y revisión de una acción propuesta. |
| CasaPyG | [MP4](https://karpeztec.com/assets/demos/casapyg-demo.mp4) | [GIF](https://karpeztec.com/assets/demos/casapyg-demo.gif) | Métricas de ejemplo, evento multimedia y escena conceptual con confirmación. |

## Dirección de desarrollo de los productos

- Bloom: validar un piloto con Claude antes de ampliar a atención a clientes adultos y más salones.
- Karpez IA: consolidar el entorno local y comprobar cada adaptador de proveedor.
- CasaPyG: validar escenarios de monitorización y automatización con dispositivos reales.

## Caso de uso de Bloom

1. Organizar citas, profesionales y bloqueos de horario.
2. Registrar los servicios realizados, las ventas y los movimientos de inventario.
3. Revisar ingresos, gastos y comisiones mediante caja y reportes diarios y mensuales.

El uso actual en **un salón real** fue confirmado por Carlos Padilla. Las muestras de este repositorio son de un entorno local con datos ficticios; no prueban ingresos, clientes de pago ni resultados comerciales. La validación con la API real de Claude está pendiente.

La dirección comercial propuesta contempla una oferta por negocio y, posteriormente, una oferta para varias sedes, incluidos salones pequeños y barberías. Los precios y la disponibilidad de la versión para varios negocios siguen por definir; no se presenta como una función ya desplegada.

## Contacto

**Carlos Padilla · Fundador de Karpeztec**  
[ingpadceo@karpeztec.com](mailto:ingpadceo@karpeztec.com) · [LinkedIn](https://www.linkedin.com/in/carlos-padilla-6a4a4a162/)

Para conocer Bloom, solicita una presentación por el correo empresarial. La vitrina pública muestra el producto con datos ficticios; el acceso operativo se entrega a usuarios autorizados por separado.

### English overview

Karpeztec is a self-funded software venture based in Cali, Colombia, operating since March 2025. Bloom is used in one real salon, as confirmed by its founder. Its admin-only, read-only Claude integration has been implemented locally and tested with simulated responses and fictional data; live API validation and deployment are pending. Registration as Karpeztec S.A.S. is being prepared and is not complete. Karpez IA and CasaPyG are development projects. This repository contains presentation materials, not product source code.

© 2026 Carlos Padilla / Karpeztec. Derechos reservados. Véase [aviso de uso](NOTICE.md). Esta vitrina no implica asociación, certificación ni aprobación por Anthropic o por otros proveedores.
