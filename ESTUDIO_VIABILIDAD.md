# Estudio de viabilidad técnica — Gestor Financiero Inteligente

## Objeto y viabilidad técnica

Se valora una primera versión web para registrar manualmente ingresos, gastos, metas y pagos recurrentes. El repositorio contiene documentación de planificación; no se afirma que el producto, las integraciones o el stack estén implementados.

El núcleo es abordable con tecnologías web habituales, interfaz, lógica de servidor y base relacional. La propuesta de referencia es Next.js/React/TypeScript y PostgreSQL, con ORM y autenticación por seleccionar. Debe validarse mediante una prueba técnica. Como no se ha confirmado qué tecnologías domina el estudiante, la viabilidad personal queda condicionada a elegir herramientas conocidas o reservar tiempo para aprenderlas. No conviene adoptar varias alternativas a la vez.

IA, scraping y notificaciones añaden dependencias y no son necesarios para el flujo central; se consideran extensiones.

## Recursos y logística

| Recurso | Uso | Consideración |
| :--- | :--- | :--- |
| Ordenador y navegador | Desarrollo y revisión | No se ha verificado una configuración concreta. |
| Entorno de desarrollo | Ejecutar y depurar | Se preparará al cerrar el stack. |
| Git y GitHub | Historial, respaldo y entrega | Repositorio existente; rama predeterminada main. |
| Base de datos | Persistir datos ficticios | Elegir opción compatible; inicialmente puede ser local. |
| Datos sintéticos | Pruebas y demostración | Evitan exponer información financiera real. |
| Tiempo | Análisis, desarrollo, revisión y documentación | Ajustar al calendario académico individual. |

Se avanzará del prototipo y modelo pequeño al registro y consulta completos. Cada fase tendrá un resultado verificable.

## Viabilidad económica

No hay presupuestos, tarifas ni costes comprobados en la información disponible; por ello no se asignan importes. Algunas herramientas pueden ofrecer opciones locales o gratuitas, sujetas a límites y condiciones que habrá que verificar.

Alojamiento, dominio, base de datos gestionada, correo, notificaciones o API de IA podrían generar costes. El MVP no depende de integraciones de pago ni de conexión bancaria. Antes de añadir servicios se revisarán precio, límites, tratamiento de datos y alternativa manual.

## Fases y dependencias

| Orden | Actividad | Entregable | Dependencia |
| :---: | :--- | :--- | :--- |
| 1 | Concretar requisitos, perfiles y criterios | Alcance priorizado y MVP | Ninguna |
| 2 | Validar herramientas y diseñar pantallas/datos | Prototipo y modelo | 1 |
| 3 | Preparar entorno y estructura | Proyecto ejecutable | 2 |
| 4 | Implementar persistencia y validaciones | Lógica de movimientos | 3 |
| 5 | Crear pantallas de movimientos, resumen y metas | Flujo MVP | 4 |
| 6 | Revisar acceso, cálculos y usabilidad | Incidencias resueltas o documentadas | 4 y 5 |
| 7 | Documentación y demostración | Versión presentable | 6 |
| 8 | Evaluar IA, scraping, avisos o fiscalidad | Decisión de ampliación | MVP revisado |

## MVP

- Acceso de usuario, si la prueba confirma que puede completarse con seguridad y en plazo.
- Alta, edición, consulta y clasificación manual de ingresos y gastos.
- Resumen de saldo por periodo.
- Metas de ahorro con progreso desde movimientos.
- Suscripciones y pagos recurrentes manuales.
- Validaciones e interfaz adaptable.
- Demostración con datos ficticios.

No incluye conexión bancaria, cálculo fiscal oficial, consejos concretos de inversión, notificaciones externas, scraping esencial ni IA con acceso a datos personales.

## Privacidad y mantenimiento

El desarrollo y la demostración usarán datos ficticios. Si se incorporan datos reales o terceros, se revisarán privacidad, condiciones, minimización y credenciales. Cálculos fiscales serían orientativos. El scraping requiere verificar condiciones de acceso; la IA no será autoridad para saldos, impuestos o inversiones.

## Conclusión

El proyecto es **viable de forma condicionada** si se limita al registro manual, resumen, metas y pagos periódicos; se valida un único stack y se reserva tiempo para pruebas y documentación. Depende de confirmar la experiencia disponible y el calendario.

La idea completa —perfiles avanzados, IA, scraping, avisos, fiscalidad y gestión empresarial— es demasiado amplia para garantizarla en una primera entrega. Debe tratarse como extensiones tras estabilizar el MVP.
