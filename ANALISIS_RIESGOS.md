# Análisis de riesgos — Gestor Financiero Inteligente

## Alcance y método

Riesgos de planificación para el proyecto propuesto; no se presupone que las funciones estén implementadas. Probabilidad e impacto son valoraciones cualitativas iniciales que se revisarán al validar el stack y el MVP.

| ID | Riesgo | Probabilidad | Impacto | Prioridad |
| :--- | :--- | :---: | :---: | :---: |
| R1 | Exposición o acceso indebido a información financiera | Media | Alto | Alta |
| R2 | Ampliación excesiva del alcance y retraso | Alta | Alto | Muy alta |
| R3 | Errores en importes, saldos o cálculos | Media | Alto | Alta |
| R4 | Curva de aprendizaje del stack | Media | Alto | Alta |
| R5 | Dependencia de API, IA o alojamiento externo | Media | Medio | Media |
| R6 | Scraping bloqueado, frágil o no permitido | Alta | Medio | Alta |
| R7 | IA incorrecta o interpretada como asesoramiento | Media | Alto | Alta |
| R8 | Pérdida de cambios o conflictos | Baja | Medio | Media |
| R9 | Exposición de datos reales en pruebas | Media | Alto | Alta |
| R10 | Falta de tiempo para revisar y documentar | Media | Alto | Alta |

## Prevención, mitigación y contingencia

| ID | Prevención y mitigación | Contingencia |
| :--- | :--- | :--- |
| R1 | Permisos por usuario, validación, datos mínimos y ficticios, secretos fuera de Git. | Desactivar acceso afectado, revisar permisos y corregir antes de reactivar. |
| R2 | Definir MVP y criterios; secuenciar tareas y aplazar extras. | Reducir a movimientos, categorías, resumen y metas; documentar pendientes. |
| R3 | Reglas explícitas, importes decimales y revisión de casos, límites y fechas. | Corregir regla y recalcular resúmenes desde movimientos guardados. |
| R4 | Elegir herramientas conocidas y hacer una prueba técnica corta. | Cambiar componentes opcionales o simplificar el alcance. |
| R5 | Mantener el núcleo independiente; revisar precios, límites y condiciones. | Desactivar integración y ofrecer alternativa manual. |
| R6 | Preferir fuentes estables y revisar condiciones; no depender del scraping. | Pausar el conector y registrar datos manualmente. |
| R7 | IA limitada a explicaciones; no delegar cálculos ni decisiones; indicar límites. | Deshabilitar IA y conservar cálculos deterministas. |
| R8 | Commits pequeños y frecuentes y copia sincronizada. | Recuperar historial y reaplicar cambios revisados. |
| R9 | Datos sintéticos, secretos separados y revisión de envíos a terceros. | Eliminar datos comprometidos, rotar credenciales y revisar configuración. |
| R10 | Reservar tiempo para revisión y cerrar primero lo esencial. | Entregar MVP y registrar mejoras futuras. |

La matriz se revisará tras el análisis, la elección tecnológica y antes de la entrega. Las probabilidades son estimaciones iniciales, no estadísticas.
