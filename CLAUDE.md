# PROJECT SHINE — Prediagnóstico PI Group
## Proyecto Claude Code | LCG MX

---

## OBJETIVO DEL PROYECTO

Ejecutar el prediagnóstico operativo de PI Group SA de CV (Productos Innovadores) como parte del proceso de adquisición por South Light Capital. El entregable final es una **presentación ejecutiva con storytelling** que presente al fondo inversionista un inventario de oportunidades priorizado con estimación de impacto e inversión requerida.

**Audiencia final:** Gerardo Mendoza (líder del fondo), Juan Carlos Bojalil, asesores financieros (Emerge Advisors, Alecrob).
**Tono:** Consultoría estratégica de alto nivel. Datos duros con narrativa clara de "de dónde venimos, dónde estamos, a dónde podemos llegar".

---

## HILO CONDUCTOR: 12 PILARES DEL MODELO MACRO LCG

Todo el prediagnóstico se organiza bajo los **12 Pilares del Modelo Macro de Diagnóstico Operativo de LCG**. Este modelo cubre el ciclo completo del negocio y es la columna vertebral de todos los entregables: hallazgos, oportunidades, documento integrador y presentación final.

**El prediagnóstico NO se organiza por entrevista ni por persona entrevistada.** Cada entrevista alimenta múltiples pilares. Cada pilar se alimenta de múltiples entrevistas y documentos. La vista final es siempre por pilar.

### Pilares Comerciales

| # | Pilar | Sub-módulos |
|---|-------|-------------|
| 01 | **Inteligencia Comercial** | Mix de clientes · Mix de productos · Venta cruzada · Prospección · Precios · Condiciones comerciales |
| 02 | **Ejecución Comercial** | Recepción de pedidos · Promotoría · Gestión KAM · CPFR · Fill rate / OTIF · Estructura comercial |

### Pilares Lean 4.0

| # | Pilar | Sub-módulos |
|---|-------|-------------|
| 03 | **Planeación de Producción** | S&OP · Pronóstico de demanda · Planeación de materiales · Capacity plan · Programación · Estándares |
| 04 | **Producción (Control de Piso)** | OEE · Fábrica visual · Trabajo estándar (SMED) · 5S · Kaizen · Gemba walk · Estándares de operación |
| 05 | **Mantenimiento** | Plan anual · CMMS · Preventivo · Correctivo · Predictivo · Autónomo · Gestión de refacciones |
| 06 | **Calidad** | Estándares · Plan de inspecciones · Inspección MP · Control de calidad · Quejas y devoluciones · Merma · Aseguramiento |
| 07 | **Innovación** | Generación de ideas · Desarrollo de iniciativas · Comité de innovación · Funnel · KPIs de innovación |
| 08 | **Abastecimiento** | Planeación de compra · Selección y negociación de proveedores · Análisis de costos · Desarrollo de proveedores · Comité |
| 09 | **Almacenes** | Control de inventarios · Slotting · Picking · Ubicación y traslado · Diseño de almacén · Recibo · KPIs |
| 10 | **Distribución** | Última milla · Capacidad y plan de flota · Control de combustible · Eficiencia · TMS · Seguimiento de rutas |

### Pilares de Soporte

| # | Pilar | Sub-módulos |
|---|-------|-------------|
| 11 | **Digitalización / IT** | Data analytics · Automatización · Sistemas de información · IoT / Tech 4.0 · Arquitectura · Infraestructura de datos |
| 12 | **Estructura, Gobierno y Capital Humano** | Desarrollo de líderes · Manejo del cambio · Gobierno operativo · Indicadores de gestión · Talento · Compensación · Cultura |

### Mapeo de Ejes de Diagnóstico → Pilares

Los 8 ejes originales del diagnóstico se absorben dentro de los 12 pilares:

