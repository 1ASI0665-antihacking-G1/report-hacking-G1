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

| **Versión** | **Fecha** | **Cambios Realizados** | **Responsable** |
|:--:|:--:|:--|:--|
| **1.0** | **2025-10-24** | **Entrega TP1 (Semana 9):** Documento de Alcance y primer paquete de entregables. Se completaron:<br><br>**Student Outcome:** Borrador sobre contribución al Outcome 2.<br><br>**Capítulo I:** (1.1) *Startup Profile* — descripción de la PyME y expectativas del cliente. (1.2) *Consultora* — descripción y perfiles/roles SCRUM. (1.3) *Solution Profile* — antecedentes, problemática y objetivos del pentesting. (1.4) *ROE* — alcance y condiciones iniciales.<br><br>**Capítulo II:** (2.1) Marco de referencia (Scrum, PTES, OWASP). (2.2) Backlog inicial (User Stories priorizadas). (2.3) Planificación de sprints (detalle Sprint 1).<br><br>**Capítulo III (Sprint 1):** Objetivo, actividades técnicas (configuración Kali, OSINT, nmap, gobuster, TLS checks) y entregables técnicos (*prep_evidence.txt*, *discovery.txt*, carpeta OSINT, lista de endpoints, screenshots) con PoC inicial.<br><br>**Capítulo IV:** Matriz de vulnerabilidades (entradas preliminares) y evidencias adjuntas. Incluye checklist DoD parcial y evidencia subida al repositorio. | **SecuraLabs** — Harold Miguel Elías Sánchez *(Product Owner)*; Fabio Maurizio Nicolich Alvis *(Scrum Master)*; Leonardo José Aquino Cruz *(Pentester & Analyst)*; Piero Alberto Velarde Luyo *(Technical Writer)* |

---

# Project Report Collaboration Insights

## Roles Scrum
- **Product Owner (líder de consultora):**  
  **Harold Miguel Elías Sánchez**  
  Responsable de definir el alcance del servicio de pentesting, gestionar la comunicación con el cliente (TutorMatch), priorizar el Product Backlog y validar los entregables de cada sprint. Supervisa la aplicación de las reglas del **ROE (Rules of Engagement)** y asegura que las pruebas se desarrollen bajo lineamientos éticos y legales.

- **Scrum Master (coordinador de procesos):**  
  **Fabio Maurizio Nicolich Alvis**  
  Encargado de coordinar las reuniones de planificación y retrospectiva, facilitar la comunicación entre los miembros del equipo, garantizar la correcta aplicación del marco **Scrum** y el cumplimiento del **Definition of Done (DoD)**. También vela por la trazabilidad y organización del repositorio (GitHub, Trello).

- **Development Team (pentesters, documentadores, analistas):**  
  **Leonardo José Aquino Cruz** – Pentester y analista técnico, responsable de la ejecución de pruebas de reconocimiento, escaneo, explotación controlada y recolección de evidencias.  
  **Piero Alberto Velarde Luyo** – Documentador y analista, encargado de registrar hallazgos, elaborar el informe técnico y consolidar las recomendaciones de seguridad.  
  El equipo colabora en la planificación de sprints, priorización de User Stories y documentación de vulnerabilidades conforme al estándar **PTES/OWASP**.

## Herramientas de colaboración usadas
- Trello  
- Jira  
- GitHub  
- Microsoft Teams / WhatsApp  
- Otras herramientas técnicas (Burp Suite, Metasploit, etc.)

---

# Tabla de Contenidos

