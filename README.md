

<p align="center">
  <img src="assets/UPC_logo.png" alt="Logo UPC" width="140"/>
</p>

<h1 align="center">UNIVERSIDAD PERUANA DE CIENCIAS APLICADAS</h1>
<h2 align="center">Ingeniería de Software - Ciclo 08</h2>

---

<h2 align="center">Anti Hacking y Nuevas Tendencias de Seguridad</h2>
<p align="center"><strong>Código del curso:</strong> 1ASI0665-2520-14423</p>

<h3 align="center">Profesor</h3>
<p align="center"><strong>David Carlos Vera Olivera</strong></p>

---

<h2 align="center">INFORME DEL TRABAJO FINAL</h2>
<p align="center"><strong>Consultora:</strong> SecuraLabs</p>
<p align="center"><strong>Empresa:</strong> Tutormatch</p>

---

<h3 align="center">Integrantes</h3>

<div align="center">

<table>
  <tr>
    <th>Nombre y Apellido</th>
    <th>Código</th>
  </tr>
  <tr>
    <td>Leonardo José Aquino Cruz</td>
    <td>u20201b949</td>
  </tr>
  <tr>
    <td>Fabio Maurizio Nicolich Alvis</td>
    <td>u202218791</td>
  </tr>
  <tr>
    <td>Harold Miguel Elías Sánchez</td>
    <td>u202212684</td>
  </tr>
  <tr>
    <td>Piero Alberto Velarde Luyo</td>
    <td>u20211a620</td>
  </tr>
</table>

</div>

<p align="center"><strong>Octubre 2025</strong></p>

---

# Registro de Versiones del Informe

| **Versión** | **Fecha** | **Cambios Realizados** | **Responsable** |
|:--:|:--:|:--|:--|
| **1.0** | **2025-10-24** | **Entrega TP1 (Semana 9):** Documento de Alcance y primer paquete de entregables. Se completaron:<br><br>**Student Outcome:** Borrador sobre contribución al Outcome 2.<br><br>**Capítulo I:** (1.1) *Startup Profile* — descripción de la PyME y expectativas del cliente. (1.2) *Consultora* — descripción y perfiles/roles SCRUM. (1.3) *Solution Profile* — antecedentes, problemática y objetivos del pentesting. (1.4) *ROE* — alcance y condiciones iniciales.<br><br>**Capítulo II:** (2.1) Marco de referencia (Scrum, PTES, OWASP). (2.2) Backlog inicial (User Stories priorizadas). (2.3) Planificación de sprints (detalle Sprint 1).<br><br>**Capítulo III (Sprint 1):** Objetivo, actividades técnicas (configuración Kali, OSINT, nmap, gobuster, TLS checks) y entregables técnicos (*prep_evidence.txt*, *discovery.txt*, carpeta OSINT, lista de endpoints, screenshots) con PoC inicial.<br><br>**Capítulo IV:** Matriz de vulnerabilidades (entradas preliminares) y evidencias adjuntas. Incluye checklist DoD parcial y evidencia subida al repositorio. | **SecuraLabs** — Harold Miguel Elías Sánchez *(Product Owner)*; Fabio Maurizio Nicolich Alvis *(Scrum Master)*; Leonardo José Aquino Cruz *(Pentester & Analyst)*; Piero Alberto Velarde Luyo *(Technical Writer)* |
| **2.0** | **2025-12-03** | **Entrega Sprint 2 y avance de Sprint 3: Se completaron:**<br><br>**Capítulo II:** Actualización de la planificación ágil — ampliación de la correspondencia PTES/OWASP/Scrum y ajustes en actividades de Sprint 2.<br><br>**Capítulo III (Sprint 2):** Desarrollo completo del sprint: enumeración avanzada, descubrimiento de endpoints API, análisis de exposición de datos sensibles, verificación de credenciales débiles y recolección de evidencias técnicas (salidas de nmap, gobuster, whatweb, capturas de Burp). Se registraron PoC iniciales asociadas a vulnerabilidades preliminares.<br><br>**Capítulo III (Sprint 3 — inicio):** Incorporación de actividades de explotación controlada (SQLi, XSS, CSRF, subida de archivos inseguros, revisión TLS/headers). Se añadieron pruebas con Burp Suite, sqlmap y herramientas de explotación para validar hallazgos críticos.<br><br>**Capítulo IV:** Actualización de la matriz de vulnerabilidades — nuevos hallazgos documentados con CVSS provisional, impacto técnico y evidencia formal (screenshots, logs y outputs).<br><br>**Capítulo V:** Inclusión del borrador inicial del plan de mitigación basado en hallazgos de los sprints 2 y 3 (hardening, saneamiento de entradas, políticas de autenticación, mejoras TLS). | **SecuraLabs** — Harold Miguel Elías Sánchez (Product Owner); Fabio Maurizio Nicolich Alvis (Scrum Master); Leonardo José Aquino Cruz (Pentester & Exploit Developer); Piero Alberto Velarde Luyo (Technical Writer & Evidence Manager) |
---

# Project Report Collaboration Insights

Durante el desarrollo del proyecto, el equipo SecuraLabs adoptó un enfoque ágil basado en Scrum, distribuyendo los roles de manera clara para garantizar una colaboración efectiva y trazable.

## Roles Scrum
- **Product Owner (líder de consultora):**  
  **Harold Miguel Elías Sánchez**  
  Responsable de definir el alcance del servicio de pentesting, gestionar la comunicación con el cliente (SafeGuard Coffee), priorizar el Product Backlog y validar los entregables de cada sprint. Supervisa la aplicación de las reglas del **ROE (Rules of Engagement)** y asegura que las pruebas se desarrollen bajo lineamientos éticos y legales.

- **Scrum Master (coordinador de procesos):**  
  **Fabio Maurizio Nicolich Alvis**  
  Encargado de coordinar las reuniones de planificación y retrospectiva, facilitar la comunicación entre los miembros del equipo, garantizar la correcta aplicación del marco **Scrum** y el cumplimiento del **Definition of Done (DoD)**. También vela por la trazabilidad y organización del repositorio (GitHub, Trello).

- **Development Team (pentesters, documentadores, analistas):**  
  **Leonardo José Aquino Cruz** – Pentester y analista técnico, responsable de la ejecución de pruebas de reconocimiento, escaneo, explotación controlada y recolección de evidencias.  
  **Piero Alberto Velarde Luyo** – Documentador y analista, encargado de registrar hallazgos, elaborar el informe técnico y consolidar las recomendaciones de seguridad.  
  El equipo colabora en la planificación de sprints, priorización de User Stories y documentación de vulnerabilidades conforme al estándar **PTES/OWASP**.

## Herramientas de colaboración usadas
- Jira  
- GitHub  
- Microsoft Teams / WhatsApp  
- Otras herramientas técnicas (Burp Suite, Metasploit, etc.)

## Repositorio del informe