| Eje original | Se mapea a Pilar(es) |
|---|---|
| 1. Rentabilidad y EBITDA | Transversal — se evalúa como resultado de todos los pilares |
| 2. Abastecimiento Estratégico y Formulación | 07. Innovación + 08. Abastecimiento |
| 3. Eficiencia Productiva y Operaciones | 03. Planeación + 04. Producción + 05. Mantenimiento |
| 4. Diversificación Comercial | 01. Inteligencia Comercial + 02. Ejecución Comercial |
| 5. Transformación Digital y Madurez de Datos | 11. Digitalización / IT |
| 6. Gobierno Corporativo y Gestión por KPIs | 12. Estructura, Gobierno y Capital Humano |
| 7. Logística y Servicio al Cliente | 09. Almacenes + 10. Distribución |
| 8. Capital Humano y Productividad | 12. Estructura, Gobierno y Capital Humano |

### Documento de referencia completo

El documento `knowledge-base/PREDX_Modelo_Macro_Integrado.md` contiene para cada pilar: sub-módulos, preguntas de entrevista y documentos/data/herramientas solicitadas. Es la guía operativa del prediagnóstico.

---

## ESTRUCTURA DEL PROYECTO

```
project-shine/
├── CLAUDE.md                              # Este archivo — instrucciones del proyecto
│
├── knowledge-base/
│   ├── PI_Group_Knowledge_Base.md         # Fuente de verdad consolidada
│   ├── LCG_Brand_Guidelines.md            # Lineamientos de marca LCG
│   ├── PREDX_Modelo_Macro_Integrado.md    # Modelo macro de 12 pilares (guía de entrevistas y RFI)
│   └── CMM_Modelo_Madurez_12_Pilares.md   # Modelo de madurez CMM por pilar y sub-módulo
│
├── entrevistas/
│   ├── raw/                               # Transcripts originales (.docx, .txt, audio)
│   ├── procesadas/                        # Notas estructuradas por entrevista (.md)
│   ├── presentaciones/                    # HTML interactivo resumen por entrevista
│   └── hallazgos_consolidados.md          # Síntesis cruzada — vista POR PILAR, no por persona
│
├── documentos/
│   ├── raw/                               # Archivos originales recibidos de PI Group
│   └── analisis/                          # Análisis de cada documento recibido
│
├── analisis/
│   ├── financiero/                        # Modelos, bridges, análisis de P&L
│   ├── operativo/                         # Hallazgos de planta, productividad
│   ├── comercial/                         # Análisis de clientes, pricing, mix
│   └── organizacional/                    # Estructura, gobierno, capital humano
│
├── oportunidades/
│   ├── inventario_oportunidades.md        # Lista maestra — cada OPP ligada a pilar(es)
│   └── fichas/                            # Ficha detallada por oportunidad
│
├── prediagnostico/                        # DOCUMENTO INTEGRADOR DE RESULTADOS
│   ├── resultados_analisis.md             # Documento maestro — organizado por los 12 pilares
│   ├── evaluacion_madurez.md              # Evaluación CMM viva — se actualiza con cada entrevista/doc
│   └── por_pilar/                         # Análisis detallado por pilar (si se requiere desglose)
│       ├── 01_inteligencia_comercial.md
│       ├── 02_ejecucion_comercial.md
│       ├── ...
│       └── 12_estructura_gobierno_rrhh.md
│
└── presentacion/
    ├── storyline.md                       # Estructura narrativa de la presentación (5 actos)
    ├── slides/                            # Contenido por slide
    └── output/                            # Archivos .pptx generados
```

---

## FLUJOS DE TRABAJO

### FLUJO 1: PROCESAR ENTREVISTA

Cuando el usuario comparta un transcript de entrevista (audio, .docx, texto pegado):

**Paso 1 — Extracción**
1. Leer el transcript completo.
2. Ignorar ruido de transcripción automática (errores de speech-to-text, muletillas, fragmentos ininteligibles).
3. Identificar al entrevistado, entrevistadores, fecha y duración.

