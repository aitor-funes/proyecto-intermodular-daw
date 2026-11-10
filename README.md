# Documentación del Proyecto Final: Gestor Financiero Inteligente

## 1. Resumen Ejecutivo

El **Gestor Financiero Inteligente** es una WebApp integral diseñada para centralizar, optimizar y automatizar el control de las finanzas personales y profesionales. A través de un asistente de Inteligencia Artificial contextual, un sistema de calendario avanzado, gestión de suscripciones y automatización mediante *Web Scraping*, la plataforma se adapta dinámicamente al perfil y a los objetivos específicos de cada usuario.

---

## 2. Sistema de Autenticación y Matriz de Roles

El inicio de sesión personaliza la experiencia de la aplicación según el perfil del usuario. La siguiente tabla resume las funciones desbloqueadas para cada tipo:

| Tipo de Usuario | Enfoque Principal | Funciones y Módulos Desbloqueados |
| :--- | :--- | :--- |
| **Trabajador por Cuenta Ajena** | Control de nóminas y ahorro personal | • Registro de ingresos fijos<br>• Metas de ahorro y huchas<br>• Control básico de gastos hormiga |
| **Autónomo (Freelance)** | Ingresos irregulares e impuestos | • Cálculo y previsión de trimestres / IVA<br>• Gestión de facturas y cobros pendientes<br>• Deducciones de gastos profesionales |
| **Empresario** | Flujo de caja y cuentas corporativas | • Múltiples cuentas y centros de coste<br>• Análisis de rentabilidad de proyectos<br>• Optimización fiscal y flujos de caja avanzados |

---

## 3. Matriz de Objetivos y Comportamiento del Bot Financiero

El usuario define un objetivo principal al registrarse. El **Bot Financiero (IA)** adapta sus consejos, alertas y cálculos según la meta elegida:

| Objetivo Seleccionado | Estrategia y Enfoque de la IA | Ejemplos de Intervención del Bot |
| :--- | :--- | :--- |
| **Ahorrar** | Maximizar el remanente mensual y crear fondos de emergencia. | *"Detecto un gasto extra del 15% en ocio; si lo reduces, alcanzarás tu hucha de vacaciones 2 semanas antes."* |
| **Invertir** | Rentabilizar el capital disponible y sugerir productos financieros. | *"Tienes 1,200€ ociosos en cuenta corriente. Considera mover el 50% a un fondo indexado de bajo riesgo."* |
| **Reducir Gastos** | Auditar suscripciones y eliminar fugas de dinero hormiga. | *"Atención: tu suscripción a la plataforma X subió un 10% este mes y no la has usado en 45 días."* |

---

## 4. Módulos Principales de la WebApp

### A. Panel de Control y Gestión Financiera
* **Sueldos e Ingresos:** Registro centralizado de entradas.
* **Gestión de Ahorros:** Visualización gráfica del progreso de metas.
* **Gestión de Suscripciones:** Auditoría en tiempo real de servicios recurrentes para evitar cargos sorpresa o duplicados.

### B. Calendario + Agenda Inteligente
* **Sistema de Notificaciones:** Alertas push y correos programados.
* **Fechas Clave:** Sincronización automática de cobros de nóminas, vencimientos de suscripciones y plazos de impuestos.
* **Anticipación:** Configuración de avisos personalizados (ej. *"Avisar 3 días antes de cobros imprevistos"*).

### C. Sistema de Web Scraping
* **Monitoreo de Mercado:** Rastreo automático de subidas de tarifas en servicios suscritos.
* **Análisis Externo:** Extracción de datos sobre rentabilidades de cuentas de ahorro e inflación para ofrecer comparativas al usuario.

---

## 5. Arquitectura Técnica Propuesta

| Capa Tecnológica | Tecnología Sugerida | Propósito Principal |
| :--- | :--- | :--- |
| **Frontend** | React.js / Next.js + Tailwind CSS | Interfaz de usuario responsiva, rápida y dinámica. |
| **Backend** | Node.js (Express) o Python (FastAPI) | Lógica de negocio, pasarelas y procesamiento de APIs. |
| **Base de Datos** | PostgreSQL / MongoDB | Almacenamiento seguro, encriptado y estructurado de datos financieros. |
| **Módulo de IA** | API de LLM (ej. OpenAI / Anthropic) + Prompt Contextual | Razonamiento financiero y asesoramiento personalizado. |
| **Web Scraping** | Python (BeautifulSoup / Selenium / Puppeteer) | Extracción automatizada de datos externos y precios. |
