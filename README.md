# Carátula

- Logo de la UPC  
- Nombre de la universidad, carrera, ciclo, código y nombre del curso, NRC  
- Nombre del profesor  
- **Título:** Informe de Trabajo Final – Anti-Hacking y Nuevas Tendencias de Seguridad  
- Nombre de la consultora  
- Relación de integrantes (código, apellidos y nombres)  
- Mes y año  

---

# Registro de Versiones del Informe

| Versión | Fecha | Cambios Realizados | Responsable |
|:--:|:--:|:--|:--|
|  |  |  |  |

---

# Project Report Collaboration Insights

## Roles Scrum
- Product Owner (líder de consultora)
- Scrum Master (coordinador de procesos)
- Development Team (pentesters, documentadores, analistas)

## Herramientas de colaboración usadas
- Trello  
- Jira  
- GitHub  
- Microsoft Teams / WhatsApp  
- Otras herramientas técnicas (Burp Suite, Metasploit, etc.)

---

# Tabla de Contenidos

- Student Outcome  
- Capítulo I: Introducción  
  - 1.1 Startup Profile (Cliente)  
  - 1.2 Consultora de Ciberseguridad (Equipo)  
  - 1.3 Solution Profile  
  - 1.4 Aceptación del Servicio de Pentesting (Rules of Engagement)  
- Capítulo II: Metodología Ágil y de Pentesting  
  - 2.1 Marco de referencia  
  - 2.2 Backlog inicial: User Stories de seguridad  
  - 2.3 Planificación de sprints (Sprint Planning)  
  - 2.4 Definición de Done (DoD)  
  - 2.5 Herramientas  
- Capítulo III: Desarrollo del Proyecto por Sprints  
  - Sprint 1 – Reconocimiento y Escaneo  
  - Sprint 2 – Enumeración y Vulnerabilidades  
  - Sprint 3 – Explotación  
  - Sprint 4 – Post-explotación y Persistencia  
  - Sprint 5 – Informe Final y Recomendaciones  
- Capítulo IV: Resultados Consolidados  
- Capítulo V: Recomendaciones y Plan de Mitigación  
- Capítulo VI: Conclusiones y Recomendaciones  
- Bibliografía  
- Anexos  

---

# Student Outcome

- Explicación de cómo el proyecto contribuye al Outcome 2 (Diseño de ingeniería con impacto en seguridad, bienestar, aspectos sociales y culturales)

---

# Capítulo I: Introducción

## 1.1 Startup Profile (Cliente)
- Descripción de la empresa PyME  
- Expectativas del cliente  

## 1.2 Consultora de Ciberseguridad (Equipo)
- Descripción de la consultora  
- Perfiles de los integrantes y roles Scrum  

## 1.3 Solution Profile
- Antecedentes y problemática  
- Objetivos del pentesting (General y específicos)  

## 1.4 Aceptación del Servicio de Pentesting (Rules of Engagement)

---

# Capítulo II: Metodología Ágil y de Pentesting

## 2.1 Marco de referencia
- Scrum aplicado a pentesting  
- PTES  
- OWASP  
- Otros marcos o normas complementarias  

## 2.2 Backlog inicial: User Stories de seguridad

Una vez redactadas todas las User Stories (US), es fundamental priorizarlas. El Product Backlog organiza las historias de usuario de acuerdo con su importancia y el valor que aportan al proyecto. Para ello, los Story Points se asignaron usando la escala de Fibonacci (1, 2, 3, 5, 8, 13). Las historias con más puntos se desarrollarán antes, al representar un mayor impacto en la seguridad del sistema.