**Paso 2 — Nota Estructurada**
Crear archivo en `entrevistas/procesadas/` con el nombre: `YYYY-MM-DD_cargo_nombre.md`

Estructura de la nota:

```markdown
# Entrevista: [Cargo] — [Nombre]
**Fecha:** [fecha] | **Duración:** [duración] | **Entrevistadores LCG:** [nombres]

## Contexto y Rol del Entrevistado
[Breve descripción de su posición, antigüedad, alcance real de responsabilidades]

## Hallazgos por Pilar del Modelo Macro

### Pilar [##]: [Nombre del Pilar]
- Hallazgo con dato concreto
- Hallazgo con dato concreto

### Pilar [##]: [Nombre del Pilar]
- ...

(Solo incluir pilares que la entrevista tocó)

## Datos Duros Obtenidos
| Dato | Valor | Contexto | Pilar |
|------|-------|----------|-------|
| ... | ... | ... | ... |

## Banderas / Alertas
- [Cosas que requieren seguimiento o que contradicen información previa]

## Oportunidades Identificadas
- [Oportunidad con estimación preliminar de impacto si es posible — indicar pilar]

## Información para Validar
- [Cosas que se mencionaron pero necesitan confirmación con otra fuente]

## Citas Relevantes (parafraseadas)
- [Frases clave del entrevistado que capturan insight importante]

## Documentos Recibidos o Comprometidos
| Documento | Tipo | Status | Pilar |
|-----------|------|--------|-------|
| ... | INDICADOR/HERRAMIENTA/EVIDENCIA/TÉCNICO | Recibido/Pendiente | ## |
```

**Paso 3 — Presentación HTML por Entrevista**
Crear un archivo HTML interactivo en `entrevistas/presentaciones/YYYY-MM-DD_cargo_nombre.html` que presente:

1. **Resumen ejecutivo de la entrevista**: quién es, qué rol juega, contexto relevante.
2. **Hallazgos organizados por Pilar del Modelo Macro**: para cada pilar que la entrevista tocó, mostrar hallazgos, datos duros y citas relevantes.
3. **Áreas de oportunidad identificadas**: conectadas al pilar correspondiente y con estimación preliminar de impacto.
4. **Archivos y documentos asociados**: referencias a los documentos que la persona compartió o que se le solicitaron, con status.
5. **Gaps de información**: qué quedó pendiente de esta persona por pilar.

**Diseño del HTML:** Usar paleta LCG (Forest Green, Teal, Mint, Sage, Off-White). Navegable por pilar. Tono visual profesional. Este es un entregable de trabajo interno — no es la estructura del documento final.

**Paso 4 — Actualizar Knowledge Base**
Integrar los hallazgos nuevos al `PI_Group_Knowledge_Base.md`:
- Corregir datos que se actualicen (nombres, cifras, estructura).
- Agregar información nueva en la sección correspondiente.
- Si hay contradicciones con datos previos, documentar ambas versiones y marcar para validación.

**Paso 5 — Actualizar Hallazgos Consolidados**
Actualizar `entrevistas/hallazgos_consolidados.md` con vista cruzada **organizada por pilar**:
- Para cada pilar: qué dicen las diferentes fuentes (entrevistas + documentos).
- Temas recurrentes, contradicciones entre fuentes y patrones emergentes.
- Nivel de confianza de la información por pilar (cuántas fuentes lo confirman).

**Paso 6 — Actualizar Documento Integrador**
Incorporar hallazgos al documento `prediagnostico/resultados_analisis.md` en el pilar correspondiente.

