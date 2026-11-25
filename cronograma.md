# Cronograma de Proyecto: Plataforma Autemia

**Institución:** Tecnológico Nacional de México · Instituto Tecnológico de Ciudad Valles  
**Proyecto:** Plataforma Autemia para *Divas Accesorios*  
**Cliente:** Miguel Ángel Velázquez (Divas Accesorios, Cd. Valles)  
**Periodo de Ejecución:** 10 de noviembre de 2026 – 22 de diciembre de 2026 (6 Semanas / 30 Días Hábiles)  
**Esfuerzo Total (PERT):** 260.6 Horas-Hombre  
**Equipo:** Jesús Eduardo García Pérez, Henry Alejandro Aguilar Torres, Jesús Rodríguez Velarde, Ángel Velázquez Orozco  

---

## 1. Ficha Técnica

| Concepto | Detalle |
| :--- | :--- |
| **Duración** | 6 semanas (30 días hábiles) |
| **Esfuerzo total (PERT)** | 260.6 horas-hombre |
| **Carga media individual** | 65.1 horas (~10.8 hrs/semana) |
| **Cliente y localización** | Miguel Ángel Velázquez (Divas Accesorios, Cd. Valles) |
| **Fecha de inicio** | 10/11/2026 |
| **Fecha estimada de término** | 22/12/2026 |

---

## 2. Cronograma de Actividades y Estructura de Desglose del Trabajo (EDT)

