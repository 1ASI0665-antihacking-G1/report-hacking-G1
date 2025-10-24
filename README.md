## Registro de Versiones

| Versión | Fecha  | Autor | Descripción |
|----------|--------|--------|--------------|
| 1.0 | 24/10/2025 | SecuraLabs | Entrega inicial del trabajo final. |

---

# Project Report Collaboration Insights

Durante el desarrollo del proyecto, el equipo **SecuraLabs** adoptó un enfoque ágil basado en **Scrum**, distribuyendo los roles de manera clara para garantizar una colaboración efectiva y trazable.

## Roles del equipo (Scrum)

| Rol Scrum | Integrante | Responsabilidades principales |
|------------|-------------|-------------------------------|
| **Product Owner** | Harold Miguel Elias Sanchez | Define el alcance del proyecto, coordina con el cliente, gestiona las prioridades del backlog y asegura que los entregables cumplan los objetivos. |
| **Scrum Master** | Fabio Maurizio Nicolich Alvis | Supervisa el cumplimiento de los sprints, facilita la comunicación entre los miembros, asegura la aplicación de las prácticas ágiles y mantiene la documentación técnica actualizada. |
| **Pentester & Analyst** | Leonardo José Aquino Cruz | Realiza tareas de reconocimiento, escaneo, explotación y análisis de vulnerabilidades, además de registrar las evidencias obtenidas. |
| **Technical Writer & Documentador** | Piero Alberto Velarde Luyo | Encargado de la redacción del informe, compilación de resultados, normalización del formato Markdown y verificación de la calidad del contenido técnico. |

---

## Herramientas de colaboración utilizadas

| Herramienta | Uso Principal |
|--------------|----------------|
| **Microsoft Word** | Redacción colaborativa inicial del informe, revisión ortográfica y consolidación de capítulos antes de la migración a GitHub. |
| **GitHub** | Control de versiones del informe final en formato Markdown (`README.md`), aplicación del flujo GitFlow, seguimiento de commits individuales y trazabilidad del proyecto. |
| **Trello** | Gestión ágil de tareas, planificación de sprints, priorización del backlog y definición de criterios de aceptación. |
| **Microsoft Teams / WhatsApp** | Coordinación de reuniones semanales, intercambio de archivos y comunicación inmediata entre los miembros. |
| **Kali Linux, Metasploit, Nmap, Burp Suite, Nessus** | Herramientas técnicas utilizadas durante las fases de reconocimiento, escaneo, explotación y análisis de vulnerabilidades. |

---

## Repositorio del informe

El informe final se desarrollará en un repositorio público bajo la organización  
`1ASI0665-antihacking-G1`, donde se documentará todo el ciclo de vida del proyecto, incluyendo commits, versiones y entregables.  

**Repositorio oficial:** `1ASI0665-antihacking-G1/report-hacking-G1`

---

## Evidencias de colaboración

Para la elaboración del informe, el equipo trabajó inicialmente en un documento compartido de Word con el fin de definir estructura, capítulos y formato uniforme.  
Posteriormente, cada integrante migró su parte al repositorio Markdown, realizando commits individuales con mensajes normalizados bajo el estándar **Conventional Commits**, reflejando la autoría y responsabilidad de cada sección.

> En la Figura 1 (a incluir en la versión final) se presentarán los analíticos de colaboración de GitHub (Insights → Contributors), evidenciando la participación equitativa de los integrantes y la evolución del proyecto durante las entregas **TP1** y **TF1**.

---

# Tabla de Contenidos