**Paso 7 — Evaluar y Actualizar Nivel de Madurez CMM**
Para cada pilar que la entrevista tocó, actualizar la evaluación de madurez en `prediagnostico/evaluacion_madurez.md`:
1. Consultar `knowledge-base/CMM_Modelo_Madurez_12_Pilares.md` para los criterios del nivel correspondiente.
2. Para cada sub-módulo tocado, asignar nivel (1-5) basado en la evidencia recopilada hasta el momento.
3. **Regla: calificar con base en evidencia, no en intención.** Si la empresa dice "tenemos un proceso" pero no hay evidencia de que se ejecute, el nivel es el que corresponda a lo observable.
4. Cuando hay duda entre dos niveles, elegir el más bajo salvo evidencia sólida del superior.
5. Registrar la evidencia que sustenta la calificación (fuente: entrevista, documento, análisis).
6. Recalcular el promedio del pilar.
7. Si un sub-módulo no tiene evidencia suficiente, marcarlo como "Pendiente de evaluación" — NO inventar calificación.

---

### FLUJO 2: PROCESAR DOCUMENTO

Cuando el usuario comparta documentos de PI Group (Excel, PDF, Word, imágenes, PowerPoint, etc.):

**Paso 1 — Catalogar**
Guardar en `documentos/raw/` y registrar en un índice con: nombre, tipo, fecha recibida, persona que lo compartió, pilar(es) relacionado(s).

**Paso 2 — Analizar**
Crear análisis en `documentos/analisis/` con:
- Resumen del contenido.
- Datos clave extraídos.
- Conexiones con hallazgos de entrevistas — referenciando pilar(es).
- Preguntas que genera.
- Impacto en el inventario de oportunidades.

**Paso 3 — Actualizar KB, Hallazgos Consolidados y Documento Integrador**
Misma lógica que en entrevistas: los datos se distribuyen al pilar que corresponda.

**Paso 4 — Evaluar y Actualizar Nivel de Madurez CMM**
Misma lógica que en entrevistas (Flujo 1, Paso 7): actualizar `prediagnostico/evaluacion_madurez.md` con la evidencia del documento.

---

### FLUJO 3: ANÁLISIS ESPECÍFICO

Cuando el usuario pida un análisis puntual (bridge de EBITDA, análisis de productividad, etc.):

1. Usar datos de la Knowledge Base + documentos + entrevistas.
2. Crear archivo en `analisis/[categoría]/`.
3. Incluir siempre: datos fuente, metodología, hallazgo, pilar(es) relacionado(s), implicación para el inventario de oportunidades.
4. Si faltan datos, listar explícitamente qué se necesita y de quién obtenerlo.

---

### FLUJO 4: CONSTRUIR INVENTARIO DE OPORTUNIDADES

El inventario es el corazón del prediagnóstico. Se construye incrementalmente.

**Estructura del inventario (`oportunidades/inventario_oportunidades.md`):**

```markdown
# Inventario de Oportunidades — Project Shine

## Resumen Ejecutivo
| Total oportunidades | Impacto estimado total | Quick wins | Mediano plazo | Largo plazo |
|---------------------|----------------------|------------|---------------|-------------|
| [n] | $[x]M MXN | [n] | [n] | [n] |

## Oportunidades Priorizadas

### OPP-001: [Nombre de la oportunidad]
| Atributo | Detalle |
|----------|---------|
| Pilar(es) | [Pilar(es) del Modelo Macro] |
| Área | [Área de la empresa] |
| Impacto estimado | $[x]M MXN / año |
| Confianza | Alta / Media / Baja |
| Plazo de implementación | Quick win / 3-6 meses / 6-12 meses |
| Inversión requerida | $[x]M MXN |
| ROI estimado | [x]:1 |
| Evidencia | [Fuentes: entrevista, documento, análisis] |
| Descripción | [Qué es la oportunidad] |
| Mecanismo de captura | [Cómo se captura el valor] |
| Riesgos / dependencias | [Qué podría salir mal] |
| Status | Identificada / Validada / En análisis |
```

**Cada oportunidad tiene una ficha detallada** en `oportunidades/fichas/OPP-XXX.md`.