| EDT | Actividad / Paquete de Trabajo | Predec. | Duración | Horas PERT | Fechas | Responsable | Entregable / Criterio DoD | Ruta Crítica | Estado |
| :---: | :--- | :---: | :---: | :---: | :---: | :--- | :--- | :---: | :---: |
| **1.1** | Entrevistas de requerimientos con dueño y 6 trabajadoras | — | 2 d | 10.0 | 10/11 - 11/11 | Jesús Eduardo García Pérez | Minutas y SOW de Alcance firmado | 🟢 No | `✅ Concluida` |
| **1.2** | Inventario físico de cosméticos y codificación de tonos | 1.1 | 2 d | 8.0 | 12/11 - 13/11 | Ángel Velázquez Orozco | Catálogo base de existencias y tonos | 🟢 No | `✅ Concluida` |
| **1.3** | Especificación de arquitectura técnica y modelo conceptual | 1.2 | 2 d | 7.0 | 14/11 - 16/11 | Henry Alejandro Aguilar Torres | Documento de Arquitectura de Software | 🔴 **SÍ (CPM)** | `✅ Concluida` |
| **2.1** | Acondicionamiento de laptop-servidor y BIOS (55%) | 1.3 | 2 d | 12.0 | 17/11 - 18/11 | Jesús Rodríguez Velarde | Servidor local Ubuntu Server sin GUI | 🔴 **SÍ (CPM)** | `✅ Concluida` |
| **2.2** | Despliegue de Docker Compose y Cloudflare Tunnels | 2.1 | 2 d | 11.7 | 19/11 - 20/11 | Jesús Rodríguez Velarde | Hito 1: Túnel HTTPS seguro activo | 🔴 **SÍ (CPM)** | `✅ Concluida` |
| **2.3** | Instalación física de Mini-UPS 12V en módem ONT de fibra | 2.1 | 1 d | 8.0 | 21/11 - 21/11 | Jesús Rodríguez / Eduardo G. | Módem con respaldo eléctrico de 3 hrs | 🟢 No (3d) | `✅ Concluida` |
| **3.1** | Diseño de árbol conversacional y copys persuasivos | 1.3 | 3 d | 12.0 | 17/11 - 19/11 | Ángel Velázquez Orozco | Diagrama interactivo de menús WhatsApp | 🟢 No | `✅ Concluida` |
| **3.2** | Diseño y compresión de Catálogo Digital en PDF (< 3MB) | 3.1 | 3 d | 15.0 | 20/11 - 23/11 | Ángel Velázquez Orozco | Catálogo PDF optimizado para smartphone | 🟢 No (4d) | `✅ Concluida` |
| **3.3** | Diseño, normalización y DDL de DB PostgreSQL (3FN) | 1.3 | 3 d | 15.3 | 17/11 - 19/11 | Henry Alejandro Aguilar Torres | Esquema relacional y DDL con restricciones | 🔴 **SÍ (CPM)** | `✅ Concluida` |
| **3.4** | Configuración de Google Sheets y protección de celdas | 3.3 | 2 d | 8.0 | 20/11 - 21/11 | Henry Aguilar / Jesús R. | Hoja conectada con fórmulas =MAX protegidas | 🟢 No | `✅ Concluida` |
| **3.5** | Sincronizador batch n8n <-> Sheets / Caché SQLite | 3.4 | 2 d | 8.0 | 23/11 - 24/11 | Henry Alejandro Aguilar Torres | Worker de sincronización periódico activo | 🔴 **SÍ (CPM)** | `✅ Concluida` |
| **4.1** | Configuración de Webhooks Meta Cloud API en n8n | 2.2 | 3 d | 22.5 | 24/11 - 26/11 | Henry Alejandro Aguilar Torres | Endpoint de recepción validado por Meta | 🔴 **SÍ (CPM)** | `⏳ En curso` |
| **4.2** | Lógica de navegación de catálogo y consulta de stock | 4.1 | 3 d | 18.0 | 27/11 - 30/11 | Henry Alejandro Aguilar Torres | Hito 2: Bot respondiendo en < 2 segundos | 🔴 **SÍ (CPM)** | `📋 Pendiente` |
| **4.3** | Módulo de apartados con vigencia de 24h (#AP-XXXX) | 4.2 | 2 d | 12.0 | 01/12 - 02/12 | Henry Alejandro Aguilar Torres | Lógica de reserva y bloqueo de stock | 🔴 **SÍ (CPM)** | `📋 Pendiente` |
| **4.4** | Desarrollo de Terminal Móvil PWA (Cobro y Apartados) | 3.3 | 4 d | 23.3 | 25/11 - 28/11 | Henry Aguilar / Ángel V. | Hito 3: PWA táctil funcional en 2 toques | 🟢 No (2d) | `⏳ En curso` |
| **5.1** | Pruebas de estrés eléctrico, cortes de luz y calor | 2.3, 4.3 | 2 d | 15.7 | 03/12 - 04/12 | Jesús Rodríguez / Eduardo G. | Informe técnico de resiliencia validado | 🟢 No | `📋 Pendiente` |
| **5.2** | Pruebas de concurrencia y validación de usuario (UAT) | 4.4, 5.1 | 2 d | 20.0 | 05/12 - 07/12 | Jesús Eduardo García Pérez | Matriz de pruebas UAT aprobada por dueño | 🔴 **SÍ (CPM)** | `📋 Pendiente` |
| **5.3** | Capacitación operativa al personal (3 Fases presenciales) | 5.2 | 3 d | 25.7 | 08/12 - 10/12 | Ángel Velázquez / Eduardo G. | Hito 4: 6 trabajadoras capacitadas | 🔴 **SÍ (CPM)** | `📋 Pendiente` |
| **6.1** | Despliegue productivo final en Divas Accesorios | 5.3 | 1 d | 6.7 | 11/12 - 11/12 | Todo el Equipo Autemia | Sistema en vivo operando en mostrador | 🔴 **SÍ (CPM)** | `📋 Pendiente` |
| **6.2** | Semana de Marcha Blanca (Operación paralela 7 días) | 6.1 | 7 d | 18.0 | 12/12 - 19/12 | Todo el Equipo Autemia | Bitácora de marcha blanca sin descuadres | 🔴 **SÍ (CPM)** | `📋 Pendiente` |
| **6.3** | Estabilización final, entrega y Acta de Cierre | 6.2 | 2 d | 7.0 | 21/12 - 22/12 | Jesús Eduardo García Pérez | Hito 5: Acta de Cierre firmada por cliente | 🔴 **SÍ (CPM)** | `📋 Pendiente` |

---

## 3. Hitos Contractuales y Definición de Terminado (DoD)

| Hito | Descripción | Fecha Límite | Responsable | Criterio de Aceptación (DoD) | Estado |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **H1** | Infraestructura Base y Túnel Seguro | 20/11/2026 | Jesús Rodríguez Velarde | Servidor local activo con Docker, túnel Cloudflare HTTPS y PostgreSQL respondiendo en < 15ms. | `✅ Concluido` |
| **H2** | Bot de WhatsApp y Catálogo Interactivo | 30/11/2026 | Henry Alejandro Aguilar | Webhooks Meta conectados; bot entrega menú, PDF y consulta existencias en < 2 segundos. | `📋 Pendiente` |
| **H3** | Terminal Móvil PWA y Sincronización | 02/12/2026 | Henry Aguilar / Jesús R. | Terminal PWA descuenta stock en 2 toques táctiles y actualiza Google Sheets sin romper fórmulas. | `📋 Pendiente` |
| **H4** | Capacitación Operativa Concluida | 10/12/2026 | Ángel Velázquez / Eduardo G. | 6 trabajadoras acreditan evaluación práctica y operan con acordeón didáctico enmicado. | `📋 Pendiente` |
| **H5** | Marcha Blanca y Acta de Cierre | 22/12/2026 | Todo el Equipo Autemia | 7 días continuos en paralelo con libreta sin caídas críticas y firma formal del Acta de Cierre. | `📋 Pendiente` |

---

## 4. Distribución de Carga de Trabajo

| Integrante | Rol | Horas PERT | Horas/Semana | % Carga |
| :--- | :--- | :---: | :---: | :---: |
| **Jesús Eduardo García Pérez** | Coordinador General / QA & Enlace | 60.7 | 10.1 | 23.3% |
| **Henry Alejandro Aguilar Torres** | Arquitecto de Software (n8n & DB) | 74.8 | 12.5 | 28.7% |
| **Jesús Rodríguez Velarde** | DevOps & Ingeniero de Servidores | 63.4 | 10.6 | 24.3% |
| **Ángel Velázquez Orozco** | Diseñador UI/UX & Conversacional | 61.7 | 10.3 | 23.7% |
| **Total** | **4 integrantes** | **260.6** | — | **100.0%** |