| Orden | User Story ID | Título | Descripción (Historia de Usuario) | Story Points |
|:--:|:--:|:--|:--|:--:|
| 01 | US-02 | Pruebas de inyección SQL en APIs y formularios | Como pentester quiero ejecutar pruebas de inyección SQL sobre los endpoints críticos de TutorMatch (login, búsqueda de tutores, consultas de perfil) para identificar accesos o manipulaciones no autorizadas a la base de datos. | 13 |
| 02 | US-03 | Pruebas de Cross-Site Scripting (XSS) | Como atacante quiero insertar scripts maliciosos en el chat en tiempo real, comentarios y campos de subida para validar la sanitización de entradas en TutorMatch. | 13 |
| 03 | US-05 | Explotación de credenciales débiles & recuperación de cuenta | Como pentester quiero evaluar contraseñas débiles, políticas de bloqueo y el flujo de recuperación de cuentas (reset) para identificar takeover de cuentas en TutorMatch. | 8 |
| 04 | US-04 | Escaneo y enumeración de endpoints API | Como atacante quiero identificar todos los endpoints REST (y métodos HTTP) expuestos por TutorMatch para detectar recursos sin protección. | 8 |
| 05 | US-09 | Detección de exposición de datos sensibles | Como pentester quiero revisar respuestas de la API y endpoints públicos para detectar tokens, correos, PII o información sensible no enmascarada. | 8 |
| 06 | US-12 | Escaneo de puertos y servicios de red | Como atacante quiero mapear hosts, puertos y servicios detrás del despliegue de TutorMatch (servidor web, DB, servicios auxiliares). | 5 |
| 07 | US-06 | Prueba de subida de archivos inseguros | Como pentester quiero probar la carga de archivos (documentos, imágenes, .php renombrado) para comprobar validación y riesgo de ejecución en TutorMatch. | 5 |
| 08 | US-08 | Verificación de TLS y headers de seguridad | Como auditor quiero comprobar HTTPS/TLS y headers (CSP, HSTS, X-Frame-Options, X-XSS-Protection) para asegurar transporte y mitigación de vectores web. | 5 |
| 09 | US-13 | Auditoría de repositorios y pipelines (DevSecOps) | Como pentester quiero revisar repositorios y pipelines de CI/CD asociados a TutorMatch para detectar secretos expuestos o malas prácticas. | 3 |
| 10 | US-10 | Pruebas CSRF en acciones críticas | Como atacante quiero comprobar si formularios/state-changing endpoints en TutorMatch protegen contra CSRF. | 3 |
| 11 | US-11 | Análisis estático de aplicación móvil | Como pentester quiero analizar la app móvil (si existe) para detectar almacenamiento inseguro, claves hardcoded y llamadas inseguras a las APIs de TutorMatch. | 3 |
| 12 | US-01 | Reconocimiento inicial y mapeo de superficie | Como atacante externo quiero identificar dominios/subdominios, landing pages, rutas de login y formularios públicos de TutorMatch para mapear la superficie de ataque. | 2 |

## Criterios de aceptación generales y Definition of Done (DoD)

### Criterios generales por historia

- **Reproducible:**  
Cada hallazgo debe incluir los pasos exactos para su reproducción (request, payloads, headers y condiciones del entorno).

- **Evidencia:**  
Toda vulnerabilidad identificada debe sustentarse con capturas de pantalla, outputs de herramientas  
*(Burp, sqlmap, nmap, ZAP, Nessus)* o grabaciones breves (máx. 30 s) como PoC.

- **Impacto:**  
Se debe asignar una clasificación CVSS provisional, indicando el impacto potencial en los datos y en la funcionalidad de TutorMatch.

- **Recomendación:**  
Por cada hallazgo se debe proponer una mitigación técnica concreta  

- **Ética / Legal:**  
Si el ROE (Rules of Engagement) prohíbe la extracción de datos reales, las PoC solo deben demostrar el error o la metadata asociada,  
sin comprometer información sensible del sistema o de usuarios.

### Definition of Done (DoD) por historia

La historia está documentada y vinculada al sprint backlog correspondiente.  

Las evidencias (screenshots, outputs, colecciones Postman/Burp, reportes ZAP/Nessus) están adjuntas y debidamente nombradas.  

Cada hallazgo tiene su CVSS estimado, descripción de impacto y priorización de riesgo *(Crítico, Alto, Medio, Bajo)*.  