**Criterios de priorización:**
1. Impacto en EBITDA (absoluto y como % de EBITDA actual).
2. Velocidad de implementación (quick win > largo plazo).
3. Nivel de confianza en la estimación.
4. Complejidad / riesgo de ejecución.
5. Dependencias (¿requiere cierre de transacción? ¿requiere datos adicionales?).

---

### FLUJO 5: DOCUMENTO INTEGRADOR DE RESULTADOS

El documento `prediagnostico/resultados_analisis.md` es el entregable analítico central. Se construye incrementalmente conforme se procesan entrevistas y documentos. **Sigue estrictamente el hilo conductor de los 12 pilares.**

**Estructura:**

```markdown
# Prediagnóstico Operativo — Resultados y Análisis
## PI Group SA de CV | London Consulting Group | 2026

---

## Resumen Ejecutivo
[Vista de alto nivel: estado general, principales hallazgos transversales, EBITDA bridge, magnitud total de oportunidades]

---

## Pilar 01: Inteligencia Comercial

### Nivel de Madurez CMM: [X.X] / 5.0 — [NOMBRE DEL NIVEL]
| Sub-módulo | Nivel | Evidencia clave |
|------------|-------|-----------------|
| Mix de clientes | [1-5] | [fuente] |
| Mix de productos | [1-5] | [fuente] |
| Venta cruzada | [1-5] | [fuente] |
| Prospección | [1-5] | [fuente] |
| Precios | [1-5] | [fuente] |
| Condiciones comerciales | [1-5] | [fuente] |

**Laggers principales:** [Los puntos críticos de este pilar vs. CMM]
**Best practices aplicables:** [Las prácticas de nivel 4-5 más relevantes para PI Group]

### Estado Actual
Descripción de cómo opera hoy PI Group en este pilar.

### Hallazgos Clave
Hallazgos consolidados de TODAS las fuentes (entrevistas, documentos, análisis financiero, visita de planta).
Cada hallazgo indica su fuente entre paréntesis.

### Datos Duros
| Métrica | Valor | Fuente |
|---------|-------|--------|
| ... | ... | ... |

### Oportunidades Identificadas
Oportunidades del inventario que corresponden a este pilar.

### Gaps de Información
Qué falta por confirmar y de quién obtenerlo.

---

## Pilar 02: Ejecución Comercial
[Misma estructura]

...

## Pilar 12: Estructura, Gobierno y Capital Humano
[Misma estructura]

---

## Vista Transversal: Rentabilidad y EBITDA
[Bridge de EBITDA, análisis de erosión de margen, conexión entre pilares y su impacto financiero]

---

## Inventario Consolidado de Oportunidades
[Resumen del inventario completo, matriz impacto vs. esfuerzo]
```

**Regla clave:** Este documento NO tiene secciones tipo "Entrevista con Marco" o "Entrevista con Hugo". Los hallazgos de cada persona se distribuyen al pilar que corresponda. Las presentaciones HTML individuales por entrevista existen como referencia de trabajo, pero el documento integrador es por pilar.

---

### FLUJO 6: CONSTRUIR PRESENTACIÓN (STORYTELLING)

La presentación es el entregable final al fondo. Se construye al final cuando hay suficiente evidencia.

**Narrativa (storyline) — 5 actos:**