- [Student Outcome](#student-outcome)  
- [Capítulo I: Introducción](#capítulo-i-introducción)  
  - [1.1 Startup Profile (Cliente)](#11-startup-profile-cliente)  
  - [1.2 Consultora de Ciberseguridad (Equipo)](#12-consultora-de-ciberseguridad-equipo)  
  - [1.3 Solution Profile](#13-solution-profile)  
  - [1.4 Aceptación del Servicio del Pentesting (ROE)](#14-aceptación-del-servicio-del-pentesting-roe)  
- [Capítulo II: Metodología Ágil y de Pentesting](#capítulo-ii-metodología-ágil-y-de-pentesting)  
  - [2.1 Marco de referencia](#21-marco-de-referencia)  
  - [2.2 Backlog inicial: User Stories de seguridad](#22-backlog-inicial-user-stories-de-seguridad)  
  - [2.3 Planificación de Sprints](#23-planificación-de-sprints)  
- [Capítulo III: Desarrollo del Proyecto por Sprints](#capítulo-iii-desarrollo-del-proyecto-por-sprints)  
- [Capítulo IV: Resultados Consolidados](#capítulo-iv-resultados-consolidados)  
- [Capítulo V: Recomendaciones y Plan de Mitigación](#capítulo-v-recomendaciones-y-plan-de-mitigación)  
- [Capítulo VI: Conclusiones y Lecciones Aprendidas](#capítulo-vi-conclusiones-y-lecciones-aprendidas)  
- [Bibliografía (APA)](#bibliografía-apa)  
- [Anexos](#anexos)

---

# Student Outcome

**Relación con ABET – Student Outcome 2:**  
El proyecto evidencia la capacidad del equipo para **identificar, formular y resolver problemas de seguridad informática**, aplicando principios de ingeniería y metodologías ágiles en un contexto real de pentesting.

**Indicadores demostrados:**
- Diseño y ejecución de pruebas de penetración en entornos reales de cliente.  
- Aplicación del estándar **PTES** y guías **OWASP Testing Guide**.  
- Desarrollo colaborativo con herramientas profesionales (GitHub, Trello, Teams).  
- Elaboración de entregables reproducibles con trazabilidad y evidencia técnica.  

---

# Capítulo II: Metodología Ágil y de Pentesting

## 2.2 Backlog inicial: User Stories de seguridad

Una vez redactadas todas las User Stories (US), se priorizaron de acuerdo con su impacto en la seguridad del sistema.  
Los Story Points se asignaron siguiendo la escala de **Fibonacci (1, 2, 3, 5, 8, 13)**.

| Orden | ID | Título | Descripción | Story Points |
|--------|----|--------|--------------|---------------|
| 1 | US-02 | Pruebas de inyección SQL en APIs y formularios | Como pentester quiero ejecutar pruebas de inyección SQL sobre los endpoints críticos de TutorMatch para identificar accesos no autorizados. | 13 |
| 2 | US-03 | Pruebas de Cross-Site Scripting (XSS) | Como atacante quiero insertar scripts maliciosos en campos de entrada para validar la sanitización. | 13 |
| 3 | US-05 | Explotación de credenciales débiles | Evaluar contraseñas débiles y recuperación de cuenta para takeover. | 8 |
| 4 | US-04 | Escaneo y enumeración de endpoints API | Identificar endpoints REST expuestos para detectar recursos sin protección. | 8 |
| 5 | US-09 | Exposición de datos sensibles | Revisar respuestas de la API para detectar tokens o PII no enmascarados. | 8 |
| 6 | US-12 | Escaneo de puertos y servicios de red | Mapear hosts, puertos y servicios detrás del despliegue. | 5 |
| 7 | US-06 | Subida de archivos inseguros | Probar carga de archivos maliciosos y validación. | 5 |
| 8 | US-08 | Verificación de TLS y headers | Comprobar HTTPS/TLS y headers de seguridad. | 5 |
| 9 | US-13 | Auditoría de repositorios y pipelines | Revisar CI/CD para detectar secretos expuestos. | 3 |
| 10 | US-10 | Pruebas CSRF en acciones críticas | Verificar protección CSRF en endpoints sensibles. | 3 |
| 11 | US-11 | Análisis estático de aplicación móvil | Detectar almacenamiento inseguro y claves hardcoded. | 3 |
| 12 | US-01 | Reconocimiento inicial y mapeo | Identificar dominios/subdominios y formularios públicos. | 2 |

**Criterios generales de aceptación:**
- Reproducible: cada hallazgo incluye pasos exactos y condiciones.  
- Evidencia: capturas, outputs o videos cortos (≤30 s).  
- Impacto: CVSS provisional y análisis del riesgo.  
- Recomendación: mitigación técnica priorizada.  
- Ética/Legal: sin extracción de datos reales, solo PoC sanitizadas.

---

## 2.3 Planificación de Sprints

Todas las actividades técnicas se desarrollaron sobre el entorno de **TutorMatch** (staging/VM autorizada) bajo aprobación del **ROE (Rules of Engagement)**.

| Sprint | Nombre | Objetivo | Duración | Entregables principales |
|:--:|:--|:--|:--:|:--|
| 1 | Reconocimiento & Escaneo inicial | Identificar la superficie de ataque y hosts autorizados. | 1 semana | `prep_evidence.txt`, `discovery.txt`, lista de endpoints. |
| 2 | Enumeración y vulnerabilidades preliminares | Identificar vulnerabilidades OWASP Top 10 en modo no destructivo. | 1 semana | `nmap_full.txt`, `ZAP_report.html`, colección Postman. |
| 3 | Explotación controlada (web y APIs) | Explotar vulnerabilidades priorizadas con PoC y evidencia. | 1 semana | Capturas, videos, matriz CVSS, PoC reproducibles. |
| 4 | Post-explotación y persistencia | Analizar impacto, escalamiento y monitoreo. | 1 semana | Reporte de impacto, checklist de remediación. |
| 5 | Informe final y recomendaciones | Consolidar hallazgos, priorizar mitigaciones y presentar informe final. | 1 semana | Informe PDF/MD, `evidence.zip`, presentación. |

**Definition of Done (DoD):**
- Historia documentada en backlog y vinculada a sprint.  
- Evidencias y PoC adjuntas y verificadas.  
- CVSS y recomendación técnica priorizada.  
- Checklist de reproducción revisado por par técnico.

---
