# Histórico de Prompts — Revisión de Documentación LTI-GRG

## Prompt 1 — Instrucción inicial y carga del documento

> **Rol:** Eres un arquitecto de software senior y analista de sistemas con amplia experiencia en revisión de documentación técnica, modelado de negocio y diseño de bases de datos.
>
> **Contexto:** Se te proporcionará un documento que contiene la documentación inicial de un sistema software. Esta documentación abarca desde el modelo de negocio hasta el modelado de datos, pasando por todos los artefactos intermedios relevantes (requisitos, casos de uso, arquitectura, etc.).
>
> **Objetivo:** Analiza exhaustivamente el documento adjunto e identifica todos los gaps, ambigüedades e incoherencias presentes en la documentación. Para cada problema identificado, propón una o varias soluciones concretas y justificadas.
>
> **Definiciones clave:**
> - **Gap:** Información ausente o incompleta que debería estar presente en la documentación.
> - **Ambigüedad:** Elementos que pueden interpretarse de más de una manera o que carecen de precisión suficiente.
> - **Incoherencia:** Contradicciones o inconsistencias entre distintas partes del documento.
>
> **Instrucciones de comportamiento:** No presentes todos los hallazgos de una sola vez. Sigue este proceso iterativo:
>
> 1. Identifica y analiza todos los problemas internamente.
> 2. Preséntame **un único problema** a la vez, indicando: el tipo (gap, ambigüedad o incoherencia), la descripción del problema, dónde se localiza en el documento y tu propuesta de solución.
> 3. Espera mi respuesta antes de continuar con el siguiente problema. Puedo aceptar la solución, rechazarla, modificarla o pedir alternativas.
> 4. Una vez que hayamos resuelto ese punto, pasa al siguiente.
> 5. Al finalizar todos los puntos, presenta un resumen consolidado con todas las decisiones tomadas.
>
> **Formato de cada entrega:**
> ```
> 🔍 Problema [N] de [Total estimado]
> Tipo: [Gap / Ambigüedad / Incoherencia]
> Ubicación: [Sección o elemento del documento]
> Descripción: [Explicación clara del problema]
> Solución propuesta: [Propuesta concreta y justificada]
> ```

*Archivo adjunto: LTI-GRG.md (primera carga — fichero vacío/truncado)*

---

## Prompt 2 — Recarga del documento

*Archivo adjunto: LTI-GRG.md (segunda carga — fichero completo, 1794 líneas)*

---

## Prompt 3 — Decisión sobre Problema 1

> A, siguiente problema

*Decisión: Aceptada Opción A (perfil acumulativo con historial de versiones y merge aditivo)*

---

## Prompt 4 — Decisión sobre Problema 2

> Acepto, siguiente

*Decisión: Aceptadas las entidades Usuario, Entrevista, Scorecard, CriterioScorecard y Nota*

---

## Prompt 5 — Decisión sobre Problema 3

> Solo punto 1, siguiente

*Decisión: Aceptado solo punto 1 (declaración de alcance MVP + roadmap con prioridades), rechazado punto 2 (fichas de roadmap mínimas)*

---

## Prompt 6 — Decisión sobre Problema 4

> Lo apuntamos como punto abierto en la sección correspondiente. Siguiente

*Decisión: Registrado como punto abierto (modelo RBAC)*

---

## Prompt 7 — Decisión sobre Problema 5

> Acepto, siguiente

*Decisión: Aceptada entidad PlantillaNotificacion y campo plantilla_id en Notificacion*

---

## Prompt 8 — Decisión sobre Problema 6

> Acepto solo punto 1. Siguiente

*Decisión: Aceptado solo punto 1 (campos en_talent_pool y fecha_ingreso_talent_pool en Candidato), rechazado punto 2 (documentar en roadmap)*

---

## Prompt 9 — Decisión sobre Problema 7

> Añadirlo como punto abierto a la sección correspondiente. Siguiente.

*Decisión: Registrado como punto abierto (PA-001.6 — diagrama de estados de la oferta)*

---

## Prompt 10 — Decisión sobre Problema 8

> Acepto. siguiente

*Decisión: Aceptada separación de etapa_actual_id (flujo) y estado (administrativo con valores cerrados)*

---

## Prompt 11 — Decisión sobre Problema 9

> Acepto, siguiene

*Decisión: Aceptada eliminación de cv_id y creación de tabla OrigenPerfil*

---

## Prompt 12 — Decisión sobre Problema 10

> Ok solución propuesta, siguiente

*Decisión: Aceptada sección de Requisitos No Funcionales consolidada*

---

## Prompt 13 — Decisión sobre Problema 11

> Acepto propuesta, añade como punto abierto. siguiente

*Decisión: Aceptado como punto abierto (modelo de tenancy para agencias)*

---

## Prompt 14 — Decisión sobre Problema 12

> Ignoramos este gap para MVP. Siguiente

*Decisión: Descartado — GDPR simplificado se mantiene para MVP*

---

## Prompt 15 — Decisión sobre Problema 13

> Opción A. Siguiente

*Decisión: Aceptada Opción A (renombrar a "Nivel 3 detallado / sub-componentes")*

---

## Prompt 16 — Decisión sobre Problema 14

> Ok propuesta, enfatiza que es alto riesgo. Siguiente

*Decisión: Aceptada ampliación de PA-002.3 con nota de riesgo alto sobre LinkedIn*

---

## Prompt 17 — Decisión sobre Problema 15

> Acepto, siguiente

*Decisión: Aceptada ampliación de PA-003.4 con modelo de feedback completo*

---

## Prompt 18 — Decisión sobre Problema 16

> Acepto, siguiente

*Decisión: Aceptada categoría de Resiliencia y Continuidad en RNFs*

---

## Prompt 19 — Decisión sobre Problema 17

> Acepto solo punto 1, siguiente

*Decisión: Aceptado solo punto 1 (unicidad de email por tenant), rechazado punto 2 (estrategia completa de duplicados como punto abierto)*

---

## Prompt 20 — Decisión sobre Problema 18 + Instrucción de aplicar cambios

> Acepto, añade como punto abierto. Como es el último problema realiza todas las modificaciones que hemos acordado sobre la documentacion original en nuestra conversación

*Decisión: Aceptado como punto abierto (PA-G.03 — matriz de planes de suscripción). Instrucción de aplicar todas las modificaciones al documento.*

---

## Prompt 21 — Continuación de aplicación de cambios

> Continuar

*Instrucción de continuar con la aplicación de modificaciones al documento (el proceso se había interrumpido por longitud de respuesta).*

---

## Prompt 22 — Solicitud de este fichero

> Ahora necesito que generes un fichero en formado Markdown con el histórico de prompts que te he lanzado en esta conversación.
