# CasaPyG · Monitorización y automatización del hogar

[← Portafolio](../README.md)

## Recorrido animado

[Ver en la web](https://karpeztec.com/#demostraciones) · [Video MP4](https://karpeztec.com/assets/demos/casapyg-demo.mp4) · [GIF](https://karpeztec.com/assets/demos/casapyg-demo.gif)

Animación conceptual de 32 segundos: métricas ficticias, un evento multimedia y una propuesta de iluminación con confirmación ilustrativa. No representa telemetría real, ejecución de un modelo ni control de luces. La asistencia con IA y la actuación sobre dispositivos son objetivos de desarrollo y validación.

**Estado: prototipo.** Proyecto de automatización doméstica desarrollado en Python, con trabajo de monitorización del sistema y exploración de escenarios vinculados a reproducción multimedia.

## Enfoque

La implementación explorada incluye métricas de CPU, memoria y red, una interfaz local basada en Flask y trabajo de integración con eventos de Emby. El objetivo es relacionar señales del entorno con escenas domésticas, por ejemplo, iluminación durante reproducción multimedia.

```mermaid
flowchart LR
  M[Métricas del sistema] --> C[CasaPyG]
  E[Eventos multimedia] --> C
  C --> V[Panel de monitorización]
  C -. Objetivo de integración .-> D[Escenas y dispositivos]
```

**Esquema conceptual del prototipo.** Las conexiones a iluminación, asistentes domésticos y otros dispositivos requieren desarrollo y validación; no se anuncian como integraciones comerciales terminadas.

## Próximos hitos

- Corregir y consolidar módulos del prototipo.
- Completar los adaptadores de dispositivos y verificar compatibilidad real.
- Validar escenarios, fallos de red y recuperación antes de una instalación de uso continuo.

No se publican direcciones de red, configuraciones domésticas, credenciales ni código de implementación.
