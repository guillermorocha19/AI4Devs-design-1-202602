# LTI ATS - Registro de Prompts

## Prompt 1 - Fase 1: Investigación y Análisis de Mercado

**Fecha:** 2026-04-04
**Rol asignado:** Experto en producto con experiencia en sistemas ATS
**Fase:** Investigación y análisis de mercado

**Prompt del usuario:**
```
LTI es una startup que quiere desarrollar el ATS (Applicant-Tracking System) del futuro. Para ello, vamos a generar una primera documentación de un sistema software que incluirá el resultado de las fases de investigación y análisis de mercado, casos de uso, modelado de datos y diseño a alto nivel. Para ello, seguirás las siguientes instrucciones:
- Irás tomando diferentes roles según la fase en la que nos encontremos
- Yo y solo yo te iré indicando cuando pasar a la siguiente fase
- Al inicio de cada fase indicaré el rol, contexto y output esperado
- Como instrucción general, pregunta siempre que lo necesites para alcanzar tu objetivo.
- Iremos confeccionando un único fichero en formato MarkDown donde iremos añadiendo los outputs de cada fase
- Muestrame un draft del fichero antes de dar por terminada una fase
- Ve generando otro fichero donde ir almacenando los prompts que usemos en esta conversación

Vamos con la primera fase: investigación y análisis de mercado.
Eres un experto en producto con experiencia en sistemas ATS. Para conseguir el output de esta fase deberás contestar estas preguntas (e investigar al respecto, basándote en ellas):
- ¿Qué funcionalidades básicas tiene un sistema ATS? Descríbelas en un listado, y ordena de mayor a menor prioridad.
- ¿Qué beneficios obtiene una empresa de un sistema ATS para considerar su uso? ¿Y un candidato?
- ¿Qué alternativas tiene a usar un sistema ATS y cuando pueden ser relevantes?
- ¿Cómo es el customer journey normal de un cliente que usa un sistema ATS? Descríbeme paso a paso todas las interacciones

Outputs de esta fase:
- Iniciar el documento con descripción breve del software LTI, valor añadido y ventajas competitivas.
- Explicación de las funciones principales.
- Un diagrama Lean Canvas para entender el modelo de negocio (en formato Mermaid)
```

**Acciones del asistente:**
- Búsquedas web realizadas:
  1. "ATS applicant tracking system features 2025 2026"
  2. "ATS alternatives spreadsheets manual hiring"
  3. "customer journey hiring manager ATS workflow steps"
- Generación del documento principal con secciones 1-3
- Generación del fichero de prompts

**Output generado:**
- Sección 1: Introducción (descripción, valor añadido, ventajas competitivas)
- Sección 2: Investigación y Análisis de Mercado (funcionalidades, beneficios, alternativas, customer journey)
- Sección 3: Lean Canvas en formato Mermaid

---

## Prompt 2 - Fase 1: Modificaciones

**Fecha:** 2026-04-04
**Fase:** Investigación y análisis de mercado (revisión)

**Prompt del usuario:**
```
Modificaciones sobre fase 1
- Elimina la parte de "Alternativas al uso de un ATS" del documento, es parte del análisis, no de la documentación final
- Como consideramos al candidato un cliente, genera un customer journey para el candidato también
```

**Acciones del asistente:**
- Eliminación de la sección 2.3 "Alternativas al uso de un ATS"
- Renumeración de secciones (2.4 → 2.3 Customer Journey del Cliente)
- Creación de nueva sección 2.4 "Customer Journey del Candidato" con 10 fases
- Actualización del fichero de prompts

---

## Prompt 3 - Fase 2: Casos de Uso (pregunta de clarificación)

**Fecha:** 2026-04-04
**Rol asignado:** Product Manager Senior + Analista Senior (para UML)
**Fase:** Casos de uso y PRDs