El informe final se desarrollará en un repositorio público bajo la organización 1ASI0665-antihacking-G1, donde se documentará todo el ciclo de vida del proyecto, incluyendo commits, versiones y entregables.
Repositorio oficial: [https://github.com/1ASI0665-antihacking-G1/report-hacking-G1](https://github.com/1ASI0665-antihacking-G1/report-hacking-G1) 

## Evidencia de colaboración

La evidencia de colaboración refleja la participación activa de todos los integrantes del equipo **SecuraLabs** en el repositorio oficial del proyecto.  
A través de commits, revisiones y coordinación mediante GitHub, se garantizó la trazabilidad y transparencia del desarrollo.

### Actividad general del repositorio (*Pulse*)
<img src="assets/evidence_collaboration/TP1/pulse_summary.PNG" alt="Pulse Summary"/>

### Gráfico de contribuciones por integrante
<img src="assets/evidence_collaboration/TP1/contributors_graph.PNG" alt="Contributors Graph"/>

### Historial de commits y mensajes 
<img src="assets/evidence_collaboration/TP1/commit1.png" alt="Commit 1"/>
<img src="assets/evidence_collaboration/TP1/commit2.png" alt="Commit 2"/>
<img src="assets/evidence_collaboration/TP1/commit3.png" alt="Commit 3"/>
<img src="assets/evidence_collaboration/TP1/commit4.png" alt="Commit 4"/>

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

## Student Outcome

| Criterio Específico | Acciones realizadas | Conclusiones |
|----------------------|--------------------|---------------|
| **Diseña soluciones en ingeniería de software que satisfacen necesidades específicas considerando salud pública, seguridad, bienestar, factores globales, culturales, sociales, ambientales y económicos.** | **Harold Elías:** Diseñé el alcance del servicio de pentesting considerando la seguridad y privacidad de los usuarios de la plataforma TutorMatch, priorizando la protección de datos personales y la reducción de riesgos de exposición. Al igual que propuse la implementación de buenas prácticas de ciberseguridad y mecanismos de validación ética para garantizar un entorno digital seguro para estudiantes y tutores.<br><br>**Fabio Nicolich:** Estructuré el marco de trabajo ágil que permitió diseñar el servicio de pentesting de manera organizada y con enfoque en la seguridad y bienestar digital. También promoví el diseño de un flujo de trabajo que respetara normas éticas y buenas prácticas internacionales en seguridad de la información, considerando factores culturales y sociales de los usuarios finales.<br><br>**Leonardo Aquino:** Diseñé los casos de prueba y las estrategias de evaluación de vulnerabilidades aplicando metodologías reconocidas (OWASP, NIST), con el fin de fortalecer la seguridad del producto. A su vez, consideré el impacto que una falla de seguridad podría tener en la reputación de la empresa y en la experiencia de los usuarios, priorizando soluciones seguras y sostenibles.<br><br>**Piero Velarde:** Diseñé la estructura de los informes técnicos y reportes de resultados asegurando claridad, transparencia y ética profesional. También incorporé en la documentación recomendaciones específicas que contribuyen al bienestar digital y a la prevención de malas prácticas en el manejo de información. | El equipo de **SecuraLabs** diseñó un servicio de pentesting integral enfocado en la protección de la información, la privacidad y el bienestar de los usuarios. Cada integrante aportó desde su rol a la creación de una solución segura y responsable, considerando factores sociales, culturales y éticos, demostrando una comprensión integral del impacto de la ingeniería de software en la sociedad digital. |
| **Valida que el diseño de la solución considere salud pública, seguridad, bienestar, y factores globales, culturales, sociales, ambientales y económicos.** | **Harold Elías:** Validé que los requerimientos del servicio de pentesting cumplieran con estándares éticos y no afectaran la disponibilidad ni la estabilidad del sistema. También supervisé la revisión de los hallazgos para asegurar que las recomendaciones propuestas reforzaran la seguridad y bienestar de los usuarios finales.<br><br>**Fabio Nicolich:** Validé la correcta ejecución del plan de trabajo y el cumplimiento de buenas prácticas en seguridad de la información durante cada sprint del proyecto. Al igual que verifiqué que el diseño del servicio mantuviera un enfoque responsable frente a factores globales y sociales, garantizando la integridad del proceso.<br><br>**Leonardo Aquino:** Validé los resultados de las pruebas de penetración mediante herramientas y análisis técnico para asegurar la fiabilidad de los hallazgos. También confirmé que las vulnerabilidades detectadas fueron tratadas de manera que promuevan un entorno seguro y éticamente responsable.<br><br>**Piero Velarde:** Validé la coherencia y exactitud de los informes técnicos, asegurando que la información presentada fuera clara y comprensible para el cliente. A su vez, garanticé que los reportes reflejaran una comunicación responsable, protegiendo la confidencialidad de los datos y fomentando la conciencia sobre seguridad digital. | El equipo **SecuraLabs** validó de manera exhaustiva que el diseño y ejecución del servicio de pentesting cumplieran con los principios de seguridad, ética y bienestar digital. Su trabajo evidenció la importancia de verificar que cada decisión técnica tenga un impacto positivo en la confianza, estabilidad y sostenibilidad de las soluciones de software, alineándose con valores globales y sociales del entorno tecnológico actual. |


---

# Capítulo I: Introducción

## 1.1 Startup Profile (Cliente)
### Descripción de la PyME 

SafeGuard Coffee es una pequeña empresa peruana dedicada a la selección, tostado y comercialización de cafés especiales de alta calidad. Desde su fundación en 2010, la empresa ha recorrido diversas regiones cafeteras del mundo en busca de granos excepcionales, trabajando de manera directa con agricultores que comparten su compromiso con la sostenibilidad, el comercio justo y la excelencia en cada etapa del proceso. </br>

La empresa forma parte del sector Agroindustrial, un rubro que combina prácticas agrícolas tradicionales con procesos modernos de trazabilidad, control de calidad y experiencia sensorial. Su principal propuesta de valor es ofrecer cafés de origen cuidadosamente seleccionados, provenientes de zonas de alta montaña garantizando una experiencia auténtica y única en cada taza. </br>

SafeGuard Coffee basa su modelo de negocio en la venta de café tostado, productos complementarios y experiencias relacionadas con el consumo del café, todo respaldado por un ecosistema digital que permite una gestión eficiente de clientes, ventas y operaciones.

**Servicios digitales ofrecidos**

Para asegurar una operación moderna y accesible, la empresa cuenta con un ecosistema tecnológico dividido en dos componentes principales:
- **Frontend Web:** Funciona como el portal principal para clientes y distribuidores, permitiéndoles explorar el catálogo de cafés de especialidad, conocer el origen de cada grano, realizar compras en línea y gestionar sus pedidos, pagos y envíos. Además, brinda acceso a información sobre certificaciones sostenibles y recomendaciones de preparación, todo mediante una interfaz intuitiva y orientada a la experiencia del usuario.
- **Backend:** El backend actúa como la API central que gestiona las operaciones internas de la empresa, incluyendo el control de inventario, la trazabilidad de lotes, el procesamiento de pedidos y pagos, y la administración de usuarios y perfiles. También coordina la sincronización con sistemas logísticos y la gestión del contenido y la información de productos, garantizando un flujo de datos seguro, eficiente y actualizado.

Ambas plataformas trabajan conjuntamente para brindar una experiencia fluida, segura y confiable, permitiendo que la empresa mantenga un estándar de calidad acorde con su compromiso: llevar a cada cliente un café sostenible, de origen certificado y cuidadosamente seleccionado.

**Misión y visión**
- **Misión:** Ofrecer cafés de especialidad de origen sostenible, conectando directamente a los consumidores con agricultores comprometidos con la calidad y el comercio justo. Buscamos brindar una experiencia auténtica en cada taza mediante procesos responsables, trazabilidad completa y el uso de tecnologías que faciliten el acceso a nuestros productos artesanales.
- **Visión:** Consolidarnos en los próximos cinco años como una de las marcas de café de especialidad más reconocidas del país, destacando por nuestra calidad, sostenibilidad y conexión directa con productores de alta montaña. Aspiramos a liderar la transformación digital del sector cafetalero mediante soluciones innovadoras que acerquen la experiencia del café premium a consumidores locales e internacionales.

**Mercado objetivo**

El mercado objetivo de SafeGuard Coffee está compuesto por consumidores interesados en cafés de especialidad, especialmente aquellos que valoran la sostenibilidad, el comercio directo y la trazabilidad del producto. La empresa se orienta tanto a clientes finales como a distribuidores, cafeterías boutique y negocios gastronómicos. A mediano plazo, busca expandir su presencia a nuevos segmentos del sector horeca y consolidarse como un referente dentro del mercado nacional e internacional de cafés de alta calidad.

### Expectativas del cliente  

Las expectativas del cliente se centran en recibir una evaluación de ciberseguridad clara, práctica y orientada a la acción, que permita identificar y priorizar amenazas reales dentro del ecosistema digital de SafeGuard Coffee. El cliente espera que el análisis detecte vulnerabilidades que puedan afectar la integridad del flujo de compra, la disponibilidad del sistema, la confidencialidad de los datos de clientes o la seguridad de las transacciones en línea. Esto incluye fallas en controles de autenticación, configuraciones inseguras, exposición de información sensible, riesgos de acceso no autorizado al inventario o al backend, y cualquier debilidad que pueda facilitar ataques como inyección, secuestro de sesión o escalación de privilegios. </br>

Asimismo, el cliente espera un informe técnico exhaustivo con hallazgos reproducibles y evidencia verificable (logs, capturas, payloads y pasos de explotación), acompañado de un plan de remediación priorizado que detalle mitigaciones concretas, estimación de esfuerzo y nivel de criticidad de cada vulnerabilidad. También valora un resumen ejecutivo orientado a personal no técnico, así como recomendaciones para fortalecer sus prácticas de seguridad, mejorar su postura de defensa y establecer lineamientos sostenibles de ciberseguridad en sus operaciones digitales.

## 1.2 Consultora de Ciberseguridad (Equipo)
### Descripción de la consultora  

SecuraLabs es una consultora académica de ciberseguridad conformada por estudiantes de la carrera de Ingeniería de Software de la Universidad Peruana de Ciencias Aplicadas (UPC). El equipo se especializa en la aplicación de metodologías de seguridad ofensiva, evaluación de vulnerabilidades y pruebas de penetración (pentesting) orientadas a entornos web, móviles y de infraestructura en red.
El enfoque de SecuraLabs se centra en la identificación proactiva de amenazas y evaluación del riesgo tecnológico dentro de organizaciones que buscan fortalecer su postura de seguridad digital. El equipo combina conocimientos técnicos adquiridos en el ámbito académico con buenas prácticas reconocidas, como el uso de estándares OWASP, NIST SP 800-115 y MITRE ATT&CK, aplicados a contextos reales de desarrollo y despliegue de software.

**Misión**

Nuestra misión es ayudar a las organizaciones a descubrir y mitigar vulnerabilidades antes de que puedan ser explotadas, mediante la ejecución de pruebas controladas y éticas que simulan ataques reales. Buscamos fomentar una cultura de seguridad preventiva y aprendizaje continuo, aportando soluciones prácticas y estrategias de mejora que fortalezcan los sistemas y procesos de nuestros clientes frente a las nuevas tendencias de ciberamenazas.


### Perfiles de los integrantes y roles Scrum  

| Perfil | Descripción |
|--------|-------------|
| <img src="assets/profiles/harold_elias.jpg" alt="Harold" width="540"/> | **Harold Elías – Product Owner**</br>Estudiante de Ingeniería de Software en octavo ciclo, con interés en las áreas de ciberseguridad y pentesting. Posee experiencia en los lenguajes C++ y Python a nivel intermedio, además de haber participado en proyectos de desarrollo web y en la implementación de pruebas unitarias utilizando C# con NUnit.</br> Como Product Owner en SecuraLabs, Harold se encarga de definir y priorizar el backlog de seguridad, alineando las necesidades del cliente con los objetivos técnicos del equipo. Su capacidad de análisis y trabajo colaborativo facilita la toma de decisiones orientadas a maximizar el valor de las pruebas de ciberseguridad, asegurando que los entregables respondan a las expectativas del cliente.|
|<img src="assets/profiles/fabio_nicolich.jpg" alt="Fabio" width="540"/>|**Fabio Nicolich – Scrum Master**</br>Estudiante de Ingeniería de Software en séptimo ciclo, destacado por su liderazgo, responsabilidad y proactividad en la gestión de equipos. Cuenta con conocimientos en C++, HTML, CSS, JavaScript y Python, además de interés en el uso de frameworks modernos para el desarrollo de aplicaciones web.</br> Como Scrum Master, Fabio promueve la comunicación efectiva, la coordinación del equipo y la aplicación de los valores ágiles, garantizando el cumplimiento de los objetivos en cada sprint. Su compromiso con la calidad y la mejora continua contribuye a mantener un entorno colaborativo, motivando al equipo hacia resultados consistentes y orientados al aprendizaje conjunto.|
|<img src="assets/profiles/leonardo_aquino.jpg" alt="Leonardo" width="540"/>|**Leonardo Aquino – Pentester & Security Analyst**</br>Estudiante de Ingeniería de Software en décimo ciclo, con experiencia en desarrollo web, ciberseguridad y diseño de videojuegos utilizando Godot y Unity. Domina lenguajes como C++, Python y JavaScript, y posee una fuerte orientación hacia la creación de soluciones seguras y la prevención de vulnerabilidades.</br> Como Pentester & Security Analyst en SecuraLabs, Leonardo lidera la ejecución de las pruebas ofensivas y el análisis técnico de vulnerabilidades, participando en la identificación, validación y documentación de hallazgos. Su capacidad analítica y su enfoque en resultados fortalecen la calidad técnica del proceso de evaluación de seguridad.|
|<img src="assets/profiles/piero_velarde.jpg" alt="Piero" width="540"/>|**Piero Velarde – Technical Writer & Documentador**</br>Estudiante de Ingeniería de Software en séptimo ciclo, con interés en tecnologías emergentes, programación y ciberseguridad. Maneja los lenguajes C++, Python, JavaScript y Dart, y mantiene una actitud proactiva hacia el aprendizaje continuo y la investigación tecnológica.</br> Dentro de SecuraLabs, Piero desempeña el rol de Technical Writer & Documentador, siendo responsable de la redacción técnica, estructuración del informe y sistematización de evidencias. Además, asegura la coherencia comunicativa entre las fases técnicas y los entregables finales, contribuyendo a la claridad, precisión y formalidad de los documentos presentados al cliente.|


## 1.3 Solution Profile
### Antecedentes y problemática  

Las pequeñas y medianas empresas que operan en entornos digitales como Safeguard Coffee, dedicada a la venta de productos y servicios a través de plataformas web, se encuentran cada vez más expuestas a riesgos de seguridad informática. La adopción de sistemas basados en comercio electrónico, formularios de contacto, pasarelas de pago, bases de datos en la nube y APIs incrementa su superficie de ataque, convirtiéndolas en objetivos atractivos para actores maliciosos que buscan vulnerar sistemas poco protegidos. </br>

Durante un análisis preliminar del sitio web de Safeguard Coffee (https://safeguard-coffee.ngrok.app/), se identificaron posibles deficiencias típicas de plataformas emergentes, tales como:

- Controles insuficientes de validación y sanitización de entradas.
- Exposición potencial de endpoints accesibles públicamente.
- Configuraciones inadecuadas de seguridad web (cabeceras HTTP, políticas de contenido, configuración TLS/SSL).
- Falta de mecanismos robustos para la protección de datos y autenticación.

Estas condiciones aumentan la probabilidad de ataques comunes como inyección SQL, XSS, secuestro de sesiones, scraping automatizado, fuerza bruta y exploración no autorizada de recursos internos. La empresa, ante el crecimiento de su presencia digital, reconoce la necesidad de una auditoría de seguridad ofensiva que evalúe de forma realista su postura actual de ciberseguridad. </br>

Asimismo, incidentes recientes en otras empresas similares del sector, donde se han reportado filtraciones de información por vulnerabilidades no corregidas, refuerzan la urgencia de actuar de manera preventiva. Por ello, Safeguard Coffee Co. ha solicitado la realización de una evaluación integral de seguridad ofensiva, con el objetivo de identificar brechas críticas, fortalecer sus activos digitales y establecer un plan de mejora continua basado en las mejores prácticas del marco OWASP y estándares internacionales de pentesting.

### Objetivos del pentesting (General y específicos)  

**Objetivo general**

Realizar una evaluación integral de seguridad ofensiva (pentesting) sobre el sitio web de Safeguard Coffee, con el fin de identificar vulnerabilidades técnicas, riesgos de exposición de datos y configuraciones inseguras. La evaluación permitirá elaborar un informe técnico y un plan de remediación que fortalezcan la postura de seguridad y reduzcan la probabilidad de explotación por parte de actores maliciosos.

**Objetivos específicos**
1.	**Identificar vulnerabilidades críticas en los componentes principales del sitio web de SafeGuard Coffee** (frontend, endpoints, formularios y servicios asociados), mediante la ejecución de pruebas de inyección, validación de entradas y análisis de permisos.

2.	**Evaluar la robustez de los mecanismos de autenticación, gestión de sesiones y recuperación de cuentas**, comprobando la resistencia del sistema frente a ataques de fuerza bruta, enumeración de usuarios y suplantación de identidad, en caso de que la plataforma implemente dichos mecanismos.

3.	**Detectar exposición de información sensible** (tokens, correos electrónicos, metadatos, claves embebidas o datos personales) en las respuestas del servidor, archivos públicos, librerías utilizadas o configuraciones del sitio.

4.	**Analizar la configuración de seguridad de la infraestructura y servicios asociados**, incluyendo protocolos de cifrado (TLS/HTTPS), encabezados de seguridad HTTP, políticas de cookies, uso de librerías desactualizadas y posibles puntos de acceso no controlados.

5.	**Ejecutar pruebas de explotación controlada (Proof of Concept)** sobre las vulnerabilidades encontradas, validando su impacto y nivel de riesgo de acuerdo con metodologías OWASP y CVSS.

Finalmente, una vez cumplidos todos los objetivos, elaborar un informe técnico detallado y un plan de remediación, priorizando las acciones correctivas y recomendaciones para mitigar riesgos y fortalecer la seguridad del ciclo de desarrollo bajo prácticas DevSecOps.


## 1.4 Aceptación del Servicio de Pentesting (Rules of Engagement)

<img src="assets/rules_of_engagement.png" alt="Rules_of_Engagement" width="1240"/>

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
| 01 | US-01 | Identificación de servicios expuestos | Como atacante externo quiero identificar los servicios expuestos del sistema para conocer los puertos abiertos y versiones activas. | 3 |
| 02 | US-02 | Descubrimiento de directorios ocultos | Como atacante quiero descubrir directorios ocultos del servidor web para identificar rutas accesibles con respuesta HTTP 200 o 301. | 5 |
| 03 | US-03 | Obtención de información pública (OSINT) | Como atacante quiero obtener información pública del sistema para identificar correos, usuarios y tecnologías utilizadas. | 5 |
| 04 | US-04 | Validación de seguridad de túneles | Como atacante quiero validar la seguridad de los túneles de comunicación para confirmar la accesibilidad a los dominios expuestos. | 2 |
| 05 | US-05 | Enumeración de endpoints web | Como pentester quiero enumerar los endpoints del sitio web para identificar todos los archivos .php accesibles. | 5 |
| 06 | US-06 | Validación de credenciales web | Como pentester quiero validar credenciales web para verificar un inicio de sesión exitoso con el usuario carlos.mendez@safeguard.coffee. | 3 |
| 07 | US-07 | Análisis de vulnerabilidades web básicas | Como pentester quiero analizar vulnerabilidades web básicas para identificar headers inseguros, XSS y SQLi. | 8 |
| 08 | US-08 | Documentación de la superficie de ataque | Como pentester quiero documentar la superficie de ataque para listar formularios, parámetros GET/POST y cookies. | 8 |
| 09 | US-09 | Acceso a logs del sistema | Como atacante quiero acceder a los logs internos del sistema para descargar archivos de registro. | 3 |
| 10 | US-10 | Obtención de credenciales de infraestructura | Como atacante quiero obtener credenciales de infraestructura para identificar usuarios y contraseñas de base de datos y SSH. | 8 |
| 11 | US-11 | Extracción de información de la base de datos | Como atacante quiero extraer información de la base de datos para obtener un dump de tablas de clientes y empleados. | 8 |
| 12 | US-12 | Acceso remoto al servidor | Como atacante quiero obtener acceso remoto al servidor para establecer una conexión SSH exitosa. | 5 |
| 13 | US-13 | Escalamiento de privilegios a root | Como atacante quiero escalar privilegios a nivel root para obtener una shell con UID 0. | 8 |
| 14 | US-14 | Búsqueda de archivos sensibles protegidos | Como atacante quiero buscar archivos sensibles en directorios protegidos para leer /root/ y archivos de configuración. | 5 |
| 15 | US-15 | Exfiltración de base de datos de clientes | Como atacante quiero exfiltrar la base de datos de clientes para descargar un archivo CSV o SQL a mi máquina local. | 5 |
| 16 | US-16 | Persistencia en el sistema (simulada) | Como atacante quiero mantener persistencia en el sistema para crear un usuario backdoor de manera simulada. | 3 |

## Criterios de aceptación generales y Definition of Done (DoD)

### Criterios de Aceptación Generales por Historia

- **Reproducibilidad:**  
Cada hallazgo debe incluir de forma detallada los pasos exactos para su reproducción, especificando requests, payloads, headers y condiciones del entorno.

- **Evidencia:**  
Toda vulnerabilidad identificada debe estar sustentada con evidencias claras, tales como capturas de pantalla y salidas de herramientas de análisis (Burp Suite, sqlmap, nmap, OWASP ZAP, Nessus, entre otras).

- **Impacto:**  
Se debe asignar una clasificación CVSS provisional, indicando el impacto potencial sobre la confidencialidad, integridad y disponibilidad de los datos, así como sobre la funcionalidad de la plataforma SafeGuard Coffee.

- **Recomendación:**  
Por cada hallazgo se debe proponer una mitigación técnica concreta, clara y aplicable al entorno evaluado.  

- **Ética / Legal:**  
En caso de que el ROE (Rules of Engagement) prohíba la extracción de datos reales, las Proof of Concept (PoC) únicamente deben demostrar la existencia de la vulnerabilidad o la metadata asociada, sin comprometer información sensible del sistema ni de los usuarios.

### Definition of Done (DoD) por Historia de Usuario

- La historia de usuario se encuentra documentada y vinculada al Sprint Backlog correspondiente.

- Las evidencias (screenshots, outputs de herramientas, colecciones Postman/Burp, reportes de ZAP/Nessus) están adjuntas, ordenadas y correctamente nombradas.  

- Cada hallazgo cuenta con su descripción de impacto y una priorización de riesgo (Crítico, Alto, Medio, Bajo).  

- Se incluye al menos una recomendación técnica priorizada, con su respectivo horizonte de mitigación.  

- El checklist de reproducción de la vulnerabilidad se encuentra completado y validado.
  
## 2.3 Planificación de sprints (Sprint Planning)

Todas las actividades técnicas se ejecutaron sobre el proyecto **SafeGuard Coffee**, en un entorno de laboratorio expuesto mediante **Ngrok**, autorizado para fines académicos.

Antes de iniciar las pruebas se definieron las **ROE (Rules of Engagement)** considerando:

- **Entorno permitido:** dominio público de laboratorio (*.ngrok.app).
- **Alcance:** únicamente reconocimiento, enumeración y acceso a archivos expuestos.
- **Restricciones:** no realizar explotación destructiva ni ataques de denegación de servicio.
- **Extracción de datos:** solo evidencia mínima necesaria (PoC).
- **Ventanas de ejecución:** fuera de horarios productivos.

---

### Sprint 1: Reconocimiento & Escaneo inicial

**Duración:** 1 semana

**Metodología:** PTES – Fase 1 (Intelligence Gathering)

**Objetivo:** Identificar y documentar la superficie de ataque pública de SafeGuard Coffee: dominio, servicios, rutas web y posibles vectores iniciales de acceso.

**Sprint Backlog 1**

| User Story Id | User Story Title | Work Item Id | Work Item Title | Description | Estimation | Assigned To | Status |
|---:|---|---:|---|---|:--:|:--|:--|
| US-01 | Reconocimiento inicial y mapeo de superficie | 1.1 | Preparación del entorno | Configuración de Kali Linux, creación de estructura de carpetas del proyecto y validación del entorno local. | (1h) | Leonardo | Done |
| US-01 | Reconocimiento inicial y mapeo de superficie | 1.2 | OSINT | Recolección de información pública del dominio mediante Google Dorks, TheHarvester y análisis de sitemap. | (2h) | Leonardo | Done |
| US-12 | Escaneo de puertos y servicios de red | 1.3 | Validación de servicios expuestos | Verificación manual de conectividad HTTP/HTTPS usando netcat debido a restricciones de Ngrok. | (1h) | Leonardo | Done |
| US-04 | Descubrimiento web | 1.4 | Enumeración recursiva /backup | Análisis del directorio /backup y detección de archivos sensibles. | (2h) | Leonardo | Done |
| US-04 | Descubrimiento web | 1.5 | Descubrimiento web | `gobuster`/`ffuf`, `whatweb` para directorios y fingerprinting. | (1h) | Leonardo | Done |
| US-08 | Verificación de TLS y headers | 1.6 | Fingerprinting HTTP | Identificación de tecnologías backend y cabeceras de seguridad ausentes mediante curl. | (1h) | Leonardo / Piero | Done |
| US-01 | Documentación de superficie de ataque | 1.7 | Registro de evidencias | Organización de evidencias, outputs y hallazgos críticos del Sprint. | (1h) | Piero | Done |

**Objetivo del Sprint:**  
Identificar y documentar de forma reproducible la superficie de ataque expuesta de SafeGuard Coffee, incluyendo:

- Dominio público activo.
- Servicios accesibles (HTTP/HTTPS).
- Tecnologías backend.
- Rutas sensibles accesibles.
- Archivos críticos expuestos.

Este inventario guía directamente las actividades de explotación controlada del Sprint 2.

**Actividades técnicas Ejecutadas**

**1. Preparación del Entorno**

- Configuración de Kali Linux.
- Creación de estructura de directorios del proyecto.
- Organización de carpetas OSINT, Nmap y Enumeración.

**2. OSINT para SafeGuard Coffee**

- Google Dorks para:
  - Archivos PHP expuestos.
  - Directorios listables.
  - Posibles credenciales en texto plano.
- TheHarvester para:
  - Correos electrónicos.
  - Subdominios.
- Descarga e inspección de sitemap.xml.

**3. Validación de Servicios**

- Uso de netcat para validar conectividad en:
  - Puerto 80 (HTTP).
  - Puerto 443 (HTTPS).
- No se ejecutó escaneo agresivo con Nmap por limitaciones del túnel Ngrok.

**4. Enumeración de Directorios**

- Enumeración manual sobre raíz del sitio mediante script Bash con curl.
- Identificación del directorio crítico: `/backup`

**5. Enumeración Recursiva de `/backup`**

- Análisis recursivo de rutas internas.
- Descubrimiento del archivo:
  - credentials.bak (200 OK – Crítico)

**6. Análisis de Archivo Crítico**

- Descarga del archivo.
- Identificación de credenciales administrativas válidas.


**Entregables del Sprint 1**

- Carpeta /osint/ con:
  - Resultados de Google Dorks.
  - TheHarvester.
  - Sitemap descargado.
- Carpetas:
  - `/enumeracion/`
  - `/backup/`
- Archivo `credentials.bak` como evidencia crítica.
- Capturas de:
  - Enumeración de directorios.
  - Cabeceras HTTP.
  - Descarga del archivo sensible.

Documento de **inventario inicial de superficie de ataque**.

---

### Sprint 2: Enumeración y vulnerabilidades preliminares

**Duración:** Semana 3 – 4

**Metodología:** PTES – Fase 2 (Vulnerability Analysis) + OWASP Testing Guide

**Objetivo del Sprint:**
Enumerar en profundidad las funcionalidades del sitio web de SafeGuard Coffee, validar las credenciales obtenidas en el Sprint 1 e identificar vulnerabilidades preliminares de forma no destructiva.


**Sprint Backlog 2**

| User Story Id | User Story Title | Work Item Id | Work Item Title | Description | Estimation | Assigned To | Status |
|---:|---|---:|---|---|:--:|:--|:--|
| US-05 | Enumeración de endpoints web | 2.1 | Preparación del entorno Sprint 2 | Creación de estructura de carpetas para Nikto, headers y enumeración web. | (1h) | Harold | Done |
| US-07 | Análisis de vulnerabilidades web | 2.2 | Escaneo Nikto | Identificación de configuraciones inseguras y directorios peligrosos. | (2h) | Harold | Done |
| US-07 | Análisis de vulnerabilidades web | 2.3 | Análisis de cabeceras HTTP | Verificación manual de HSTS, CSP, X-Frame-Options. | (1h) | Harold | Done |
| US-06 | Validación de credenciales | 2.4 | Login con credenciales filtradas | Autenticación en panel administrativo usando credenciales de `credentials.bak.` | (1h) | Harold | Done |
| US-05 | Enumeración de endpoints web | 2.5 | Enumeración autenticada | Descubrimiento de rutas internas usando cookies de sesión válidas. | (2h) | Harold | Done |
| US-08 | Documentación de superficie de ataque | 2.6 | Registro de evidencias y matriz de vulnerabilidades | Clasificación de vulnerabilidades preliminares con severidad. | (1h) | Piero | Done |

**Objetivo:**  
Enumerar en profundidad los endpoints web públicos y autenticados de SafeGuard Coffee, validar las credenciales obtenidas en el Sprint 1 y detectar vulnerabilidades preliminares a nivel de configuración, cabeceras de seguridad y exposición de información sensible, bajo un enfoque no destructivo.

**Actividades técnicas**
- Preparación del entorno de trabajo para el Sprint 2 y organización de carpetas de evidencias.
- Escaneo automático de vulnerabilidades web mediante Nikto.
- Análisis manual de cabeceras HTTP para verificación de políticas de seguridad.
- Validación de credenciales obtenidas en el Sprint 1 mediante autenticación real en el sistema.
- Enumeración autenticada de directorios y funciones internas del panel administrativo.
- Identificación de rutas internas, archivos de log y posibles vectores de ataque adicionales.
- Documentación de la superficie de ataque autenticada (formularios, parámetros, sesiones, cookies).

**Entregables**
- Carpeta del Sprint 2 con estructura organizada (nikto, headers, web_enum).
- Reporte de escaneo Nikto.
- Archivo de cabeceras HTTP capturadas.
- Evidencias de autenticación exitosa en el sistema.
- Evidencias de enumeración autenticada.
- Listado de vulnerabilidades preliminares detectadas.
- Registro de la superficie de ataque autenticada.

---

### Sprint 3: Explotación controlada (web, APIs)

**Duración:** Semana 5 – 6

**Metodología:** PTES – Fase 3 (Exploitation)

**Objetivo del Sprint:**
Explotar de manera controlada las vulnerabilidades críticas identificadas en los sprints previos para acceder a los logs internos del sistema, obtener credenciales de infraestructura, extraer información de la base de datos y lograr acceso remoto al servidor mediante SSH, respetando las reglas de compromiso (ROE).

**Sprint Backlog 3**

| User Story Id | User Story Title | Work Item Id | Work Item Title | Description | Estimation | Assigned To | Status |
|---:|---|---:|---|---|:--:|:--|:--|
| US-09 | Acceso a logs del sistema | 3.1 | Descarga de logs internos | Descarga y análisis del archivo `db_connection_test.log` desde `/admin/logs/`. | (2h) | Leonardo | Planned |
| US-10 | Obtención de credenciales de infraestructura | 3.2 | Extracción de credenciales | Identificación de usuarios y contraseñas de DB y SSH desde los logs internos. | (2h) | Harold | Planned |
| US-11 | Extracción de información de base de datos | 3.3 | Acceso y dump de BD | Conexión remota a MySQL y consulta de tablas de clientes y empleados. | (3h) | Leonardo | Planned |
| US-12 | Acceso remoto al servidor | 3.4 | Conexión SSH al servidor | Acceso remoto mediante SSH con credenciales obtenidas y verificación de privilegios. | (2h) | Leonardo | Planned |

**Objetivo:**  
Explotar de forma controlada las vulnerabilidades críticas identificadas en los sprints anteriores para obtener acceso a los logs internos del sistema, credenciales de infraestructura, información sensible de la base de datos y acceso remoto al servidor mediante SSH, respetando en todo momento las reglas de compromiso (ROE).

**Actividades técnicas**
- Preparación del entorno de trabajo para actividades de explotación y organización de evidencias.
- Descarga y análisis de archivos de log internos desde el panel administrativo.
- Identificación y validación de credenciales de base de datos y acceso remoto obtenidas desde los logs.
- Conexión remota a la base de datos MySQL mediante credenciales válidas.
- Enumeración de bases de datos, tablas y extracción controlada de información sensible.
- Obtención de acceso remoto al servidor mediante conexión SSH.
- Verificación de privilegios del usuario obtenido en el sistema.
- Documentación técnica de cada vector de explotación ejecutado.

**Entregables**
- Carpeta del Sprint 3 organizada (logs, db_dump).
- Evidencias de descarga y análisis de archivos de log internos.
- Evidencias de conexión exitosa a la base de datos MySQL.
- Evidencias de extracción de información de tablas críticas.
- Evidencias de acceso remoto al servidor mediante SSH.
- Registro de credenciales de infraestructura comprometidas (entorno de laboratorio).
- Documentación técnica de vectores de explotación utilizados.
- Matriz de impacto preliminar de la información comprometida.

---

### Sprint 4: Post-explotación y persistencia

**Duración:** Semana 7 – 8

**Metodología:** PTES – Fase 4 (Post Exploitation)

**Objetivo del Sprint:**
Escalar privilegios hasta nivel root en el servidor comprometido, localizar información sensible en directorios protegidos, exfiltrar datos críticos de clientes y evaluar mecanismos de persistencia de forma controlada, respetando las reglas de compromiso (ROE).

**Sprint Backlog 4**

| User Story Id | User Story Title | Work Item Id | Work Item Title | Description | Estimation | Assigned To | Status |
|---:|---|---:|---|---|:--:|:--|:--|
| US-13 | Escalamiento de privilegios a root | 4.1 | Enumeración de privilegios sudo | Verificación de permisos sudo del usuario `sysadmin` para detectar posibles vías de escalamiento. | (2h) | Leonardo | Planned |
| US-13 | Escalamiento de privilegios a root | 4.2 | Explotación de binario con NOPASSWD | Uso del binario `python3` con sudo para obtener shell con UID 0. | (2h) | Leonardo | Planned |
| US-14 | Búsqueda de archivos sensibles | 4.3 | Exploración de directorio `/root` | Lectura de archivos de configuración, notas administrativas y backups. | (2h) | Leonardo | Planned |
| US-15 | Exfiltración de base de datos de clientes | 4.4 | Transferencia de archivo de respaldo | Copia y descarga del archivo `clientes_exportacion.csv` mediante SCP hacia la máquina del atacante. | (2h) | Leonardo | Done |
| US-16 | Persistencia (simulada) | 4.5 | Evaluación de persistencia | Análisis de posibilidades de creación de usuarios backdoor o tareas programadas (sin ejecución real). | (1h) | Leonardo | Planned |

**Objetivo:**  
Realizar post-explotación controlada para escalar privilegios a root, localizar información sensible adicional y evaluar vectores de persistencia y movimiento lateral teórico, entregando recomendaciones de mitigación y detección.

**Actividades técnicas**
- Enumeración local de privilegios y comprobación de configuraciones sudo / SUID.
- Explotación segura de vectores de escalamiento (uso controlado de binarios con NOPASSWD, SUID, etc.).
- Exploración de directorios protegidos (/root, backups) para identificar artefactos y backups (solo metadata cuando ROE lo exija).
- Transferencia controlada de artefactos de prueba (simulada o con datos no sensibles) y verificación de rutas de exfiltración permitidas.
- Revisión de logging y mecanismos de detección; comprobación de si acciones quedan registradas.
- Documentación de técnicas de persistencia posibles (simulación) y propuestas de mitigación operativa y de monitoreo.

**Entregables**
- Carpeta del Sprint 4 organizada (postexp, artifacts).
- Registro de comandos y scripts de escalamiento y búsqueda (sanitizados).
- Lista de artefactos accesibles (metadata) y, si procede, archivos de respaldo (sanitizados).
- Checklist de remediación inmediata (rotación de credenciales, cierre de endpoints, permisos).
- Recomendaciones de detección (reglas SIEM/IDS, formatos de logging y alertas).
- Matriz de impacto final y plan de reversión/mitigación priorizado.

---

### Sprint 5: Informe final y recomendaciones

**Objetivo:**  
Consolidar todos los hallazgos del proceso de pentesting, clasificar las vulnerabilidades mediante CVSS, documentar evidencias técnicas y proponer un plan de mitigación priorizado a corto, mediano y largo plazo para SafeGuard Coffee.

**Actividades técnicas**
- Consolidación de la **matriz final de vulnerabilidades**, incluyendo descripción, severidad (CVSS), impacto y trazabilidad por cada hallazgo.
- Elaboración del **informe final** en formato técnico y ejecutivo (resumen ejecutivo, alcance, metodología, resultados y mitigaciones).
- Organización y empaquetado de **evidencias técnicas**: accesos, explotación, escalamiento de privilegios, exfiltración y pruebas de impacto.
- Clasificación de vulnerabilidades según **criticidad y prioridad de remediación**.
- Diseño de la **hoja de ruta de mitigación** (corto, mediano y largo plazo).
- Sanitización de información sensible (PII) y validación de cumplimiento ético y de ROE.
- Preparación de **presentación ejecutiva** para exposición final de resultados.

**Entregables**
- Informe final de auditoría de seguridad (Word/PDF).
- Matriz consolidada de vulnerabilidades con severidades CVSS.
- Paquete de evidencias técnicas organizado (`evidence.zip`).
- Presentación ejecutiva (PPTX).
- Hoja de ruta de remediación priorizada.
- Documento de conclusiones y estado final del proyecto.

## 2.4 Definición de Done (DoD)

La **Definición de Hecho (Definition of Done)** establece los criterios obligatorios que determinan cuándo una historia de usuario se considera completamente finalizada dentro del proyecto de pentesting. Su aplicación garantiza que cada vulnerabilidad identificada cuente con evidencia verificable, pasos reproducibles, documentación formal de la PoC y un análisis claro de impacto, cumpliendo los estándares técnicos, éticos y académicos del proyecto.

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
### Objetivos del sprint  

Identificar y documentar de manera reproducible la superficie de ataque pública del cliente **TutorMatch** (entorno de staging o host/VM autorizado), incluyendo dominios, subdominios, hosts, puertos, servicios y endpoints de autenticación.  
Generar un inventario que guíe la fase de enumeración en el siguiente sprint y garantizar el cumplimiento de las **Rules of Engagement (ROE)** antes de cualquier explotación.

### Historias de usuario atendidas  

- **US-01** – *Reconocimiento inicial y mapeo de superficie (2 SP)*  
  Como atacante externo, quiero identificar dominios/subdominios, rutas de login y formularios públicos de TutorMatch para delimitar la superficie de ataque.

- **US-12** – *Escaneo de puertos y servicios de red (5 SP)*  
  Como atacante, quiero mapear hosts, puertos y servicios detrás del despliegue de TutorMatch (servidor web, base de datos, servicios auxiliares).

- **US-08** – *Verificación de TLS y headers de seguridad (5 SP)*  
  Como auditor, quiero comprobar los mecanismos HTTPS/TLS y cabeceras de seguridad para asegurar el transporte y la mitigación de ataques web.

- **US-04** – *Enumeración de endpoints API (8 SP)*  
  Como atacante, quiero identificar endpoints REST y métodos HTTP expuestos por TutorMatch para detectar recursos sin protección.

### Actividades realizadas  

Todas las actividades se ejecutaron **únicamente en el entorno autorizado** y tras la confirmación del **ROE**.  
Las salidas sensibles fueron sanitizadas antes de su almacenamiento público.

1. **Preparación del entorno de pruebas**  
   - Configuración de Kali Linux y estructura de trabajo (`~/securalabs/tutormatch/sprint1/`).
   - Creación de cuentas de prueba (roles *student* / *tutor*).  
   - Captura de evidencia (`prep_evidence.txt` con hostname, IP, uname -a).

2. **OSINT para TutorMatch**  
   - Búsqueda de dominios/subdominios con *theHarvester*, *Google Dorks*, *Archive.org*, *crt.sh*, *whois*.  
   - Identificación de endpoints externos (landing, api, CDN).  
   - Evidencias en `evidence/osint/`.

3. **Descubrimiento de red y hosts**  
   - *netdiscover / arp-scan* (si aplica) y `nmap -sn`.  
   - Evidencias: `evidence/discovery/discovery.txt`.

4. **Escaneo de puertos y servicios**  
   - `nmap -p- -T4 <target>` → puertos abiertos.  
   - `nmap -sV` → versiones y fingerprinting.  
   - Archivos: `nmap_full_ports.txt`, `nmap_sV.txt`.

5. **Descubrimiento web**
   - *gobuster* o *ffuf* → rutas públicas.  
   - *whatweb* → fingerprint tecnológico.  
   - Resultados en `evidence/web/`.

6. **Verificación TLS y cabeceras HTTP**  
   - *testssl.sh* + `curl -I`.  
   - Resultados: `tls_headers.txt`, `testssl_tutormatch.log`.

### Resultados y evidencias  

#### Resultados:
Durante el Sprint 1 se logró identificar la superficie de ataque inicial del entorno de pruebas de TutorMatch, delimitando los activos expuestos y generando el inventario técnico base para la fase de enumeración.
Los escaneos OSINT y de red permitieron mapear correctamente los hosts accesibles y reconocer la estructura pública de la aplicación web. A través del uso de herramientas como theHarvester, dnsenum y Google Dorks, se detectaron subdominios válidos y endpoints potenciales asociados al dominio principal tutormatch-server-test.netlify.app, confirmando que el despliegue activo correspondía a una instancia de staging alojada en la infraestructura de Netlify.

El escaneo de red con Nmap reveló la presencia de servicios HTTP/HTTPS activos en los puertos estándar (80 y 443), con respuesta positiva a los paquetes ICMP y detección correcta del sistema operativo basado en Linux. No se evidenciaron servicios adicionales en ejecución ni puertos de bases de datos o servicios internos expuestos públicamente, lo que sugiere una configuración de red básica y relativamente segura.

Mediante el análisis web con WhatWeb y Gobuster, se identificaron directorios accesibles como /api, /login y /uploads, que posteriormente servirán para las pruebas de enumeración y vulnerabilidades del Sprint 2. Los resultados del análisis TLS, realizados con testssl.sh, confirmaron la presencia de certificados válidos y un canal HTTPS funcional, aunque se observaron ausencias de cabeceras de seguridad complementarias (como Content-Security-Policy y X-Frame-Options), que representan vectores de riesgo bajo a medio.

En general, el sprint permitió establecer las bases técnicas del pentest, generando un mapa claro de dominios, servicios y tecnologías utilizadas por la plataforma. Toda la información obtenida se consolidó en la carpeta /evidence/sprint1/, sirviendo como punto de partida para la identificación de vulnerabilidades específicas en el siguiente sprint.

#### Evidencias:
- **Preparación del entorno de pruebas:**
<img src="assets/sprint_1/preparacion.PNG" alt="preparacion-sprint1"/>
**archivo prep_evidence.txt:**
<img src="assets/sprint_1/preptxt.PNG" alt="preparacion-TXT"/>

- **OSINT para TutorMatch:**
  - theHarvester:
  <img src="assets/sprint_1/theHarvester.PNG" alt="theHarvester"/>

  - Dnsenum:
  <img src="assets/sprint_1/dnsenum.PNG" alt="Dnsenum"/>

- **Descubrimiento de red y hosts:**
  - netdiscover: Se usa Host por el hecho de que es una web pública y no netdiscover/arp-scan que son para redes locales
  <img src="assets/sprint_1/host.PNG" alt="Host"/>

  Host_resolution.txt:
  tutormatch-server-test.netlify.app has address 54.232.119.62
  tutormatch-server-test.netlify.app has IPv6 address 2600:1f1e:7c1:c300::258
  tutormatch-server-test.netlify.app has HTTP service bindings 1 . alpn="h2"

- **Escaneo inicial de puertos/servicios:**
  - Ping / host discovery (útil si objetivo responde ICMP): nmap -Pn -sn -oN evidence/discovery/nmap_ping_scan.txt tutormatch-server-test.netlify.app
  <img src="assets/sprint_1/nmap.PNG" alt="Nmap"/>

  - Escaneo rápido de puertos (top 1000 + versión): nmap -Pn -sS -T4 --top-ports 1000 -oN evidence/scans/nmap_top1000.txt tutormatch-server-test.netlify.app
  <img src="assets/sprint_1/nmap2.PNG" alt="Nmap2"/>

  - Escaneo de todos los puertos (más lento) + detección de versiones + OS fingerprint (si aplica): nmap -Pn -p- -T4 -sV -O -oA evidence/scans/nmap_full tutormatch-server-test.netlify.app
  <img src="assets/sprint_1/nmap3.PNG" alt="Nmap3"/>

- **Descubrimiento web:**
  - Gobuster (directorios): gobuster dir -u https://tutormatch-server-test.netlify.app -w /usr/share/wordlists/dirb/common.txt -t 50 -o evidence/web/gobuster_dirs.txt
  <img src="assets/sprint_1/gobuster.PNG" alt="Gobuster"/>

  - ffuf: ffuf -u https://tutormatch-server-test.netlify.app/FUZZ -w /usr/share/wordlists/dirb/common.txt -o evidence/web/ffuf_dirs.json
  <img src="assets/sprint_1/ffuf.PNG" alt="Ffuf"/>

- **Primera versión TLS/cabeceras HTTP:**
  - Revisar cabeceras HTTP: curl -I -L https://tutormatch-server-test.netlify.app/login > evidence/web/tls_headers.txt
  <img src="assets/sprint_1/curl1.PNG" alt="Curl"/>

  - Test TLS: ./testssl.sh --logfile evidence/web/testssl_tutormatch.log https://tutormatch-server-test.netlify.app
  <img src="assets/sprint_1/testssl.PNG" alt="TestSSL"/>

### Retrospectiva del sprint 

**Lo que funcionó**
- Preparación del entorno organizada y reproducible.  
- Cobertura OSINT completa.  
- Escaneos bien documentados.  
- Flujo colaborativo entre los miembros vía GitHub.

**Qué no funcionó**
- Inconsistencia en nombres de archivos.  
- Dudas sobre el alcance de Netlify.  
- Formato de evidencia no estandarizado (faltaron XML/CSV).  
- Escaneos demorados y evidencias visuales desiguales.

**Lecciones aprendidas**
- Aplicar estrategia escalonada para *Nmap*.  
- Registrar autorizaciones ROE antes de pruebas agresivas.  
- Estandarizar nombres desde el inicio (`YYYYMMDD_tool_target.ext`).  
- Automatizar tareas repetitivas con scripts.

**Acciones de mejora**
| Acción | Responsable | Plazo | Entregable |
|--------|--------------|--------|-------------|
| Estandarizar convención de nombres | Piero | 3 días | `EVIDENCE_CONVENTION.md` |
| Crear scripts de automatización (OSINT / Nmap) | Leonardo & Fabio | 5 días | `scripts/run_nmap_safe.sh` |
| Formalizar autorización y alcance (ROE) | Harold | Inmediato | `authorization_email.txt` |
| Plantilla PoC y guía de capturas | Piero | 4 días | `templates/poc_template.md` |
| Optimizar estrategia de escaneo | Leonardo | 5 días | `run_nmap_safe.sh` |
| Peer-review de hallazgos | Fabio | Sprint 2 | Checklist de revisión |

**Métricas del sprint**
- ≥ 1 commit por integrante.  
- ≥ 90 % de evidencias renombradas según convención.  
- Scripts automatizados en repositorio.  
- Plantilla PoC adoptada.

## Sprint 2 – Enumeración y Vulnerabilidades

### Historias de usuario atendidas  

- **US-04 – Enumeración de endpoints API (8 SP):** Como atacante, quiero identificar todos los endpoints REST y métodos HTTP expuestos por TutorMatch para detectar recursos sin protección.
- **US-09 – Detección de exposición de datos sensibles (8 SP):** Como pentester, quiero revisar respuestas de la API y endpoints públicos para detectar tokens, correos o información sensible no enmascarada.
- **US-03 – Pruebas de Cross-Site Scripting (XSS) (13 SP):** Como atacante, quiero insertar scripts maliciosos en los campos de entrada y formularios de TutorMatch para validar la sanitización y filtrado de entradas de usuario.
- **US-05 – Explotación de credenciales débiles y recuperación de cuenta (8 SP):** Como pentester, quiero evaluar contraseñas débiles, políticas de bloqueo y el flujo de recuperación de cuentas para detectar posibles riesgos de takeover.
- **US-06 – Prueba de subida de archivos inseguros (5 SP):** Como pentester, quiero probar la carga de archivos con extensiones o contenidos no permitidos para verificar la validación y el control de tipo MIME implementado.
- **US-08 – Verificación de TLS y headers de seguridad (5 SP):** Como auditor, quiero comprobar los mecanismos HTTPS/TLS y los encabezados de seguridad (CSP, HSTS, X-Frame-Options, X-XSS-Protection) para asegurar el transporte y la mitigación de vectores web.
- **US-12 – Escaneo de puertos y servicios de red (5 SP):** Como atacante, quiero mapear los hosts, puertos y servicios detrás del despliegue de TutorMatch (servidor web, base de datos, servicios auxiliares) para identificar configuraciones o versiones vulnerables.

### Actividades (Nessus, Nikto, análisis de endpoints API)  

1. **Preparación del entorno**
   - Validación de ROE (`authorization_email.txt`).  
   - Cuentas de prueba autenticadas.  
   - Registro de versiones de herramientas (*Nessus*, *Nikto*, *ZAP*).

2. **Escaneo de vulnerabilidades web – Nessus**
   - Política “no destructiva”: CVE, TLS, HTTP.  
   - Reportes `.nessus` y `.pdf` → `/evidence/sprint2/nessus/`.

3. **Escaneo no intrusivo – Nikto**
   - Detección de cabeceras y rutas sensibles.  
   - Resultados → `/evidence/sprint2/nikto/`.

4. **Enumeración web**
   - *Gobuster / ffuf* → `/api/`, `/uploads/`, `/admin/`.  
   - *WhatWeb* → frameworks y librerías detectadas.

5. **Detección de endpoints API (ZAP / Burp / Postman)**
   - Spidering controlado y extracción de *OpenAPI fragments*.  
   - Colección Postman: `postman_collection_tutormatch.json`.

6. **Verificación de métodos HTTP y CORS**
   - `curl -X OPTIONS` y cabeceras de seguridad.

7. **Consolidación de hallazgos preliminares**
   - `findings_prelim.csv` con severidad, PoC y responsable.

### Resultados y evidencias  

#### Resultados:

Durante el Sprint 2, el equipo SecuraLabs logró consolidar un proceso sistemático de enumeración de servicios, endpoints y vulnerabilidades preliminares en el entorno autorizado de TutorMatch, aplicando metodologías seguras y herramientas de análisis no destructivas. A partir del escaneo realizado con Nessus, Nikto y WhatWeb, se identificaron múltiples componentes web activos y configuraciones susceptibles de mejora en materia de seguridad.

El escaneo con Nessus permitió detectar vulnerabilidades de baja y media severidad, principalmente relacionadas con la falta de cabeceras de seguridad HTTP y configuraciones SSL/TLS parcialmente optimizadas. No se encontraron vulnerabilidades críticas ni de ejecución remota, lo cual indica una arquitectura estable en términos de exposición de servicios. Paralelamente, el análisis de Nikto reveló la presencia de rutas y archivos sensibles (por ejemplo, /uploads/ y /backup/) que, aunque no contenían datos visibles, representan vectores potenciales de acceso indebido si no se controlan adecuadamente.

En la fase de enumeración web y API, el uso de Gobuster y ZAP permitió mapear endpoints REST relevantes, como /api/v1/users y /api/v1/login, además de descubrir métodos HTTP habilitados (GET, POST, OPTIONS) y políticas CORS permisivas en algunos recursos. La colección de solicitudes en Postman facilitó la verificación manual de los endpoints autenticados, confirmando que el flujo de acceso de usuarios se encuentra protegido mediante tokens válidos y con controles básicos de sesión.

Asimismo, el análisis TLS y de cabeceras evidenció que el servidor mantiene certificados válidos, aunque carece de cabeceras de seguridad complementarias como X-Frame-Options, Strict-Transport-Security o Content-Security-Policy. Estos hallazgos, si bien no constituyen vulnerabilidades críticas, se consideran áreas de mejora dentro de las buenas prácticas OWASP.

Finalmente, la consolidación de hallazgos preliminares permitió clasificar y priorizar cada vulnerabilidad en un archivo findings_prelim.csv, asignando niveles de severidad según CVSS y responsables de verificación por integrante del equipo. Esta organización de evidencias facilitó la trazabilidad y sirvió como insumo directo para el Sprint 3, enfocado en pruebas de explotación controlada.

En conclusión, el Sprint 2 permitió identificar debilidades técnicas de configuración y exposición web, validar la correcta aplicación de políticas de seguridad en la API, y fortalecer la base documental del proceso de pentesting. Los resultados confirman un progreso significativo en la comprensión estructural del sistema y preparan el terreno para la validación práctica de vulnerabilidades en la siguiente etapa del proyecto.

#### Evidencias:

- **Preparación del entorno de pruebas:**
<img src="assets/sprint_2/prep.PNG" alt="Preparacion-Sprint2"/>
<img src="assets/sprint_2/preptxt.PNG" alt="Preparacion-TXT"/>

- **Escaneo de vulnerabilidades web (Nessus):**
<img src="assets/sprint_2/nessus.PNG" alt="Nessus"/>

- **Escaneo web no intrusivo (Nikto):** nikto -host "https://$TARGET" -output "$BASE/nikto/${DATE}_nikto_${TARGET}.txt"
<img src="assets/sprint_2/nikto.PNG" alt="Nikto"/>

- **Descubrimiento web y enumeración de directorios:** ffuf -u "https://$TARGET/FUZZ" -w /usr/share/wordlists/dirb/common.txt -t 30 -mc 200,301,302,403 -o "$BASE/web_enumeration/${DATE}_ffuf_dirs_${TARGET}.json" -of json
<img src="assets/sprint_2/ffuf.PNG" alt="Ffuf-Sprint2"/>

- **Detección de endpoints API (OWASP ZAP / Burp / Postman):**
<img src="assets/sprint_2/zap.PNG" alt="Owasp Zap"/>

<img src="assets/sprint_2/zap2.PNG" alt="Zap PDF"/>

- **Verificación de métodos HTTP, CORS y cabeceras (OPTIONS / curl):** curl -i -X OPTIONS "https://$TARGET/login" > "$BASE/http_options/${DATE}_options_${TARGET}.txt"
curl -I -L "https://$TARGET/login" > "$BASE/http_options/${DATE}_headers_login.txt"
<img src="assets/sprint_2/curl.PNG" alt="Curl"/>

- **Metagoofil + exiftool (OSINT de documentos públicos):**
<img src="assets/sprint_2/metagoofil.PNG" alt="Metagoofil"/>

### Retrospectiva  

**Lo que funcionó**
- Las herramientas se ejecutaron de forma controlada y con autorización documentada (ROE firmado), cumpliendo el criterio ético del proyecto.  
- Se estandarizó correctamente la estructura de carpetas y nombres de evidencia (/evidence/sprint2/), lo que agilizó la consolidación de resultados.  
- El uso combinado de Nessus, Nikto y OWASP ZAP permitió obtener hallazgos reproducibles y validados con un enfoque no destructivo. 
- La colección Postman generada a partir del spider de ZAP facilitó la detección de endpoints REST y la preparación del backlog para el Sprint 3.
- Se redujeron falsos positivos gracias al filtrado manual y revisión cruzada entre Leonardo y Fabio.

**Qué no funcionó**
- Nessus presentó lentitud durante el análisis TLS y algunos plugins fueron omitidos por timeout, afectando la cobertura del reporte.  
- Nikto arrojó varios falsos positivos en encabezados por la naturaleza del hosting (Netlify), requiriendo verificación manual.
- No se logró obtener el archivo swagger.json completo, solo fragmentos parciales (OpenAPI), lo que limitó el mapeo total de la API.
- Las pruebas XSS reflejadas debieron repetirse con autenticación para obtener resultados más concluyentes.

**Lecciones aprendidas**
- Planificar escaneos largos (Nessus/Nikto) en ventanas horarias de baja latencia para optimizar el tiempo de ejecución.
- Verificar previamente el hosting (Netlify) para evitar bloqueos automáticos ante múltiples requests. 
- Consolidar los resultados en formato CSV desde el inicio y no al final del sprint para facilitar priorización CVSS.
- Utilizar capturas con metadatos (fecha, comando) para mejorar la trazabilidad de evidencias.

**Acciones de mejora**
| Acción | Responsable | Plazo | Entregable |
|--------|--------------|--------|-------------|
| Optimizar política de escaneo Nessus y desactivar plugins innecesarios | Leonardo | 2 días | `policy_safe_scan_v2.nessus` |
| Validar hallazgos de Nikto con curl/Burp y marcar falsos positivos | Fabio | 3 días | `findings_validated.csv` |
| Completar documentación de endpoints en Postman con autenticación | Harold | 3 días | `postman_collection_v2_auth.json` |
| Estandarizar formato CSV para hallazgos (ID, severidad, endpoint, CVSS, PoC) | Piero | 2 días | `docs/findings_template.csv` |

**Métricas del sprint**
- ≥ 95 % de hallazgos validados con evidencia adjunta.
- Al menos 1 PoC por tipo de vulnerabilidad confirmada (XSS, exposición de datos, auth).
- Reducción de ≥ 30 % en falsos positivos respecto al Sprint 2.  
- Política Nessus optimizada y reutilizable para Sprint 3.

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

## 4.1. Matriz de vulnerabilidades

| ID | Descripción | CVSS (Base estimado) | Impacto |
|----|-------------|----------------------:|---------|
| VULN-001 | Exposición de archivos sensibles (`.bashrc`, `.bash_history`, `.archive`, `.assets`) accesibles públicamente detectados por fuzzing (`ffuf`). | **5.3** | Divulgación de información sensible que facilita reconocimiento y pivoteo; posible revelación de endpoints, rutas o secretos que aumentan la probabilidad de ataques posteriores. |
| VULN-002 | Cross-Site Scripting (XSS) reflejado: entradas que devuelven contenido sin sanitizar (PoC documentada). | **6.1** | Robo de cookies/tokens, ejecución de acciones en nombre del usuario autenticado y pérdida de confianza en la plataforma. |
| VULN-003 | API / endpoints expuestos sin controles claros de autenticación/autorization detectados por enumeración (Postman / ffuf / spider). | **8.0** | Exposición de PII, posibilidad de IDOR y operaciones no autorizadas; facilita ataques encadenados y puede comprometer la plataforma. |
| VULN-004 | Cabeceras de seguridad y TLS incompletas o mal configuradas (ausencia/deficiencia de CSP, HSTS, X-Frame-Options; parámetros TLS a revisar). | **4.3** | Incrementa riesgo de ataques complementarios (clickjacking, downgrade, facilitan XSS); afecta cumplimiento y confianza del sitio. |

## 4.2. Evidencias técnicas (pantallazos, logs, outputs)

## 4.3. Impacto en el negocio

Los hallazgos identificados durante las pruebas representan riesgos relevantes para TutorMatch en aspectos técnicos y reputacionales. La exposición de endpoints y APIs sin controles de acceso (**VULN-003**) supone el riesgo más alto, ya que podría permitir el acceso o modificación de información de usuarios, afectando la confidencialidad y generando pérdida de confianza en la plataforma. El **XSS reflejado (VULN-002)** también representa un impacto importante, pues podría ser aprovechado para robar sesiones o ejecutar código malicioso en los navegadores de los usuarios. Por otro lado, la **exposición de archivos sensibles (.bash_history o .bashrc) (VULN-001)** facilita el reconocimiento del entorno y la obtención de información útil para otros ataques. Finalmente, la **falta de cabeceras de seguridad y configuraciones TLS adecuadas (VULN-004)** incrementa la superficie de ataque ante técnicas como clickjacking o degradación de conexión. En conjunto, estas vulnerabilidades pueden afectar la integridad y confidencialidad de los datos, comprometer la estabilidad del servicio y disminuir la percepción de seguridad de los usuarios. Se recomienda priorizar la protección de APIs, la corrección del XSS y el aseguramiento de los archivos y cabeceras para reducir el riesgo general del sistema.

---

# Capítulo V: Recomendaciones y Plan de Mitigación

## 5.1 Recomendaciones técnicas
- Patching, WAF, hardening  

## 5.2 Recomendaciones organizacionales
- Capacitación, políticas  

## 5.3 Priorización por impacto / urgencia

---

# Capítulo VI: Conclusiones y Recomendaciones

Conclusiones y recomendaciones del equipo
El proyecto de auditoría y pentesting realizado sobre la plataforma TutorMatch permitió aplicar de forma práctica la metodología ágil y los marcos de referencia de seguridad (Scrum, PTES y OWASP) en un entorno web real. A través de las fases de reconocimiento, enumeración, explotación controlada y análisis de resultados, se logró identificar vulnerabilidades con distintos niveles de severidad que podrían afectar la confidencialidad, integridad y disponibilidad de los datos.

Los hallazgos más relevantes se concentraron en la exposición de endpoints y APIs sin controles de acceso adecuados, la presencia de un XSS reflejado en el frontend, la exposición de archivos sensibles del servidor y la falta de cabeceras y configuraciones TLS seguras. Estas vulnerabilidades evidencian la necesidad de fortalecer los mecanismos de autenticación, sanitización de entradas y políticas de seguridad web para garantizar un entorno más robusto.

El trabajo en equipo bajo un enfoque ágil permitió distribuir responsabilidades, planificar actividades por sprints y documentar cada etapa con evidencias técnicas claras. Este proceso favoreció no solo la identificación de riesgos, sino también la generación de recomendaciones viables que podrían incorporarse en el ciclo de desarrollo de la aplicación, alineándose con la filosofía DevSecOps.

En conclusión, el proyecto demostró la importancia de integrar la seguridad desde las primeras fases del desarrollo, realizar evaluaciones periódicas de vulnerabilidades y mantener prácticas de mejora continua. Con la implementación de las medidas propuestas, TutorMatch podrá reducir significativamente su superficie de ataque, fortalecer la confianza de sus usuarios y sentar las bases para un modelo de gestión de seguridad sostenible en el tiempo.

---

# Bibliografía

OffSec Services Limited. (s. f.). nmap — Kali Linux Tools. Recuperado el 25 de octubre de 2025, de https://www.kali.org/tools/nmap/

OffSec Services Limited. (s. f.). gobuster — Kali Linux Tools. Recuperado el 25 de octubre de 2025, de https://www.kali.org/tools/gobuster/

OffSec Services Limited. (s. f.). ffuf — Kali Linux Tools. Recuperado el 25 de octubre de 2025, de https://www.kali.org/tools/ffuf/

OffSec Services Limited. (s. f.). hydra — Kali Linux Tools. Recuperado el 25 de octubre de 2025, de https://www.kali.org/tools/hydra/

OffSec Services Limited. (s. f.). nikto — Kali Linux Tools. Recuperado el 25 de octubre de 2025, de https://www.kali.org/tools/nikto/

---

# Anexos

- Registro de User Stories  
- Product Backlog y Sprint Backlogs  
- Evidencias de cada sprint (capturas, reportes de herramientas)  
- Scripts y código  
- Registro de retrospectivas  