```
ACTO 1 — "La empresa que construyeron" (Context)
→ Quién es PI Group, qué han logrado, por qué es un activo valioso.
→ Datos: 30+ años, capacidad, fill rate, certificaciones, Members Mark.
→ Tono: Reconocimiento genuino del negocio.

ACTO 2 — "Lo que los números revelan" (Diagnostic)
→ Análisis financiero: la historia que cuentan los estados financieros.
→ Bridge de EBITDA: de $690M a $389M — dónde se fue el valor.
→ Banderas: devoluciones, Labour COGS, SG&A, concentración.
→ Tono: Analítico, sin juicio. Los datos hablan.

ACTO 3 — "Lo que encontramos en el terreno" (Findings)
→ Hallazgos organizados por los 12 pilares del Modelo Macro LCG.
→ Secuencia: Pilares Comerciales (01-02) → Lean 4.0 (03-10) → Soporte (11-12).
→ **CADA PILAR ABRE CON SU NIVEL DE MADUREZ CMM** (basado en evaluacion_madurez.md):
  - Slide de apertura por pilar: nombre del pilar + nivel de madurez (número grande + barra visual)
    + semáforo (Reactivo/Gestionado/Definido/Cuantitativo/Optimizado)
    + desglose por sub-módulo como mini-radar o barra horizontal
    + los 2-3 laggers principales del pilar (qué los ancla en ese nivel)
    + las 2-3 best practices más relevantes de nivel 4-5 que podrían aplicar
  - Slides siguientes: hallazgos clave con datos duros que sustentan la calificación.
→ NO se presenta por entrevista. Las entrevistas son fuente; los pilares son estructura.
→ Contraste entre lo que dicen los números (Acto 2) y lo que encontramos en cada pilar.
→ Tono: Descubrimiento, insight operativo. Cada pilar cuenta una historia.
→ La referencia de laggers y best practices sale de CMM_Modelo_Madurez_12_Pilares.md.

ACTO 4 — "El valor que está sobre la mesa" (Opportunities)
→ Inventario de oportunidades priorizado, cada una ligada a su(s) pilar(es).
→ Quick wins vs. mediano plazo vs. transformacional.
→ Estimación de impacto en EBITDA con rangos.
→ Casos de referencia LCG (Runcal, KATCON).
→ Tono: Ambición fundamentada. "Esto es lo que se puede lograr."

ACTO 5 — "El plan para capturarlo" (Roadmap)
→ Propuesta de proyecto LCG: fases, equipo, timeline.
→ Inversión requerida vs. retorno esperado.
→ Primeros 100 días post-cierre.
→ Tono: Acción concreta. "Así arrancamos."
```

**Diseño de la presentación:**
- **OBLIGATORIO:** Seguir `knowledge-base/LCG_Brand_Guidelines.md` para colores, tipografía y composición.
- Paleta: Forest Green (`#003D2D`) + Teal (`#009072`) + Mint (`#31EB97`) + Sage (`#CDDCC9`) + Off-White (`#F3F3F3`).
- Tipografía: DM Serif Text (títulos), Archivo (body), Suisse Int'l Mono (datos/metadata).
- Estructura "sandwich": slides oscuras para títulos de acto y oportunidades, slides claras para contenido y datos.
- Slides de datos: Grandes números (60-72pt) con contexto en texto pequeño.
- Bridge de EBITDA: Waterfall chart.
- Inventario: Matriz de impacto vs. esfuerzo.
- No usar bullet points genéricos. Cada slide debe tener un visual.

---

## REGLAS Y CONVENCIONES

### Sobre datos
- Todas las cifras financieras en **MXN millones (MXN mm)** salvo que se indique lo contrario.
- Período de análisis: **2022–2025**.
- Año base para comparaciones: **2023** (pico de ingresos/EBITDA).
- Si un dato tiene dos fuentes que se contradicen, documentar ambas y marcar para validación.

### Sobre confidencialidad
- Este es un proyecto **CONFIDENCIAL**.
- El fondo se llama **South Light Capital**.
- **Internamente en PI Group**, LCG se presenta como haciendo un "diagnóstico operativo" — NO mencionar due diligence ni M&A.
- **No incluir fórmulas, nombres de materias primas ni procesos productivos específicos** (restricción del LOI).

### Sobre el tono
- Para documentos internos LCG: directo, analítico, sin rodeos.
- Para la presentación al fondo: storytelling consultivo — datos duros envueltos en narrativa clara. Ni alarmista ni complaciente.
- Siempre conectar hallazgo → pilar → impacto financiero → oportunidad de mejora.

