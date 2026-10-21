# Carlos + Codex · Caso Bloom y trabajo técnico

Carlos confirma que Bloom fue construido enteramente con Codex y ChatGPT mediante la extensión Roo Code, mientras él dirigía el desarrollo, probaba y corregía el producto. La fuente es su declaración para esta preparación; no se presenta como una auditoría de autoría ni un reparto porcentual entre herramientas. Roo Code se identifica como la extensión utilizada y no como un producto de OpenAI.

La aportación humana incluye definir las necesidades del negocio, revisar el comportamiento y aceptar o solicitar correcciones. No se publican cifras de tiempo ahorrado, productividad, cobertura o porcentajes de código.

## Evidencia disponible y faltante

- Bloom: producto usado en un salón según Carlos; ficha pública y capturas de un piloto con datos ficticios.
- Arquitectura: [resumen público](BLOOM-ARCHITECTURE.md), redactado a partir de documentación local sin copiar implementación.
- KarpezAI: [componente real de KarpezVoz y ocho pruebas públicas](https://github.com/ingcarlospad/karpezai-public/tree/main/examples/karpezvoz). El detector original se publica sin cambios y con hash de procedencia; los datos de entrada son sintéticos. No se atribuye su autoría histórica a Codex.
- Sesión de preparación: Codex seleccionó el componente, verificó procedencia y preparó pruebas y lanzador. Para Bloom creó una copia aislada y comprobó citas, ingresos y rechazo de solapamientos con datos ficticios.
- Pruebas del piloto de Bloom: trece pruebas existentes aprobadas en la copia, con SQLite temporal y Claude simulado; [alcance y guion de demo](BLOOM-DEMO.md).
- Demo visual: [seis capturas del recorrido real](BLOOM-DEMO.md), incluida una cita creada desde la interfaz, disponibilidad, ingresos y reporte. Solo datos ficticios; asistente IA desactivado.
- Depuración pública de esta preparación: [fallo de procedencia al publicar desde Windows y corrección con Codex](https://github.com/ingcarlospad/karpezai-public/blob/main/docs/build-notes/2026-10-21-source-bytes.md). Incluye ejecuciones fallida y aprobada y el commit que conservó los bytes originales. Es un problema de empaquetado de la muestra, no un defecto del Core ni una sesión histórica de desarrollo de Bloom.
- Pendiente: publicar una sesión sanitizada de depuración funcional del producto con prueba de regresión. No se ha realizado un video continuo narrado del recorrido.

La evidencia disponible muestra dirección de desarrollo y documentación. Los resultados históricos de depuración y pruebas requieren artefactos verificables antes de describir casos concretos. No se publican transcripciones privadas completas ni se atribuye todo KarpezAI a Codex.