**Prompt del usuario:**
```
Vamos a la fase 2. Ahora eres un Product Manager Senior. Desarrolla un PRD (Product Requirements Document) para los tres principales casos de uso (los tres primeros puntos del listado "Funcionalidades Básicas de un Sistema ATS"), basándote en la información existente en el documento. No añadas nada nuevo que no aparezca en la descripción original. Si necesitas contexto, pregúntame. Una vez que lo tengas necesitarás además la ayuda de un Analista Senior para generar un diagrama UML para cada caso de uso.
Outputs de esta fase, por cada caso de uso:
- PRD completo
- Diagrama UML (en formato PlantUML)
```

**Preguntas de clarificación realizadas:**
1. Nivel de detalle de los PRDs → Respuesta: Detalle completo (stories + acceptance criteria + edge cases + restricciones técnicas)
2. Actores principales para los diagramas UML → Respuesta: Reclutador + Candidato + Sistema

**Acciones del asistente:**
- Revisión del documento existente (secciones 2.1, 2.3, 2.4) para extraer contexto sin añadir información nueva
- Generación de 3 PRDs completos con: información general, objetivos, user stories con criterios de aceptación, edge cases, restricciones técnicas
- Generación de 3 diagramas UML de casos de uso en formato PlantUML
- Actualización del fichero de prompts

**Output generado:**
- Sección 4: Casos de Uso Principales — PRDs
  - PRD-001: Publicación y Distribución de Ofertas de Empleo (5 user stories)
  - PRD-002: Parsing y Almacenamiento de CVs (5 user stories)
  - PRD-003: Screening y Filtrado Automatizado de Candidatos (5 user stories)
- 3 diagramas PlantUML (uno por caso de uso)

---

## Prompt 4 - Fase 2: Modificaciones sobre PRDs

**Fecha:** 2026-04-04
**Fase:** Casos de uso y PRDs (revisión)

**Prompt del usuario:**
```
Modificaciones sobre fase 2:
- US-001.2 : elimina los ejemplos de portales, crea ambigüedad
- Añade por cada PRD una sección más "puntos abiertos" (ejemplo: lista final de portales que estarán disponibles o redes sociales a conectar)
- US-002.1 tiene dos US encubiertas, separalas ya que una será para adjuntar un CV y otra para conectar el perfil de LinkedIn
```

**Acciones del asistente:**
- Eliminación de ejemplos de portales (LinkedIn, Indeed, Glassdoor, etc.) en US-001.2
- Separación de US-002.1 en dos user stories: US-002.1 (Envío de CV) y US-002.2 (Importación de perfil desde LinkedIn)
- Renumeración de US del PRD-002 (ahora 6 user stories en lugar de 5)
- Actualización del diagrama UML del PRD-002 para reflejar los dos casos de uso separados
- Adición de sección "Puntos Abiertos" a cada PRD:
  - PRD-001: 5 puntos abiertos (portales, redes sociales, career page, límites por plan, SLA)
  - PRD-002: 6 puntos abiertos (formatos, idiomas NLP, integración LinkedIn, duplicados, retención, OCR)
  - PRD-003: 6 puntos abiertos (modelo IA, formatos killer questions, auditoría sesgos, feedback, recálculo, límites)

---

## Prompt 5 - Fase 3: Modelado de Datos

**Fecha:** 2026-04-04
**Rol asignado:** Arquitecto de Software
**Fase:** Modelado de datos

**Prompt del usuario:**
```
Vamos a la fase 3: modelado de datos.
Rol: ahora eres un brillante arquitecto de software. Eres capaz de diseñar, explicar y diagramar los diferentes aspectos de un sistema de software. Basándote única y exclusivamente en la documentación generada hasta ahora, diseña un completo modelo de datos que incluya entidades, atributos (nombre y tipo) y relaciones. Usa el estándar Diagramas Entidad-Relación (ER).
Output de esta fase: diagrama con el modelado de datos en formato Mermaid
```

