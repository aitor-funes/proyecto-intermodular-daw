# Gestor Financiero Inteligente

## Resumen y alcance

El **Gestor Financiero Inteligente** es una aplicación web propuesta para centralizar el control de las finanzas personales y profesionales. Pretende ayudar a registrar ingresos y gastos, consultar la evolución del presupuesto, organizar metas de ahorro y recordar pagos y vencimientos. Contempla perfiles de trabajador por cuenta ajena, autónomo y empresario, además de posibles ampliaciones con IA, notificaciones y consulta automatizada de información pública.

> **Estado:** este repositorio contiene documentación de planificación. Las tecnologías y funcionalidades descritas son propuestas; no se afirma que estén implementadas.

### Perfiles considerados

| Perfil | Necesidades |
| :--- | :--- |
| Trabajador por cuenta ajena | Ingresos regulares, control de gastos y metas de ahorro. |
| Autónomo | Ingresos variables, facturas y gastos profesionales; estimaciones orientativas. |
| Empresario | Varias cuentas o categorías, flujo de caja y resultados por proyecto. |

El alcance contempla movimientos manuales, panel de resúmenes, ahorro, pagos recurrentes y calendario. IA, avisos y fuentes externas son ampliaciones. Recomendaciones concretas de inversión y cálculos fiscales oficiales quedan fuera del MVP.

## Justificación técnica y arquitectura propuesta

Se plantea una aplicación web adaptable con interfaz, lógica de negocio y base de datos relacional. La opción de referencia se validará antes de programar; no representa una implementación existente.

| Capa | Propuesta pendiente de validar | Justificación |
| :--- | :--- | :--- |
| Interfaz y servidor | Next.js con React y TypeScript | Pantallas y endpoints en un proyecto; tipado. |
| Estilos | Tailwind CSS o CSS convencional | Interfaz adaptable, según conocimientos y necesidades. |
| Persistencia | PostgreSQL | Relaciones entre usuarios, movimientos, categorías, metas y vencimientos. |
| Acceso a datos | Prisma, opcional | Facilita el modelado y las consultas si encaja con el alcance. |
| Autenticación | Auth.js u otra solución compatible | Proteger los datos y gestionar sesiones. |
| Gráficos | Biblioteca React por seleccionar | Representar resúmenes definidos. |
| IA y scraping | Opcionales, fuera del núcleo | Añaden dependencias, privacidad y mantenimiento. |
| Control de versiones | Git y GitHub | Historial, respaldo y coordinación de cambios. |

No se propone conexión bancaria en el MVP; los datos se introducirían manualmente. La elección final dependerá de una prueba técnica, competencias disponibles y requisitos de despliegue.

## Fases y dependencias

| Fase | Actividades y resultado | Depende de |
| :--- | :--- | :--- |
| 1. Análisis | Requisitos, perfiles, casos de uso y criterios de aceptación. | Ninguna |
| 2. Validación y diseño | Confirmar stack, prototipo, entidades y privacidad. | 1 |
| 3. Preparación | Repositorio, entorno local, base de datos de desarrollo. | 2 |
| 4. Datos y lógica | Usuarios, movimientos, categorías, metas y validaciones. | 3 |
| 5. Interfaz MVP | Registro manual, panel, filtros, ahorro y pagos periódicos. | 3 y 4 |
| 6. Revisión | Permisos, cálculos, errores y escenarios funcionales. | 4 y 5 |
| 7. Documentación | Guía, limitaciones y material de demostración. | 6 |
| 8. Ampliaciones | Calendario avanzado, avisos, IA o fuentes externas. | MVP estable |

Si el tiempo es limitado, se priorizarán movimientos manuales y resumen financiero, aplazando integraciones.

## MVP propuesto

Acceso de usuario si la prueba técnica lo confirma; alta, edición, consulta y clasificación manual de ingresos/gastos; saldo por periodo; metas de ahorro; pagos recurrentes manuales; validaciones básicas e interfaz adaptable.

Fuera del MVP: conexión bancaria, importación automática, fiscalidad oficial, recomendaciones concretas de inversión, scraping esencial, notificaciones externas e IA con datos personales. Las extensiones se estudiarán una vez estable el núcleo.

## Recursos, logística y seguridad

Se prevén ordenador, navegador, entorno de desarrollo compatible, Git/GitHub, herramientas de diseño y documentación, y base de datos de desarrollo. Se usarán datos ficticios. El tiempo se distribuirá entre análisis, implementación, revisión y documentación.

No se fija presupuesto ni se afirman costes comprobados. Alojamiento, dominio, base de datos gestionada o API de IA pueden generar costes según proveedor y uso; se comprobarán antes de contratar.

El diseño deberá contemplar autenticación, autorización por usuario, validación, gestión segura de secretos y copias de seguridad según el entorno. Los cálculos serán explícitos y verificables. La IA, si se incorpora, no será la fuente de verdad para importes ni impuestos. Se revisarán privacidad y condiciones de terceros antes de usar datos reales.

## Documentos relacionados

- [Análisis de riesgos](ANALISIS_RIESGOS.md)
- [Estudio de viabilidad](ESTUDIO_VIABILIDAD.md)