- [Student Outcome](#student-outcome)  
- [Capítulo I: Introducción](#capítulo-i-introducción)  
  - [1.1 Startup Profile (Cliente)](#11-startup-profile-cliente)  
  - [1.2 Consultora de Ciberseguridad (Equipo)](#12-consultora-de-ciberseguridad-equipo)  
  - [1.3 Solution Profile](#13-solution-profile)  
  - [1.4 Aceptación del Servicio de Pentesting (Rules of Engagement)](#14-aceptación-del-servicio-de-pentesting-rules-of-engagement)  
- [Capítulo II: Metodología Ágil y de Pentesting](#capítulo-ii-metodología-ágil-y-de-pentesting)  
  - [2.1 Marco de referencia](#21-marco-de-referencia)  
  - [2.2 Backlog inicial: User Stories de seguridad](#22-backlog-inicial-user-stories-de-seguridad)  
  - [2.3 Planificación de sprints (Sprint Planning)](#23-planificación-de-sprints-sprint-planning)  
  - [2.4 Definición de Done (DoD)](#24-definición-de-done-dod)  
  - [2.5 Herramientas](#25-herramientas)  
- [Capítulo III: Desarrollo del Proyecto por Sprints](#capítulo-iii-desarrollo-del-proyecto-por-sprints)  
  - [Sprint 1 – Reconocimiento y Escaneo](#sprint-1--reconocimiento--escaneo-inicial-1-semana)  
  - [Sprint 2 – Enumeración y Vulnerabilidades](#sprint-2--enumeración-y-vulnerabilidades-preliminares)  
  - [Sprint 3 – Explotación](#sprint-3--explotación-controlada-web-apis)  
  - [Sprint 4 – Post-explotación y Persistencia](#sprint-4--post-explotación-y-persistencia)  
  - [Sprint 5 – Informe Final y Recomendaciones](#sprint-5--informe-final-y-recomendaciones)  
- [Capítulo IV: Resultados Consolidados](#capítulo-iv-resultados-consolidados)  
- [Capítulo V: Recomendaciones y Plan de Mitigación](#capítulo-v-recomendaciones-y-plan-de-mitigación)  
- [Capítulo VI: Conclusiones y Recomendaciones](#capítulo-vi-conclusiones-y-recomendaciones)  
- [Bibliografía](#bibliografía)  
- [Anexos](#anexos) 

---

# Student Outcome

- Explicación de cómo el proyecto contribuye al Outcome 2 (Diseño de ingeniería con impacto en seguridad, bienestar, aspectos sociales y culturales)

---

# Capítulo I: Introducción

## 1.1 Startup Profile (Cliente)
### Descripción de la PyME 

SkillSwap Inc. es una startup tecnológica conformada por un equipo estudiantes de la carrera de Ingeniería de Software de la Universidad Peruana de Ciencias Aplicadas (UPC). Su principal iniciativa es TutorMatch, una plataforma digital orientada a mejorar el acceso y la gestión de tutorías académicas dentro del entorno universitario. El objetivo de la solución es facilitar la conexión entre estudiantes que buscan apoyo académico y tutores calificados, promoviendo una experiencia de aprendizaje colaborativa y flexible. </br>
La empresa se enmarca en el sector EdTech, un rubro que integra tecnologías digitales con metodologías educativas innovadoras, contribuyendo a la transformación digital del ámbito académico. TutorMatch representa el principal activo digital de la organización y constituye el eje central de su modelo de negocio.

**Servicios digitales ofrecidos**

La solución TutorMatch está compuesta por un ecosistema tecnológico distribuido en tres capas principales:
- **Frontend Web:** Portal de acceso principal desarrollado para navegadores, desde el cual los estudiantes pueden registrarse, buscar tutores, agendar sesiones, chatear en tiempo real y acceder a recursos académicos compartidos.
- **Backend:** API central que gestiona la autenticación de usuarios, el manejo de perfiles, el registro de tutorías, la comunicación en tiempo real y la administración de la base de datos.
- **Aplicación Móvil:** Complemento multiplataforma que ofrece las mismas funcionalidades del portal web, con un enfoque en la usabilidad y la accesibilidad desde dispositivos móviles.

Estas plataformas integran funcionalidades como videollamadas, chat en tiempo real, transferencia de archivos y gestión de disponibilidad y horarios, lo que permite una experiencia académica fluida y personalizada.

**Misión y visión**
- **Misión:** Facilitar la conexión entre estudiantes y tutores universitarios, optimizando la experiencia de aprendizaje mediante el uso de tecnologías colaborativas que permitan acceder a apoyo académico en tiempo real, de manera flexible y efectiva.
- **Visión:** Convertirse en la principal plataforma universitaria de tutorías académicas en un plazo de cinco años, promoviendo una educación más accesible, personalizada y eficiente mediante el uso de herramientas digitales innovadoras que fortalezcan el rendimiento académico y la autonomía del estudiante.

**Mercado objetivo**

El mercado objetivo de TutorMatch está compuesto principalmente por estudiantes universitarios de la carrera de Ingeniería de Software de la UPC, con proyección de expandirse a otras carreras y universidades del país. La plataforma busca posicionarse como un punto de encuentro confiable y ágil entre tutores y alumnos dentro del entorno académico digital.

### Expectativas del cliente  

Las expectativas del cliente se centran en obtener una evaluación de seguridad práctica y accionable que permita identificar y priorizar riesgos reales para TutorMatch. Específicamente, el cliente espera que el ejercicio de pentesting detecte vulnerabilidades críticas y de alto impacto (riesgo de takeover de cuentas, exposición de datos sensibles, ejecución remota o acceso no autorizado a la base de datos), que se entregue un informe técnico detallado con hallazgos reproducibles y evidencia (pruebas, logs, capturas) y que se proponga un plan de remediación con mitigaciones concretas, estimación de esfuerzo y prioridades para corregir los problemas detectados. Además, el cliente valora recibir un resumen ejecutivo comprensible para áreas no técnicas y recomendaciones para mejorar prácticas de desarrollo seguro (DevSecOps) y políticas operativas.

## 1.2 Consultora de Ciberseguridad (Equipo)
### Descripción de la consultora  

SecuraLabs es una consultora académica de ciberseguridad conformada por estudiantes de la carrera de Ingeniería de Software de la Universidad Peruana de Ciencias Aplicadas (UPC). El equipo se especializa en la aplicación de metodologías de seguridad ofensiva, evaluación de vulnerabilidades y pruebas de penetración (pentesting) orientadas a entornos web, móviles y de infraestructura en red.
El enfoque de SecuraLabs se centra en la identificación proactiva de amenazas y evaluación del riesgo tecnológico dentro de organizaciones que buscan fortalecer su postura de seguridad digital. El equipo combina conocimientos técnicos adquiridos en el ámbito académico con buenas prácticas reconocidas, como el uso de estándares OWASP, NIST SP 800-115 y MITRE ATT&CK, aplicados a contextos reales de desarrollo y despliegue de software.

**Misión**

Nuestra misión es ayudar a las organizaciones a descubrir y mitigar vulnerabilidades antes de que puedan ser explotadas, mediante la ejecución de pruebas controladas y éticas que simulan ataques reales. Buscamos fomentar una cultura de seguridad preventiva y aprendizaje continuo, aportando soluciones prácticas y estrategias de mejora que fortalezcan los sistemas y procesos de nuestros clientes frente a las nuevas tendencias de ciberamenazas.


### Perfiles de los integrantes y roles Scrum  

| Perfil | Descripción |
|--------|-------------|
|--------| **Harold Elías – Product Owner**</br>Estudiante de Ingeniería de Software en octavo ciclo, con interés en las áreas de ciberseguridad y pentesting. Posee experiencia en los lenguajes C++ y Python a nivel intermedio, además de haber participado en proyectos de desarrollo web y en la implementación de pruebas unitarias utilizando C# con NUnit.</br> Como Product Owner en SecuraLabs, Harold se encarga de definir y priorizar el backlog de seguridad, alineando las necesidades del cliente con los objetivos técnicos del equipo. Su capacidad de análisis y trabajo colaborativo facilita la toma de decisiones orientadas a maximizar el valor de las pruebas de ciberseguridad, asegurando que los entregables respondan a las expectativas del cliente.|
|--------|**Fabio Nicolich – Scrum Master**</br>Estudiante de Ingeniería de Software en séptimo ciclo, destacado por su liderazgo, responsabilidad y proactividad en la gestión de equipos. Cuenta con conocimientos en C++, HTML, CSS, JavaScript y Python, además de interés en el uso de frameworks modernos para el desarrollo de aplicaciones web.</br> Como Scrum Master, Fabio promueve la comunicación efectiva, la coordinación del equipo y la aplicación de los valores ágiles, garantizando el cumplimiento de los objetivos en cada sprint. Su compromiso con la calidad y la mejora continua contribuye a mantener un entorno colaborativo, motivando al equipo hacia resultados consistentes y orientados al aprendizaje conjunto.|
|--------|**Leonardo Aquino – Pentester & Security Analyst**</br>Estudiante de Ingeniería de Software en décimo ciclo, con experiencia en desarrollo web, ciberseguridad y diseño de videojuegos utilizando Godot y Unity. Domina lenguajes como C++, Python y JavaScript, y posee una fuerte orientación hacia la creación de soluciones seguras y la prevención de vulnerabilidades.</br> Como Pentester & Security Analyst en SecuraLabs, Leonardo lidera la ejecución de las pruebas ofensivas y el análisis técnico de vulnerabilidades, participando en la identificación, validación y documentación de hallazgos. Su capacidad analítica y su enfoque en resultados fortalecen la calidad técnica del proceso de evaluación de seguridad.|
|--------|**Piero Velarde – Technical Writer & Documentador**</br>Estudiante de Ingeniería de Software en séptimo ciclo, con interés en tecnologías emergentes, programación y ciberseguridad. Maneja los lenguajes C++, Python, JavaScript y Dart, y mantiene una actitud proactiva hacia el aprendizaje continuo y la investigación tecnológica.</br> Dentro de SecuraLabs, Piero desempeña el rol de Technical Writer & Documentador, siendo responsable de la redacción técnica, estructuración del informe y sistematización de evidencias. Además, asegura la coherencia comunicativa entre las fases técnicas y los entregables finales, contribuyendo a la claridad, precisión y formalidad de los documentos presentados al cliente.|


## 1.3 Solution Profile
### Antecedentes y problemática  

Las startups de tecnología educativa, como TutorMatch, están altamente expuestas a riesgos de seguridad informática debido al manejo de grandes volúmenes de datos sensibles (credenciales, historiales académicos, etc.) a través de plataformas, webs y aplicaciones móviles. TutorMatch, en su fase de desarrollo, es un objetivo atractivo para ciberatacantes que buscan explotar vulnerabilidades en sistemas emergentes. El análisis preliminar de su entorno ha revelado múltiples deficiencias de seguridad que amplían su superficie de ataque, incluyendo la carencia de controles robustos de autenticación y gestión de sesiones, la potencial exposición de APIs, validación insuficiente de entradas de usuario (formularios, chat) y archivos subidos. Adicionalmente, se detectaron fallos en la configuración de seguridad (TLS, encabezados HTTP) y en la gestión de credenciales, lo que justifica de manera urgente la realización de una auditoría de seguridad ofensiva.

Ante el contexto de ataques recientes en plataformas educativas similares, que han resultado en filtraciones masivas por la explotación de vulnerabilidades como inyecciones SQL o XSS, SkillSwap Inc. reconoce la necesidad crítica de actuar proactivamente. El objetivo principal es llevar a cabo una evaluación integral de ciberseguridad para TutorMatch. Esto permitirá identificar las brechas de seguridad más críticas, fortalecer la protección de los activos digitales de la plataforma y establecer un plan de mejora continua que siga las mejores prácticas de seguridad ofensiva.

### Objetivos del pentesting (General y específicos)  

**Objetivo general**

Realizar una evaluación integral de seguridad ofensiva (pentesting) sobre las plataformas web, backend y aplicación móvil de TutorMatch, con el fin de identificar vulnerabilidades técnicas, riesgos de exposición de datos y configuraciones inseguras, proporcionando un informe técnico y un plan de remediación que permitan fortalecer la postura de seguridad y la resiliencia del sistema ante potenciales ataques.

**Objetivos específicos**
1.	Identificar vulnerabilidades críticas en los componentes principales de TutorMatch (frontend, APIs, backend y app móvil) mediante la ejecución de pruebas de inyección, validación de entradas y análisis de permisos.

2.	Evaluar la robustez de los mecanismos de autenticación, gestión de sesiones y recuperación de cuentas, comprobando la resistencia del sistema frente a ataques de fuerza bruta y suplantación de identidad.

3.	Detectar exposición de información sensible (tokens, correos, datos personales o claves embebidas) en las respuestas del sistema, repositorios de código y pipelines de integración continua.

4.	Analizar la configuración de seguridad de la infraestructura y servicios asociados, incluyendo protocolos de cifrado (TLS/HTTPS), encabezados de seguridad HTTP y políticas de acceso a servidores y bases de datos.

5.	Ejecutar pruebas de explotación controlada (Proof of Concept) sobre las vulnerabilidades encontradas, validando su impacto y nivel de riesgo de acuerdo con metodologías OWASP y CVSS.

6.	Elaborar un informe técnico detallado y un plan de remediación, priorizando las acciones correctivas y recomendaciones para mitigar riesgos y fortalecer la seguridad del ciclo de desarrollo (DevSecOps).


## 1.4 Aceptación del Servicio de Pentesting (Rules of Engagement)

---

# Capítulo II: Metodología Ágil y de Pentesting

## 2.1 Marco de referencia

El presente proyecto adopta un enfoque ágil basado en **Scrum**, adaptado al contexto del **pentesting corporativo**. Esta integración permite gestionar de forma iterativa y controlada las actividades técnicas, priorizando la entrega continua de valor en cada sprint y la mejora constante del producto.  
El marco Scrum, tradicionalmente orientado al desarrollo de software, se ajusta aquí para guiar los ciclos de **planificación, ejecución, validación y documentación** de las pruebas de penetración. El equipo se organiza en roles específicos:  
- **Product Owner (PO)**: responsable de definir el alcance, objetivos y criterios de aceptación del pentest.  
- **Scrum Master**: vela por el cumplimiento del marco Scrum, la gestión de impedimentos y la comunicación efectiva del equipo.  
- **Equipo de Pentesters**: encargados de ejecutar las tareas técnicas, documentar hallazgos y proponer medidas de mitigación.  

Cada sprint de pentesting está alineado con las fases de los estándares reconocidos en la industria, especialmente **PTES (Penetration Testing Execution Standard)** y **OWASP Testing Guide (v5)**. Estas metodologías proporcionan la estructura técnica sobre la cual Scrum define su dinámica de trabajo. La correspondencia se resume así:

| Fase PTES | Fase OWASP | Sprint Scrum asociado | Objetivo principal |
|------------|-------------|-----------------------|--------------------|
| Pre-engagement Interactions | Information Gathering | Sprint 1: Reconocimiento y Escaneo inicial | Identificar el alcance, activos y vectores de ataque |
| Intelligence Gathering | Threat Modeling | Sprint 2: Enumeración y vulnerabilidades preliminares | Descubrir servicios, endpoints y posibles vulnerabilidades |
| Vulnerability Analysis | Testing for OWASP Top 10 | Sprint 3: Explotación controlada | Validar vulnerabilidades críticas mediante PoC seguras |
| Exploitation | Post-Exploitation | Sprint 4: Persistencia y escalamiento controlado | Verificar impacto y acceso a información sensible |
| Reporting | Remediation Verification | Sprint 5: Informe final y recomendaciones | Documentar hallazgos, riesgos e impactos al negocio |

Además, se complementa con las guías de:
- **OSSTMM (Open Source Security Testing Methodology Manual)**: como referencia para la evaluación objetiva de seguridad y métricas.  
- **NIST SP 800-115**: para estructurar la documentación y trazabilidad de pruebas.  
- **MITRE ATT&CK Framework**: como apoyo en la identificación de técnicas y tácticas de adversarios reales.

Este marco integrado garantiza que el proceso sea **repetible, medible y verificable**, manteniendo la ética profesional y la conformidad con buenas prácticas internacionales.  

La ejecución de cada sprint incluye reuniones de **Sprint Planning**, **Daily Scrums**, **Sprint Review** y **Retrospective**, donde se evalúan los avances técnicos, los obstáculos y las oportunidades de mejora.  
De esta manera, se asegura que cada iteración aporte resultados concretos (evidencias, PoC, registros) y que las decisiones técnicas se documenten oportunamente en función de la evolución del pentest.


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

La **Definición de Hecho (Definition of Done)** establece los criterios que determinan cuándo una tarea, user story o sprint se considera finalizado de manera satisfactoria.  
Su aplicación asegura que todos los entregables del proyecto cumplan estándares técnicos, éticos y de documentación coherentes con los objetivos del pentesting.

| Categoría | Criterio de cumplimiento | Evidencia esperada |
|------------|--------------------------|--------------------|
| **Técnico** | Las pruebas se ejecutaron en entornos autorizados y con metodologías reproducibles. | Capturas de terminal, logs o PoC controladas. |
| **Validación** | Cada hallazgo ha sido verificado al menos dos veces y clasificado según CVSS v3. | Registro en matriz de vulnerabilidades con puntaje y nivel de riesgo. |
| **Documentación** | El resultado de cada sprint está documentado con fecha, responsable y descripción de hallazgos. | Informe parcial y resumen técnico. |
| **Trazabilidad** | Se conserva el historial de comandos, herramientas y configuraciones usadas. | Carpeta `/evidence` o `/tools_log`. |
| **Seguridad y ética** | No se realizaron ataques destructivos, DoS ni acceso no autorizado a datos reales. | Declaración de conformidad firmada por el equipo. |
| **Revisión** | El Product Owner validó que la evidencia sea clara y comprensible. | Comentario o firma de validación. |


## 2.5 Herramientas

Durante la ejecución del proyecto se empleará un conjunto de herramientas de uso profesional incluidas en la distribución **Kali Linux**, complementadas con utilitarios especializados para cada fase del pentesting.  
Estas herramientas fueron seleccionadas conforme a las fases del estándar **PTES** y a las prácticas recomendadas por **OWASP**.

| Fase PTES / OWASP | Herramienta | Propósito / Uso principal |
|--------------------|-------------|---------------------------|
| **Reconocimiento y mapeo de activos** | `Nmap`, `Netdiscover`, `WhatWeb`, `Wappalyzer` | Identificación de hosts, puertos, servicios y tecnologías en uso. |
| **Enumeración de recursos y subdominios** | `Gobuster`, `ffuf`, `Dirb`, `Sublist3r` | Descubrimiento de rutas ocultas, endpoints y archivos sensibles. |
| **Análisis de vulnerabilidades web** | `Burp Suite`, `Nikto`, `OWASP ZAP` | Interceptar peticiones HTTP, detectar fallos de seguridad y validar respuestas. |
| **Explotación de vulnerabilidades** | `sqlmap`, `Hydra`, `Metasploit Framework` | Pruebas de inyección SQL, fuerza bruta y explotación controlada. |
| **Tráfico y protocolos** | `Wireshark`, `tcpdump` | Captura y análisis de paquetes de red, validación de cifrado y sesiones. |
| **Pruebas complementarias / scripts** | `Python`, `curl`, `bash` | Automatización de pruebas, generación de PoC y validación de payloads. |
| **Gestión de evidencia** | `Obsidian`, `CherryTree`, `Excel/Sheets` | Organización de hallazgos, logs, y generación de reportes intermedios. |


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