Se incluye una recomendación técnica priorizada con horizonte de mitigación.  

El checklist de reproducción está completado y verificado por un segundo revisor o par técnico.
  
## 2.3 Planificación de sprints (Sprint Planning)

Todas estas actividades técnicas se ejecutarán sobre el proyecto TutorMatch (entorno de staging o el host/VM autorizado por el propietario). Antes de cualquier prueba de explotación, se deberá firmar/confirmar el ROE (reglas de compromiso): entornos permitidos, cuentas de prueba, límites de extracción de datos y ventanas de ejecución.

# Sprint 1: Reconocimiento & Escaneo inicial (1 semana)

**Objetivo:**  
Identificar y documentar la superficie de ataque pública de TutorMatch: dominios, subdominios, hosts, puertos, servicios web y endpoints de autenticación. Generar inventario reproducible que guíe la enumeración.

**Actividades técnicas**
- Preparación del entorno de pruebas: configurar Kali y ambiente de trabajo, crear cuentas de prueba en TutorMatch (student/tutor) y capturar hostname, `ip a`, `uname -a` (evidencia prep).
- OSINT para TutorMatch: buscar dominios/subdominios externos y assets públicos (theHarvester, Google Dorks, Archive.org) — identificar posibles endpoints externos (landing, `api.tutormatch`, CDN, etc.).
- Descubrimiento de red y hosts: `netdiscover` / `arp-scan` (si hay red interna) y `nmap -sn` para descubrir hosts autorizados del entorno de TutorMatch.
- Escaneo inicial de puertos/servicios: `nmap -p- -T4 <target>` para identificar puertos abiertos; `nmap -sV` para versiones.
- Descubrimiento web: `gobuster`/`ffuf` para directorios y rutas públicas; `whatweb` para fingerprinting de tecnologías.
- Primera revisión TLS/headers: test rápido de TLS (`testssl.sh` o similar) y captura de cabeceras HTTP.

**Entregables**
- `prep_evidence.txt` con comandos y salidas básicas (hostname, `ifconfig`/ip, `uname -a`).
- `discovery.txt` con resultados de `netdiscover`/`nmap -sn`.
- Carpeta OSINT con outputs (theHarvester, dorks).
- Lista de URLs/endpoints descubiertos (CSV / Postman collection).
- Screenshots de las herramientas usadas y outputs principales.

**Criterio de finalización**  
Inventario reproducible de hosts y endpoints de TutorMatch; evidencias (outputs y screenshots) subidos; aprobación para pasar a enumeración.

---

# Sprint 2: Enumeración y vulnerabilidades preliminares

**Objetivo:**  
Enumerar en detalle servicios, versiones y endpoints API/WEB de TutorMatch; identificar vulnerabilidades de superficie (OWASP Top 10) en modo no destructivo y priorizar hallazgos.

**Actividades técnicas**
- Escaneo Nmap avanzado: `nmap -p- -sS -sV -O --script=vuln <target>` para identificar servicios, versiones y scripts de vulnerabilidad.
- Reconocimiento web profundo: `whatweb -v`, `gobuster dir -u <url> -w /usr/share/wordlists/dirb/common.txt` para encontrar directorios y recursos (uploads, admin, api).
- Escaneo automático de web/API: OWASP ZAP para spider + scan, generar `ZAP_report.html`.
- Detección de endpoints API: buscar swagger/openapi, endpoints JSON, y construir colección Postman/Burp.
- Pruebas preliminares no destructivas: payloads de XSS reflejado simple, pruebas básicas de SQLi con payloads manuales (no extracción), verificación de métodos HTTP permitidos (`OPTIONS`), comprobación de CORS y cabeceras.
- Revisión SCA superficial si hay acceso al repo: `npm audit`, `mvn dependency:tree` o reportes automáticos.

**Entregables**
- `nmap_full.txt`, `whatweb_<IP>.txt`, `gobuster_<IP>.txt`.
- `ZAP_report.html`.
- Colección Postman/Burp con endpoints descubiertos.
- Lista priorizada de hallazgos preliminares con CVSS estimado y PoC mínimo (errores o respuesta anómala).