**Acciones del asistente:**
- Revisión exhaustiva de toda la documentación existente (secciones 1-4)
- Identificación de 17 entidades con sus atributos y tipos de datos
- Definición de relaciones con cardinalidades (1:1, 1:N, M:N)
- Generación del diagrama ER en formato Mermaid
- Documentación de decisiones de diseño con trazabilidad a secciones del documento

**Entidades identificadas:**
- Organizativas: Empresa, Reclutador
- Oferta y publicación: OfertaEmpleo, EtapaPipeline, PortalEmpleo, Publicacion
- Candidato y perfil: Candidato, CV, PerfilEstructurado, ExperienciaLaboral, FormacionAcademica, Competencia, IdiomaCandidato
- Candidatura: Candidatura
- Screening: CriterioScreening, KillerQuestion, RespuestaKillerQuestion, ScoringDetalle
- Transversales: Notificacion, AuditTrail

**Output generado:**
- Sección 5: Modelado de Datos (descripción, diagrama ER Mermaid, notas de diseño)

---

## Prompt 6 - Fase 3: Preguntas y modificaciones sobre modelo de datos

**Fecha:** 2026-04-04
**Fase:** Modelado de datos (revisión)

**Prompt del usuario:**
```
Modificaciones (y preguntas) sobre fase 3:
- Añade auditoría al modelo completo para registrar información detallada que responda a quién, qué, cuándo, dónde y cómo se modificaron o consultaron los datos.
- Añade a ScoringDetalle información para conocer con qué modelo LLM se ha calculado
Preguntas
- Justifícame por qué es necesaria la entidad "Empresa"
- Si solo te centras en los PRDs de este documento, ¿identificas alguna optimización del modelo?
```

**Acciones del asistente (respuesta a preguntas):**
- Justificación de la entidad Empresa: multitenancy SaaS, career page/branding, aislamiento de datos
- Optimizaciones identificadas:
  1. IdiomaCandidato y FormacionAcademica → campos JSON en PerfilEstructurado (no participan en screening de PRDs)
  2. PortalEmpleo unificado con redes sociales via campo `tipo`

## Prompt 7 - Fase 3: Confirmación y aplicación de cambios

**Fecha:** 2026-04-04
**Fase:** Modelado de datos (aplicación de cambios)

**Prompt del usuario:**
```
Ok a las respuestas. Haz las modificaciones solicitadas + optimizaciones
```

**Acciones del asistente:**
- AuditTrail → AuditLog: nueva entidad con campos 5W (actor_id, actor_tipo, accion, entidad, entidad_id, datos_antes, datos_despues, motivo, ip_origen, user_agent, fecha). Desvinculada de Candidatura para ser transversal a todo el sistema.
- ScoringDetalle: añadidos campos modelo_llm, version_modelo_llm y fecha_calculo
- PortalEmpleo → CanalPublicacion: renombrado con campo tipo (job_board/red_social) unificando US-001.2 y US-001.3
- IdiomaCandidato eliminada → campo json idiomas en PerfilEstructurado
- FormacionAcademica eliminada → campo json formacion_academica en PerfilEstructurado
- Eliminadas relaciones obsoletas y actualizadas notas del modelo
- Modelo resultante: 15 entidades (antes 17)

---

## Prompt 8 - Fase 4: Diseño de Arquitectura

**Fecha:** 2026-04-04
**Rol asignado:** Arquitecto de Software Senior
**Fase:** Diseño de arquitectura a alto nivel

**Prompt del usuario:**
```
Fase 4: diseño de la arquitectura
Eres un experto arquitecto software con muchos años de experiencias en el diseño de arquitectura de sistemas como este. Analiza toda la documentación disponible y, basándote sólo y exclusivamente en esta información, diseña el sistema a un alto nivel, añadiendo además por qué has tomado las diferentes decisiones de arquitectura y generando un diagrama simple pero con mucha fuerza visual.
Output: documentación actualizada + diagrama de la arquitectura en formato Mermaid
```