### Sobre la Knowledge Base
- `PI_Group_Knowledge_Base.md` es la **fuente de verdad consolidada**.
- Se actualiza con cada entrevista y documento nuevo.
- Si Claude necesita contexto sobre PI Group, este archivo tiene todo.

### Sobre el Modelo Macro
- `PREDX_Modelo_Macro_Integrado.md` es la **guía operativa del prediagnóstico**.
- Contiene las preguntas de entrevista y solicitudes de documentos por pilar.
- Si Claude necesita saber qué preguntar o qué solicitar para un pilar específico, este archivo tiene la respuesta.

### Sobre el Modelo de Madurez CMM
- `CMM_Modelo_Madurez_12_Pilares.md` es el **repositorio de knowledge management** con los criterios de madurez por sub-módulo.
- Define 5 niveles (Reactivo → Optimizado) con descripción detallada de cada nivel para cada sub-módulo de los 12 pilares.
- Contiene los **laggers** (prácticas de nivel 1-2) y **best practices** (prácticas de nivel 4-5) por pilar.
- La evaluación viva se mantiene en `prediagnostico/evaluacion_madurez.md` — se actualiza con cada entrevista y documento procesado.
- **En la presentación final (Acto 3)**, cada pilar abre con su nivel de madurez CMM como contexto visual antes de los hallazgos.
- **Regla de calificación:** solo con evidencia. Sin evidencia = "Pendiente". Cuando hay duda, nivel más bajo.

---

## COMANDOS RÁPIDOS

| Comando | Acción |
|---------|--------|
| `procesa entrevista [archivo]` | Ejecutar Flujo 1 completo (nota + HTML + KB + consolidados + doc integrador) |
| `procesa documento [archivo]` | Ejecutar Flujo 2 completo |
| `actualiza KB` | Re-sincronizar Knowledge Base con hallazgos recientes |
| `status oportunidades` | Mostrar resumen del inventario actual |
| `nueva oportunidad [nombre]` | Crear ficha de oportunidad nueva |
| `analisis [tema]` | Ejecutar análisis específico (Flujo 3) |
| `status pilares` | Mostrar nivel de madurez CMM + completitud de información por cada pilar |
| `madurez [pilar]` | Mostrar evaluación CMM detallada por sub-módulo del pilar indicado (o todos si no se indica) |
| `storyline` | Mostrar estructura narrativa actual de la presentación |
| `genera presentacion` | Ejecutar Flujo 6 — crear .pptx |
| `que me falta` | Listar gaps de información por pilar: qué datos faltan y de quién obtenerlos |
| `status proyecto` | Vista general: entrevistas realizadas, documentos procesados, oportunidades, gaps |

---

## ESTADO ACTUAL DEL PROYECTO

### Información recopilada
- ✅ Estados financieros consolidados 2022-2025 (mensuales y anuales, por entidad)
- ✅ Organigrama general del grupo (PDF, edición julio 2024)
- ✅ Investigación de cuenta (fuentes públicas)
- ✅ Notas de estados financieros (análisis LCG)
- ✅ Plan de entrevistas y ejes de diagnóstico
- ✅ Transcript reunión de presentación LCG (9 marzo 2026)
- ✅ Transcript entrevista Marco Bárcenas (18 marzo 2026)
- ✅ Modelo Macro Integrado de 12 pilares (guía de entrevistas y RFI)

### Entrevistas realizadas
| # | Fecha | Entrevistado | Status nota | Status HTML |
|---|-------|-------------|------------|-------------|
| 1 | 18-mar-2026 | Marco Bárcenas (Dir. Finanzas) | ✅ Integrada en KB | 🔲 Pendiente |