**Criterio de finalización**  
Hallazgos preliminares documentados y validados (falsos positivos filtrados); backlog priorizado con historias asignadas para explotación.

---

# Sprint 3: Explotación controlada (web, APIs)

**Objetivo:**  
Explotar de forma controlada las vulnerabilidades prioritarias identificadas en Sprint 2 (por ejemplo SQLi, XSS, IDOR, credenciales), usando cuentas y datos de prueba y respetando ROE.

**Actividades técnicas**
- SQL Injection controlado: `sqlmap` en parámetros detectados con flags limitantes; si ROE prohíbe exfiltración, capturar error SQL o metadata en lugar de datos sensibles. Documentar comando exacto y outputs.
- Cross-Site Scripting: confirmar XSS (reflejado/almacenado) usando Burp Repeater y navegador; grabar PoC (GIF/short video) mostrando contexto en TutorMatch (p. ej. chat o perfil).
- Autenticación/Autorización: pruebas de fuerza bruta / credenciales comunes en cuentas de prueba (Hydra/Burp Intruder con rate-limit respetuoso), pruebas de IDOR y escalamiento horizontal/vertical en APIs (cambiar `user_id` en endpoints).
- File upload testing: subir archivos con contenido malicioso renombrado, revisar si son accesibles/ejecutables (ruta de archivos en TutorMatch).
- Uso de Burp Suite para interceptar y modificar requests a la API de TutorMatch y documentar payloads.

**Entregables**
- PoC reproducible para cada vulnerabilidad explotada (capturas, comandos, colecciones).
- Matriz de impacto con CVSS estimado y recomendaciones inmediatas (prepared/parametrized queries, validar inputs, rate-limits).
- Videos/GIFs cortos mostrando PoC (máx. 30s cada uno).

**Criterio de finalización**  
PoC reproducibles y revisados por el responsable del entorno; compromisos/soft-fixes urgentes sugeridos para mitigación.

---

# Sprint 4: Post-explotación y persistencia

**Objetivo:**  
Evaluar el impacto real tras una explotación autorizada sobre TutorMatch (limitado por ROE): comprobar escalamiento, artefactos accesibles, posibilidad de persistencia y mapeo de movimiento lateral teórico; además validar detección/monitoring.

**Actividades técnicas**
- Escalamiento de privilegios (local/DB-level) usando técnicas seguras y sólo en cuentas/entornos de prueba: intentar obtener mayor acceso mediante fallos detectados (p. ej. vulnerabilidades en consultas SQL que permitan cambiar roles).
- Revisión de dumps/backups y artefactos accesibles: localizar backups, dumps o endpoints de export (no exfiltrar datos sensibles; capturar solo metadata o hashes).
- Simulación de movimiento lateral: mapear servicios internos accesibles desde el punto de compromiso (p. ej. servicios internos que la web puede alcanzar) y documentar rutas teóricas de pivot (sin moverse fuera del entorno autorizado).
- Revisar logging y detección: comprobar si las acciones quedan registradas en logs (aplicación, webserver, DB); capturar logs locales y usar Wireshark/log capture si permiso; verificar si existen alertas/thresholds configurados.
- Documentar mitigaciones para evitar persistencia: archivos SUID, permisos, rotación de claves, configuración de WAF/IDS y reglas SIEM sugeridas.

**Entregables**
- Reporte de post-explotación que describa impacto, artefactos accesibles (metadata), y evidencia (capturas de logs, outputs).
- Recomendaciones para detección (ej.: reglas SIEM, patrones de alerta, logging format).
- Checklist de remediación inmediata (cambio de permisos, cierre de endpoints, rotación de credenciales de prueba).

**Criterio de finalización**  
Impacto clasificado (por prioridad), evidencia de las acciones realizadas (sanitizada) y un plan de reversión/mitigación listo para ser aplicado por el equipo de TutorMatch.

---

# Sprint 5: Informe final y recomendaciones