**Acciones del asistente:**
- Revisión completa de toda la documentación (secciones 1-5) para identificar drivers arquitectónicos
- Identificación de 14 requisitos del documento que derivan en decisiones de arquitectura
- Formulación de 6 ADRs (Architecture Decision Records) resumidos
- Diseño de arquitectura en 7 capas con justificación trazada al documento
- Generación de diagrama Mermaid con estilo visual diferenciado por capa

**Drivers arquitectónicos identificados:**
- API-first (sección 1.3) → API Gateway
- Multitenancy SaaS (Lean Canvas) → Row-Level Security
- Procesamiento asíncrono x3 PRDs → Cola de mensajes central
- NLP/LLM con trazabilidad (PRD-002, PRD-003, modelo datos) → Gateway LLM
- Búsqueda full-text < 1s (PRD-002) → Motor de búsqueda dedicado
- Career page < 2s (PRD-001) → CDN
- Cifrado + GDPR (PRD-002, sección 2.1) → Object Storage cifrado
- Tiempo real (sección 1.2, CJ candidato) → WebSockets
- Auditoría 5W (modelo datos) → Middleware transversal

**Output generado:**
- Sección 6: Diseño de Arquitectura a Alto Nivel
  - 6.1 Visión General (tabla requisito → driver → decisión)
  - 6.2 ADRs resumidos (6 decisiones de arquitectura)
  - 6.3 Diagrama de Arquitectura (Mermaid con 7 capas y estilos visuales)
  - 6.4 Descripción de Componentes (detalle por capa con trazabilidad)

---

## Prompt 9 - Fase 5: Modelo C4 de la Capa de Clientes

**Fecha:** 2026-04-04
**Rol asignado:** Arquitecto de Software Senior
**Fase:** Modelo C4 — Capa de Clientes

**Prompt del usuario:**
```
Última fase (fase cinco): Con el mismo rol de la fase anterior, ahora debes generar un modelo C4 completo, con todo detalle, en formato Structurizr DSL del componente "Capa de Clientes" (este es el output de esta fase)
```

**Acciones del asistente:**
- Revisión de la arquitectura (sección 6) para identificar los 4 contenedores de la Capa de Clientes
- Revisión de PRDs (sección 4) para derivar componentes internos de cada contenedor
- Revisión de customer journeys (secciones 2.3, 2.4) para mapear interacciones a componentes
- Revisión de restricciones técnicas para decisiones de tecnología por componente
- Generación del modelo C4 completo en Structurizr DSL con 4 niveles

**Descomposición generada:**
- L1 Context: 4 personas + 3 sistemas externos + LTI como sistema principal
- L2 Container: 4 contenedores (WebApp, Portal Candidato, Career Page, API Externa) + 3 backend de referencia
- L3 Component:
  - App Web Reclutador: 9 componentes (Ofertas, Pipeline Kanban, Explorador Candidatos, Screening Dashboard, Perfil Candidato, Analytics, Colaboración, Notificaciones, API Client)
  - Portal Candidato: 7 componentes (Aplicación, Status Tracker, Entrevistas, Ofertas Recibidas, Feedback, Onboarding, API Client)
  - Career Page: 5 componentes (Branding, Listado Ofertas, Detalle Oferta, CTA Aplicación, Generador Estático)
  - API Externa: 4 componentes (REST Endpoints, Webhooks, Auth, Documentación)
- L4 Code: 4 sub-componentes del Módulo de Aplicación (CV Uploader, LinkedIn Importer, Killer Questions Form, Application Orchestrator)
- 6 vistas definidas (1 Context, 1 Container, 4 Component)
- Estilos visuales diferenciados por tipo de elemento

**Output generado:**
- Sección 7: Modelo C4 — Capa de Clientes (Structurizr DSL + tabla de trazabilidad + notas de decisiones)