### Entrevistas pendientes
| # | Cargo | Nombre | Prioridad | Pilares principales |
|---|-------|--------|-----------|---------------------|
| 1 | Director General | Por confirmar | CRÍTICA | 12 (Gobierno), Transversal |
| 2 | Director Comercial | Hugo Ambrosi | CRÍTICA | 01, 02 |
| 3 | Director de Operaciones | Rodolfo Vega | ALTA | 03, 04, 05, 09, 10 |
| 4 | Gerente de Producción | Por confirmar | ALTA | 03, 04 |
| 5 | Gerente de Logística | Por confirmar | ALTA | 09, 10 |
| 6 | Subdirector I+D | Por confirmar (mujer) | ALTA | 07 |
| 7 | Gerente de Compras | Por confirmar | ALTA | 08 |
| 8 | Gerente de TI | Por confirmar | ALTA | 11 |
| 9 | Gerente de Mantenimiento | Por confirmar | MEDIA-ALTA | 05 |
| 10 | Gerente de Control de Calidad | Por confirmar | MEDIA-ALTA | 06 |
| 11 | Gerente de Costos | Por confirmar | ALTA | 12 (Gobierno/KPIs) |
| 12 | Gerente Capital Humano | Por confirmar | MEDIA | 12 |
| 13 | Gerente Normatividad / SGI | Por confirmar | MEDIA | 06, 12 |
| + 5 más | Ver plan completo en KB sección 10.2 | | | |

### Cobertura por Pilar (% de información recopilada)

| # | Pilar | Cobertura | Fuentes actuales |
|---|-------|-----------|------------------|
| 01 | Inteligencia Comercial | 🟡 ~20% | Marco (financiero), KB pública |
| 02 | Ejecución Comercial | 🟡 ~15% | Marco (overview) |
| 03 | Planeación de Producción | 🔴 ~10% | Marco (overview) |
| 04 | Producción | 🔴 ~10% | Marco (overview: baches 30K L) |
| 05 | Mantenimiento | 🔴 ~5% | — |
| 06 | Calidad | 🔴 ~10% | KB (certificaciones ISO) |
| 07 | Innovación | 🔴 ~5% | — |
| 08 | Abastecimiento | 🔴 ~10% | Marco (overview) |
| 09 | Almacenes | 🔴 ~10% | Marco (layout naves) |
| 10 | Distribución | 🔴 ~10% | Marco (modelo CEDIS) |
| 11 | Digitalización / IT | 🔴 ~5% | — |
| 12 | Estructura, Gobierno y RRHH | 🟡 ~30% | Marco (gobierno, estructura, familia) |

### Oportunidades identificadas (preliminar)
| ID | Oportunidad | Pilar(es) | Impacto est. | Status |
|----|------------|-----------|-------------|--------|
| OPP-001 | Reducción de devoluciones y descuentos | 01, 02, 06 | $50-135M | Identificada |
| OPP-002 | Optimización de formulación y MP | 07, 08 | $30-80M | Identificada |
| OPP-003 | Productividad laboral | 04, 12 | $10-20M | Identificada |
| OPP-004 | Racionalización de SG&A/PISA | 12 | $20-50M | Identificada |
| OPP-005 | Diversificación de clientes | 01, 02 | Estratégica | Identificada |
| OPP-006 | Gobierno corporativo y KPIs | 12 | Habilitadora | Identificada |
| OPP-007 | Digitalización de planta | 11 | Habilitadora | Identificada |

*Todas las estimaciones son preliminares. Se refinan con evidencia de entrevistas y documentos operativos.*

---

## DEPENDENCIAS Y HERRAMIENTAS

- **Archivos Excel:** openpyxl para lectura, análisis con Python/pandas.
- **Transcripts:** pandoc para conversión, procesamiento manual de contenido.
- **Presentación final:** pptxgenjs (ver skill pptx) para generar .pptx de calidad.
- **Análisis financieros:** Python con pandas/numpy para modelos y bridges.
- **Visualizaciones:** matplotlib/seaborn para gráficos de análisis; pptxgenjs para gráficos en slides.
- **HTMLs de entrevistas:** HTML + CSS con paleta LCG, navegable por pilar.