**Objetivo:**  
Consolidar todos los hallazgos en un informe técnico y ejecutivo, priorizar vulnerabilidades (CVE/CVSS), entregar evidencia organizada y proponer plan de mitigación y seguimiento.

**Actividades técnicas**
- Consolidar matriz de hallazgos: por cada hallazgo incluir servicio/endpoint, descripción, PoC, CVE (si aplica), CVSS estimado, evidencia y recomendación técnica concreta.
- Preparar informe en el template del curso (resumen ejecutivo, alcance, metodología PTES/OSSTMM, hallazgos y mitigaciones).
- Empaquetar evidencias: nmap, theHarvester, whatweb, gobuster, ZAP report, Nessus report, `discovery.txt`, `prep_evidence.txt`, PoCs y capturas en `evidence.zip`.
- Preparar presentación y video corto (si el curso lo exige) mostrando procesos clave y recomendaciones.
- Validación final de ética/legal: sanitizar PII en evidencias, comprobar ROE compliance.

**Entregables**
- Informe final (Word/PDF) listo para entrega.
- `evidence.zip` con todos los outputs y PoC (archivos nombrados y con README).
- Presentación (PPTX) y vídeo resumen (opcional según entrega).
- Hoja de ruta de remediación priorizada (short/mid/long term fixes).

**Criterio de finalización**  
Informe y paquete de evidencia entregados y verificados; checklist DoD completo (reproducibilidad, evidencias, recomendaciones priorizadas); aprobación final del Product Owner / Instructor.


## 2.4 Definición de Done (DoD)
- Evidencia clara, reproducible y con PoC  

## 2.5 Herramientas
- Kali Linux  
- Metasploit  
- Burp Suite  
- Nmap  
- sqlmap  
- Wireshark  
- Otras herramientas relevantes  

---

# Capítulo III: Desarrollo del Proyecto por Sprints

## Sprint 1 – Reconocimiento y Escaneo
- Objetivos del sprint  
- Historias de usuario atendidas  
- Actividades realizadas  
- Resultados y evidencias  
- Retrospectiva del sprint  

## Sprint 2 – Enumeración y Vulnerabilidades
- Historias de usuario atendidas  
- Actividades (Nessus, Nikto, análisis de endpoints API)  
- Resultados y evidencias  
- Retrospectiva  

## Sprint 3 – Explotación
- Historias de usuario atendidas  
- Actividades (Metasploit, Burp, sqlmap)  
- Resultados y PoC  
- Retrospectiva  

## Sprint 4 – Post-explotación y Persistencia
- Historias de usuario atendidas  
- Actividades (escalamiento, extracción de credenciales, movimiento lateral)  
- Evidencias  
- Retrospectiva  

## Sprint 5 – Informe Final y Recomendaciones
- Historias de usuario atendidas  
- Consolidación de hallazgos y plan de mitigación  
- Preparación de la presentación ejecutiva  
- Retrospectiva global  

---

# Capítulo IV: Resultados Consolidados

## 4.1 Matriz de vulnerabilidades
- ID, descripción, CVSS, impacto  

## 4.2 Evidencias técnicas
- Pantallazos, logs, outputs  

## 4.3 Impacto en el negocio

---

# Capítulo V: Recomendaciones y Plan de Mitigación

## 5.1 Recomendaciones técnicas
- Patching, WAF, hardening  

## 5.2 Recomendaciones organizacionales
- Capacitación, políticas  

## 5.3 Priorización por impacto / urgencia

---

# Capítulo VI: Conclusiones y Recomendaciones

- Conclusiones y recomendaciones del equipo  
- Lecciones aprendidas en metodología ágil  
- Relación con Student Outcome 2  
- Video “About-the-Team”  

---

# Bibliografía
- Formato APA  

---

# Anexos

- Registro de User Stories  
- Product Backlog y Sprint Backlogs  
- Evidencias de cada sprint (capturas, reportes de herramientas)  
- Scripts y código  
- Registro de retrospectivas  
