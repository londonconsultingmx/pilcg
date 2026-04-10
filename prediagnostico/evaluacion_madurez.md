# Evaluacion de Madurez CMM — PI Group
## Prediagnostico Operativo | London Consulting Group | 2026

**Ultima actualizacion:** 2026-04-08
**Referencia de criterios:** `knowledge-base/CMM_Modelo_Madurez_12_Pilares.md`

---

## Mapa de Calor General

| # | Pilar | Promedio | Semaforo | Sub-modulos evaluados | Confianza |
|---|-------|---------|----------|----------------------|-----------|
| 01 | Inteligencia Comercial | 1.7 | ROJO | 6 / 6 | Media |
| 02 | Ejecucion Comercial | 1.8 | ROJO | 6 / 6 | Media |
| 03 | Planeacion de Produccion | 2.0 | NARANJA | 5 / 6 | Media |
| 04 | Produccion (Control de Piso) | 1.9 | ROJO | 7 / 9 | Media |
| 05 | Mantenimiento | 2.3 | NARANJA | 6 / 7 | Media |
| 06 | Calidad | 2.0 | NARANJA | 4 / 7 | Baja |
| 07 | Innovacion | 1.8 | ROJO | 3 / 5 | Baja-Media |
| 08 | Abastecimiento | 2.2 | NARANJA | 5 / 7 | Media |
| 09 | Almacenes | 1.8 | ROJO | 4 / 7 | Baja-Media |
| 10 | Distribucion | 2.5 | NARANJA | 5 / 7 | Media-Alta |
| 11 | Digitalizacion / IT | 1.5 | ROJO | 4 / 6 | Media |
| 12 | Estructura, Gobierno y RRHH | 1.8 | ROJO | 6 / 7 | Media-Alta |

**Promedio general:** 1.9 (Reactivo-Gestionado)
**Escala:** 1 Reactivo | 2 Gestionado | 3 Definido | 4 Cuantitativo | 5 Optimizado

**Interpretacion:** Operacion funcional pero fragil. Dependencia de heroismo individual en multiples pilares. Se requiere estabilizar y estandarizar procesos basicos, medir lo esencial y asignar responsables. La empresa genera resultados a pesar de su nivel de madurez — lo cual confirma la magnitud de la oportunidad de mejora.

---

## Pilar 01: Inteligencia Comercial

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| Mix de clientes | 1 | Sam's Club representa ~96-99% de ingresos. No existe plan de diversificacion activo con metas y timeline — solo intenciones (Costco, Home Depot). No se calcula rentabilidad por cliente. No existe CRM ni herramienta de analisis de cartera. | Marco Barcenas, Hugo Ambrosi, Analisis Comercial | 2026-04-08 |
| Mix de productos | 2 | Existe catalogo de SKUs con ventas por producto (Excel). Se identifican los SKUs estrella (Top 5 = 65.1% de la venta). Sin embargo, no hay analisis de margen de contribucion por SKU con costos completos asignados; no hay proceso de racionalizacion formal; cola de SKUs automotrices con sobreinventario cronico (Abrillantador 125 dias DDI) sin accion de kill/keep. | Analisis Comercial (Ventas Piso, Formato de Stock), Hugo Ambrosi | 2026-04-08 |
| Venta cruzada | 1 | No se analiza sistematicamente que categorias adicionales podrian venderse a clientes existentes. Hugo lo identifica como oportunidad (ampliar catalogo Home Depot, explorar sector institucional) pero no existe analisis de white spaces ni plan formal de penetracion. E-commerce completamente abandonado (cuentas en MeLi y Amazon sin atencion, $0 ventas). | Hugo Ambrosi | 2026-04-08 |
| Prospeccion | 2 | Se han intentado acercamientos esporadicos: proyecto Costco (jabon de manos, piden "mas premium"), acercamiento a Bolt (exitoso, 3x ventas esperadas), exploracion de sector institucional en feria de Las Vegas. Pero no hay pipeline formal en CRM, no hay equipo hunter, no hay metas de apertura de cuentas. El dueno atiende prospectacion personalmente. | Marco Barcenas, Hugo Ambrosi | 2026-04-08 |
| Precios | 2 | Se tiene nocion del costo pero la negociacion es reactiva. Llevan 2 anos sin incremento de precio al cliente (desde finales 2023) mientras costos suben. Se detecto alerta de volumen vs precio (detergente 10L cayo -9.6% en unidades pero crecio +0.9% en pesos) pero sin modelo de elasticidad. El costo de los nuevos SKUs de detergente es 12% mayor sin ajuste proporcional de precio. | Hugo Ambrosi, Rodolfo Vega, Analisis Comercial | 2026-04-08 |
| Condiciones comerciales | 2 | Se registran descuentos comerciales ($263M en 2025 = 12.7% sobre venta neta), pero el rubro "Otros" ($35M real vs $7M presupuesto = 5x desviacion) evidencia falta de control. Devoluciones se duplicaron de $143M (2022) a $276M (2025) = 13.2% de ventas brutas, sin diagnostico de causa raiz que separe calidad vs comercial vs logistica. | Analisis Financiero, Marco Barcenas | 2026-04-08 |

**Promedio:** 1.7
**Laggers principales:**
- Concentracion >96% en un solo cliente sin plan de mitigacion con metas y timeline concretos
- No se conoce la rentabilidad real por cliente ni por SKU (con costos completos asignados)
- Sin CRM ni pipeline documentado para diversificacion
- Devoluciones de 13.2% de ventas brutas creciendo sin diagnostico de causa raiz
- 2 anos sin incremento de precios al cliente mientras costos suben

**Best practices aplicables:**
- Regla del "no mas de 30%" de ingresos en un solo cliente como meta estrategica a 5 anos, con pipeline de diversificacion con etapas, probabilidad y timeline
- P&L por cliente actualizado mensualmente con costos asignados (produccion, logistica, condiciones comerciales)
- Modelo de riesgo de concentracion con escenarios de impacto ante perdida del cliente ancla
- Analisis ABC-XYZ de portafolio cruzando rentabilidad con variabilidad de demanda; comite de portafolio trimestral con criterios de kill/keep/grow (urgente para SKUs automotrices con 90-125 dias de inventario)
- Separacion transparente de devoluciones por causa: calidad vs condicion comercial vs logistica

---

## Pilar 02: Ejecucion Comercial

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| Recepcion de pedidos | 2 | Canal principal definido (portal Sam's). Captura en sistema. Validacion basica de inventario. Sin integracion EDI/API completa. No se evidencia proceso formalizado para otros clientes (Home Depot pide poco y se acumulan pedidos, "a veces les surtimos, a veces no"). | Hugo Ambrosi, Rodolfo Vega | 2026-04-08 |
| Promotoria | 1 | Dos personas en campo (Cesar Barrios GDL, Ivan Cantu CDMX) cuyo aporte actual es tomar fotos. No llegan preparados con datos de desempeno por tienda. Sin checklist de ejecucion. Sin metricas. Hugo reconoce: "no me estan sumando nada de valor". | Hugo Ambrosi | 2026-04-08 |
| Gestion KAM | 2 | Un solo KAM (Klaus, para Sam's) que "no esta funcionando" y sera reemplazado a <3 meses de incorporacion. No existe KAM para Home Depot, Garraton, Aeromexico ni Sanchez y Martin — Hugo atiende directamente al resto. Antes, el dueno era quien daba la cara al cliente. No hay plan de cuenta formal ni scorecard. | Hugo Ambrosi | 2026-04-08 |
| CPFR | 2 | CPFR formal con Sam's Club recien implementado (3 meses): convenio de confidencialidad firmado, posicion de CPFR asignada (Cesar + Azael). Avance significativo vs el punto de partida (cero). Sin embargo, no hay CPFR con ningun otro cliente. No se mide forecast accuracy formalmente. Sin proceso para Home Depot, Bolt/S&M u otros. | Hugo Ambrosi | 2026-04-08 |
| Fill rate / OTIF | 2 | Fill rate in-full reportado por Rodolfo: 99.8% (2025). Pero el analisis de datos reales de Sam's muestra fill rate promedio de 95.2% con caidas severas a 65-75% en 5+ semanas del ano (~$45-55M en venta perdida). On-time delivery ~50% (penalizado por entregas anticipadas). Hay discrepancia entre OTIF interno y lo que mide el cliente — clasico lagger nivel 2. | Rodolfo Vega vs Analisis Comercial (Formato Stock) | 2026-04-08 |
| Estructura comercial | 2 | Estructura creada hace 3 meses por Hugo: director + KAM (fallido) + CPFR + CPFR Jr + promotores (sin valor). La mayoria de perfiles son "coordinador hacia abajo". Sin subdirector. Sin Sales Intelligence. Sin marketing estrategico. Antes no existia estructura profesional — se paso de 0 a algo, pero el algo es aun fragil. | Hugo Ambrosi | 2026-04-08 |

**Promedio:** 1.8
**Laggers principales:**
- Discrepancia entre fill rate interno (99.8%) y medicion real del cliente (95.2%) — autoengano clasico
- Fuerza de campo sin valor: 2 personas en nomina cuyo aporte es tomar fotos sin metricas ni checklist
- KAM unico que no funciona, a reemplazar. Ningun otro cliente tiene KAM dedicado
- CPFR solo con Sam's (3 meses de vida); cero proceso con otros clientes
- Home Depot desatendido >1 ano: "a veces les surtimos, a veces no"

**Best practices aplicables:**
- Single version of truth del OTIF conciliada con el cliente (alinear el 99.8% interno con el 95.2% real)
- War room semanal de servicio con representantes de produccion, logistica y comercial para cerrar gap en semanas criticas (5 semanas con FR <80% = $45-55M perdidos/ano)
- Checklist de ejecucion en tienda (12 puntos tipo PepsiCo) con scorecard por promotor
- KAMs con plan de cuenta formal (objetivos, acciones, timeline) y scorecard de desempeno
- CPFR formal para al menos los top 3 clientes (Sam's, Home Depot, S&M) con forecast accuracy como KPI compartido

---

## Pilar 03: Planeacion de Produccion

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| S&OP | 2 | Existe un AOP anual (primer AOP del area comercial, creado por Hugo en 2026). La planeacion opera en cascada: mensual → semanal → diaria. Se reconoce estacionalidad (2 temporadas definidas). Pero la funcion de planeacion reporta a Contraloria, no a Operaciones — separacion quien planea vs quien ejecuta. No hay evidencia de reunion S&OP formal con todos los stakeholders. Los cambios frecuentes llegan hasta nivel diario. | Hugo Ambrosi, Rodolfo Vega | 2026-04-08 |
| Pronostico de demanda | 2 | Hugo construyo dashboards de forecast de sellout semana a semana vs mismo periodo del ano anterior. Pero no se mide forecast accuracy formalmente. No hay modelo estadistico — es basado en historico con ajuste manual. Para S&M, la desviacion es absurda: contratan 100, terminan comprando 250. | Hugo Ambrosi, Rodolfo Vega | 2026-04-08 |
| Planeacion de materiales | 2 | Existe requerimiento de materiales basado en programa de produccion. Sin embargo, hay paros de linea por falta de material/envase (clasificados como paro de "almacen" o "planeacion"). Calidad de envases genera paros adicionales (envases inflados, rebaba). Lead times de proveedores criticos alterados por crisis geopolitica. | Rodolfo Vega, Marco Barcenas | 2026-04-08 |
| Capacity plan | 2 | Capacidad teorica conocida por linea (estandares al 85% de eficiencia). Rodolfo estima ~40% de capacidad disponible en turno actual y posibilidad de 3 turnos. Pero NO existe reporte formal que compare produccion real vs capacidad estandar. El 40% es una estimacion, no un indicador gestionado. Utilizacion real de det. 10L: ~70% de capacidad. | Rodolfo Vega | 2026-04-08 |
| Programacion de produccion | 2 | Programa formal entregado por linea con producto y cantidad. Cumplimiento ~106% (6% arriba de lo programado). Sin embargo, la programacion NO la hace operaciones (la hace Contraloria), y los cambios diarios son frecuentes. No hay frozen period. | Rodolfo Vega | 2026-04-08 |
| Estandares de produccion | Pendiente de evaluacion | Se mencionan tiempos de ciclo estandar por linea (ej. Linea 17: 1,695 tarimas/mes al 85%), piezas por hora, piezas por turno, piezas por tarima. Pero falta validacion en visita de planta del 15 abril para confirmar adherencia real. | Rodolfo Vega | — |

**Promedio:** 2.0
**Laggers principales:**
- Planeacion de produccion separada de Operaciones (reporta a Contraloria) — desconexion entre quien planea y quien ejecuta
- No existe reporte formal de utilizacion de capacidad (solo estimacion verbal del 40% disponible)
- Cambios al programa hasta nivel diario sin frozen period ni proceso formal de change request
- Forecast accuracy no medido; desviacion dramatica en clientes como S&M (250% vs contrato)
- No se evidencia reunion S&OP formal con agenda, participantes y decisiones documentadas

**Best practices aplicables:**
- S&OP mensual formal con demand review, supply review y reconciliacion ejecutiva; horizonte 3-6 meses
- Frozen period de 1-2 semanas donde el plan no cambia sin aprobacion de nivel director
- Capacity plan mensual formal: capacidad disponible vs demanda por linea, con dashboard visible
- Forecast accuracy como KPI compartido entre ventas y planeacion, medido mensualmente
- Proceso formal de gestion de excepciones (rush orders) con costo visible para quien solicita el cambio

---

## Pilar 04: Produccion (Control de Piso)

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| OEE | 2 | Se registran paros principales (2,089 horas en 2025 = ~2.18% del tiempo productivo). Se miden piezas por hora, piezas por turno. Se clasifican paros por area causal (mantenimiento ~25%, produccion, calidad MP, planeacion, almacen). Pero NO se calcula OEE formal (Disponibilidad x Rendimiento x Calidad). No hay descomposicion sistematica de perdidas por linea. | Rodolfo Vega | 2026-04-08 |
| Fabrica visual | Pendiente de evaluacion | No se evidencio informacion sobre tableros en piso, senalizacion, andones o gestion visual. Requiere validacion en visita de planta 15 abril. | — | — |
| Trabajo estandar (SMED) | 2 | Existen tiempos de ciclo estandar por linea (calculos al 85% eficiencia). Se manejan plantillas definidas por temporada. Pero no se evidencio aplicacion de SMED para changeovers, ni se mencionaron tiempos de cambio como tema gestionado. | Rodolfo Vega | 2026-04-08 |
| 5S | 2 | Rodolfo menciona que se implementan practicas de 5S. Pero no se proporcionaron scores de auditorias, frecuencia de auditorias ni resultados. Clasificado como nivel 2 (campanas esporadicas sin evidencia de sostenimiento). Pendiente verificar en visita de planta. | Rodolfo Vega | 2026-04-08 |
| Kaizen | 2 | Se mencionan practicas de Kaizen y TPM. Pero no se evidencio programa formal con eventos periodicos, tracking de ideas implementadas, ni impacto cuantificado. Sin evidencia de A3 o PDCA formal. | Rodolfo Vega | 2026-04-08 |
| Gemba walk | Pendiente de evaluacion | No se recogio evidencia sobre rutina de presencia directiva en piso. Requiere validacion. | — | — |
| Estandares de operacion | 2 | Tiempos de ciclo estandar por linea documentados. Reporte mensual a direccion con indicadores. Pero NO se mide productividad de mano de obra como indicador (costo MO / ventas). Rodolfo: "Yo no manejo costos." Desconexion total entre volumen producido y costo. | Rodolfo Vega | 2026-04-08 |
| Reto de productividad | 1 | No se mide productividad de mano de obra. Mano de obra por litro se duplico de $0.18/L (2022) a $0.41/L (2025) con produccion similar. Gastos de fabricacion por litro se duplicaron de $0.78/L a $1.53/L. Nadie tiene visibilidad cruzada entre volumen y costo. | Analisis Financiero, Rodolfo Vega | 2026-04-08 |
| Entrenamientos Lean | 2 | Se realizan capacitaciones (cuando hay paro programado se envia a capacitacion). Evaluaciones de personal. Pero no se evidencio programa estructurado de entrenamiento Lean con curricula, certificaciones o progresion. | Rodolfo Vega | 2026-04-08 |

**Promedio:** 1.9
**Laggers principales:**
- No se calcula OEE formal — solo paros y piezas/hora sin integracion en el framework Disponibilidad x Rendimiento x Calidad
- No se mide productividad de mano de obra vs costo: MO/litro se duplico en 3 anos sin alarma porque nadie cruza volumen con costo
- Vacantes criticas: gerente de produccion y jefe de produccion vacantes, operacion sostenida por 1 supervisor
- Desconexion operaciones-costos: "Yo no manejo costos" (Rodolfo) — produccion no tiene incentivo ni visibilidad para optimizar costo
- Sin SMED evidenciado, sin programa Kaizen formal con impacto cuantificado

**Best practices aplicables:**
- OEE automatico con sensores en cada linea; juntas diarias de 15 min en piso (tier 1 meeting) con OEE del dia anterior
- Top 5 losses con dueno y fecha compromiso por perdida; SMED para reduccion de changeover en lineas principales
- Indicador de productividad: costo MO / unidad producida y MO / litro, visible tanto para Operaciones como para Finanzas
- Cubrir vacantes criticas (gerente y jefe de produccion) como condicion habilitadora de cualquier mejora
- Programa Kaizen formal: >1 idea implementada por colaborador/ano, con impacto financiero cuantificado

---

## Pilar 05: Mantenimiento

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| Plan anual | 3 | Cumplimiento a ordenes de mantenimiento preventivo 2025: 97.22%. Bajones puntuales (junio por disponibilidad de equipos). Causas de incumplimiento identificadas (falta de refaccion, equipo no prestado, olvido). Plan basado en historial con cobertura amplia. | Rodolfo Vega | 2026-04-08 |
| CMMS | 2 | Migracion en curso de MP version 10 (obsoleto, sin soporte) a Fractal. Proyecto iniciado 2025, bloqueado por falta de licencias. El sistema actual es funcional pero limitado. Fractal aun no esta desplegado completamente — no hay indicadores automaticos (MTBF, MTTR), ni asignacion de gasto por equipo. | Rodolfo Vega | 2026-04-08 |
| Preventivo | 3 | Cumplimiento 97.22% al programa preventivo. Los paros por mantenimiento representan ~25% del total (~522 horas/ano). Se miden: tiempo de reaccion, tiempo entre fallas, gastos por area. Nivel 3 porque el cumplimiento es alto y medido. | Rodolfo Vega | 2026-04-08 |
| Correctivo | 2 | Los paros por mantenimiento (522 horas/ano) se registran como causa causal en el tablero de paros. Pero no se evidencio RCA formal obligatorio para correctivos recurrentes. No se mide ratio preventivo:correctivo explicitamente. | Rodolfo Vega | 2026-04-08 |
| Predictivo | 1 | No se evidencio monitoreo de condicion de equipos (vibracion, termografia, ultrasonido). Mantenimiento basado en calendario (preventivo) y reactivo (correctivo), no en condicion real. | Rodolfo Vega | 2026-04-08 |
| Autonomo | Pendiente de evaluacion | No se recogio evidencia de mantenimiento autonomo por operadores (inspeccion, lubricacion, limpieza). Requiere validacion con Ismael Hernandez (Gte. Mantenimiento). | — | — |
| Gestion de refacciones | 2 | Almacen de refacciones con 4-5 personas en nave 8. Inventario ha crecido progresivamente en valor. Pero no se evidencio clasificacion por criticidad de equipo, ni min/max basado en analisis de consumo, ni control optimizado. | Rodolfo Vega | 2026-04-08 |

**Promedio:** 2.2 (sobre 6 evaluados)
**Laggers principales:**
- CMMS obsoleto (MP v10 sin soporte) con migracion a Fractal bloqueada por licencias — mas de 1 ano sin completar
- Cero mantenimiento predictivo: no hay monitoreo de condicion de equipos
- Gestion de refacciones sin clasificacion por criticidad ni min/max basado en analisis
- No se mide productividad por tecnico (ordenes de trabajo realizadas por persona)
- No se evidencio ratio formal preventivo:correctivo

**Best practices aplicables:**
- Completar migracion a Fractal como prioridad: resolucion del tema de licencias es cuello de botella critico
- Implementar MTBF y MTTR como KPIs principales con metas y tendencias una vez Fractal este activo
- Iniciar mantenimiento predictivo en equipos criticos: analisis de vibracion y termografia en lineas principales
- Almacen de refacciones con min/max por criticidad de equipo; acuerdos de consignacion con proveedores clave
- Mantenimiento autonomo: operadores hacen inspeccion diaria, lubricacion y limpieza como rutina estandar

---

## Pilar 06: Calidad

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| Estandares de calidad | 2 | Certificaciones ISO existentes (mencionadas en KB). Area de normatividad y SGI reporta a Rodolfo. Pero no se evidencio si los estandares se viven en el dia a dia vs existir solo para certificacion. Nivel 2 conservador hasta verificar en planta. | Rodolfo Vega, KB | 2026-04-08 |
| Plan de inspecciones | 2 | Calidad hace muestreo a la recepcion de MP. Produccion detecta problemas en llenado que el muestreo no captura (envases inflados, rebaba). No se evidencio plan de inspeccion formal con puntos de control, frecuencia y criterios documentados. | Rodolfo Vega | 2026-04-08 |
| Inspeccion MP | 2 | Muestreo a la recepcion de MP existe pero es insuficiente: produccion detecta defectos que el muestreo no atrapo. Calidad de envases de proveedores genera paros de linea. | Rodolfo Vega | 2026-04-08 |
| Control de calidad | 2 | 135 defectos reportados por cliente en 2025 (~1.76% de incidencia por viaje). Tipos: fuera de pesos, falta de codificado, mal cerrado, etiqueta desprendida, microfugas. Se rastrean por linea gracias al codificado. Pero sin SPC, sin FTQ medido, sin plan de inspeccion en proceso formalizado. | Rodolfo Vega | 2026-04-08 |
| Quejas y devoluciones | 1 | Devoluciones se duplicaron de $143M (2022) a $276M (2025) = 13.2% de ventas brutas. NO se separa causa: calidad vs comercial vs logistica. Crecen sin alarma. El area de "Atencion y Quejas" (Cesar Barrios GDL, Ivan Cantu CDMX) solo toma fotos — sin diagnostico, sin RCA, sin cierre de ciclo. | Analisis Financiero, Hugo Ambrosi | 2026-04-08 |
| Merma | Pendiente de evaluacion | No se recogio evidencia sobre medicion de merma por etapa, por producto o por turno. Requiere validacion. | — | — |
| Aseguramiento | Pendiente de evaluacion | No se recogio evidencia suficiente sobre la funcion de aseguramiento (prevencion vs deteccion). Requiere entrevista con Gte. Control de Calidad y Gte. Normatividad. | — | — |

**Promedio:** 1.8 (sobre 5 evaluados; sube a 2.0 si se promedian los 4 con nivel)
**Laggers principales:**
- Devoluciones de 13.2% de ventas brutas creciendo SIN diagnostico de causa raiz ni separacion calidad vs comercial
- Inspeccion de MP insuficiente: produccion detecta defectos que calidad no atrapo en muestreo (envases inflados, rebaba)
- Funcion de "Atencion y Quejas" no genera valor: solo fotos, sin RCA, sin cierre de ciclo
- 135 defectos reportados por cliente sin evidencia de accion correctiva sistematica

**Best practices aplicables:**
- Costo de no-calidad (COPQ) cuantificado y reportado mensualmente al comite directivo: incluir devoluciones + reprocesos + merma + paros por calidad de MP
- Separacion transparente de devoluciones: calidad vs condicion comercial vs logistica — cada una con dueno y plan de accion
- 8D para quejas de cliente con cierre en <30 dias y verificacion de eficacia
- Inspeccion de MP con criterios claros de rechazo documentados; penalizacion a proveedores por calidad deficiente
- SPC en puntos criticos del proceso; FTQ (First Time Quality) medido por linea

---

## Pilar 07: Innovacion

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| Generacion de ideas | 2 | Existe capacidad demostrada de innovacion: molecula vegetal para suavizante, migracion LESS 28% a 70%, primer envase reciclado 10L en Mexico (con Tecnopelets), exploracion de productos concentrados para sector institucional (feria Las Vegas). Pero los proyectos entran ad-hoc — no hay proceso sistematico de generacion de ideas. | Marco Barcenas, Hugo Ambrosi | 2026-04-08 |
| Desarrollo de iniciativas | 2 | Se desarrollan productos (exitosamente en varios casos), pero sin proceso stage-gate formal. No hay priorizacion sistematica: los proyectos entran por presion del cliente o por relacion con proveedores (Juan Carlos Bojalil). Costco pidio algo "mas premium" y se esta trabajando — proceso informal. | Marco Barcenas, Hugo Ambrosi | 2026-04-08 |
| Comite de innovacion | Pendiente de evaluacion | No se recogio evidencia de comite de innovacion formal. La subdirectora de I+D (Aide Gomez) tiene gestion directa con Sam's para temas tecnicos. Requiere entrevista con ella. | Hugo Ambrosi | — |
| Funnel de iniciativas | 1 | No hay funnel documentado de proyectos de innovacion con etapas, probabilidad y timeline. Se manejan proyectos puntuales sin pipeline visible. No se mide hit rate ni time-to-market. | Marco Barcenas, Hugo Ambrosi | 2026-04-08 |
| KPIs de innovacion | Pendiente de evaluacion | No se evidenciaron KPIs de innovacion (% ingresos de nuevos productos, ROI de desarrollo, etc.). Se conoce el ROI exitoso de la maquina enmangadora (recuperada en 8 meses vs 3 anos) pero como dato aislado, no como indicador gestionado. | — | — |

**Promedio:** 1.7 (sobre 3 evaluados)
**Laggers principales:**
- Todo el conocimiento de formulacion concentrado en pocas personas (Aide Gomez + relacion con Juan Carlos Bojalil para MP) — bus factor critico
- Sin proceso stage-gate: proyectos entran ad-hoc por presion de cliente o por relacion personal con proveedores
- Sin funnel de innovacion ni KPIs (hit rate, time-to-market, ROI de nuevos productos)
- Sin comite de innovacion formal para priorizar proyectos

**Best practices aplicables:**
- Base de datos de formulacion segura, documentada y con control de versiones — plan de sucesion para roles tecnicos criticos
- Stage-gate con decisiones de go/kill basadas en criterios claros (impacto, factibilidad, alineacion estrategica)
- % de ingresos provenientes de productos lanzados en los ultimos 3 anos como KPI
- Pipeline de innovacion con horizonte 1-3 anos; balance entre proyectos incrementales (mejora de formulas existentes) y adyacentes (nuevas categorias como concentrados, premium)

---

## Pilar 08: Abastecimiento

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| Planeacion de compra | 2 | Compras basadas en requerimiento del programa de produccion. Contratos a plazo fijo para materias primas criticas (LESS: 6 meses a $1.79-1.80 USD/kg vs spot de $2.30). Reporte de inflacion interna mensual. Pero paros de linea por falta de material siguen ocurriendo. Anticipos a proveedores explotaron de $0.2M (2022) a $52M (2025). | Marco Barcenas, Rodolfo Vega | 2026-04-08 |
| Seleccion y negociacion | 3 | Marco negocia personalmente con top 10 proveedores (70% del gasto). Relaciones directas con accionistas de proveedores clave (Simprise, Envases Universales, BM/M-Chem). PI obtiene precios 15% debajo de mercado con Envases Universales. Exclusividad negociada con proveedores criticos. Contrato de rebate por volumen con Simprise. Contratos a plazo fijo para proteger contra volatilidad. | Marco Barcenas | 2026-04-08 |
| Analisis de costos | 2 | Existe reporte de costo estandar diario/mensual y reporte de inflacion interna mensual de MP. Analisis de proveedores por volumen (ABC). Pero no se evidencio analisis de total cost of ownership (solo precio unitario). La gestion es reactiva ante crisis (crisis Ormuz: incrementos de envases +30%, ADBS sin stock en Mexico). | Marco Barcenas | 2026-04-08 |
| Desarrollo de proveedores | 3 | Co-desarrollo activo: molecula vegetal con Juan Carlos Bojalil, envase reciclado con Tecnopelets (PI puso ingenieria, Tecnopelets moldes). Busqueda de alternativas en China. Pero no se evidencio scorecard formal de proveedores ni evaluacion periodica estructurada con plan de accion. | Marco Barcenas | 2026-04-08 |
| Evaluacion de proveedores | Pendiente de evaluacion | No se recogio evidencia de proceso formal de evaluacion periodica de proveedores con scorecard. Requiere validacion con Gerente de Compras (vacante). | — | — |
| Ferias y congresos | Pendiente de evaluacion | Se asistio a feria en Las Vegas para productos concentrados. Sin evidencia de programa sistematico de inteligencia de mercado de proveedores. | — | — |
| Comite de abastecimiento | 1 | No se evidencio comite de abastecimiento formal. Las decisiones de compra estan altamente centralizadas en Marco (top 10) y parcialmente en Francisco Rojas (subdirector). Vacante de gerente de compras — han rotado varios sin encontrar al adecuado. Solo 2 compradores + 1 coordinador. | Marco Barcenas | 2026-04-08 |

**Promedio:** 2.2 (sobre 5 evaluados)
**Laggers principales:**
- Centralizacion extrema en Marco Barcenas: negocia personalmente 70% del gasto. "El detalle de todo, 100%, lo reviso yo"
- Vacante cronica de Gerente de Compras — han rotado varios sin exito. Solo 2 compradores + 1 coordinador
- Sin comite de abastecimiento formal para decision colegiada
- Sin analisis de total cost of ownership — gestion reactiva ante crisis de suministro
- Anticipos a proveedores crecieron 260x en 3 anos ($0.2M a $52M) sin control evidente

**Best practices aplicables:**
- Matriz de Kraljic para categorizar proveedores (estrategico, leverage, bottleneck, rutina) y definir estrategia de sourcing por categoria
- Dual sourcing minimo para insumos criticos — reducir dependencia de proveedores unicos
- Total cost of ownership como base de negociacion, no solo precio unitario
- Cubrir vacante de Gerente de Compras con perfil de sourcing estrategico — liberar tiempo de Marco
- Comite de abastecimiento mensual con participacion de calidad, I+D y operaciones

---

## Pilar 09: Almacenes

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| Control de inventarios | 2 | Inventario de producto terminado registrado. Pero dias de inventario se dispararon de ~17 (2022-2023) a ~105 (2025) — explosion de $88M a $301M (+244%). Sobreinventario cronico en categoria automotriz (Abrillantador 125 dias, Desengrasante 96 dias vs ideal de 18). No se evidencio proceso de gestion de obsolescencia. | Analisis Financiero, Analisis Comercial | 2026-04-08 |
| Slotting | Pendiente de evaluacion | No se recogio evidencia suficiente sobre optimizacion de ubicaciones. Requiere entrevista con Orlando Rodriguez (Jefe Almacen, 11 abril). | — | — |
| Picking | Pendiente de evaluacion | No se recogio evidencia. Requiere entrevista con Jefe de Almacen. | — | — |
| Ubicacion y traslado | 2 | Operacion dispersa en 11-12 naves industriales arrendadas. Se mide tiempo de traspaso entre naves. Hay proyectos de optimizacion de layout. Pero la dispersion genera complejidad logistica interna significativa. Personal almacen MP: ~26 personas. | Rodolfo Vega, Marco Barcenas | 2026-04-08 |
| Diseno de almacen | 1 | 11-12 naves arrendadas sin diseno integrado de almacen. La dispersion es un constraint historico, no una decision optimizada. Se evidenciaron traslados de MP entre naves que generan paros de produccion. | Rodolfo Vega | 2026-04-08 |
| Recibo | 2 | Se mide tiempo de recibo (descarga de camion). Almacen de MP con ~26 personas. Pero calidad de MP que pasa al piso y genera paros sugiere que el proceso de recibo-inspeccion tiene gaps. | Rodolfo Vega | 2026-04-08 |
| KPIs y gobierno | 2 | Se miden: tiempo de recibo, traspaso entre naves, paros causados por almacen, productividad individual, capacidad de personal, danos a materiales, acomodo. Sin embargo, no se evidencio dashboard consolidado ni gestion por excepcion. | Rodolfo Vega | 2026-04-08 |

**Promedio:** 1.8 (sobre 5 evaluados)
**Laggers principales:**
- Dias de inventario se dispararon de ~17 a ~105 en un ano (+244%), con posible obsolescencia no provisionada de $50-100M
- Operacion dispersa en 11-12 naves sin diseno integrado — genera complejidad logistica interna y paros por falta de material en linea
- Sobreinventario cronico en automotriz: Abrillantador con 125 dias DDI (7x el ideal), algunos clubs con hasta 618 dias
- No se evidencio proceso de gestion de obsolescencia ni conteos ciclicos estructurados

**Best practices aplicables:**
- Exactitud de inventario >98% con conteos ciclicos diarios (frecuencia ABC)
- Dashboard de inventario en tiempo real: excesos, faltantes, cobertura, obsolescencia por SKU
- Inventario de seguridad calculado estadisticamente (no por regla de dedo) — urgente para productos temporales con 25% stockout rate
- Programa de reduccion de sobreinventario automotriz con decision formal de kill/reduce/discount
- Layout optimizado por perfil de movimiento (slotting analysis) considerando el constraint de naves multiples

---

## Pilar 10: Distribucion

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| Ultima milla | 3 | Fill rate 99.8% in-full (excelente cumplimiento). 176 tiendas Sam's servidas en toda la Republica desde 8 CEDIS. Camiones siempre van llenos (24-28 tarimas/trailer). Incidencias de robo minimas: 3 de 7,690 viajes. Unidad de venta es la tarima — no hay complejidad de picking de pedidos parciales. | Rodolfo Vega | 2026-04-08 |
| Capacidad y plan de flota | 2 | Modelo basado en transportistas terceros: ~80% hombre-camion (cartera de ~30, trabaja con ~15), ~20% backhaul Walmart. No hay flota propia. No se evidencio plan de flota a mediano plazo ni analisis de make-or-buy. | Rodolfo Vega | 2026-04-08 |
| Control de combustible | Pendiente de evaluacion | No es aplicable en la misma dimension — flota tercerizada. El costo de combustible esta embebido en la tarifa de flete. | — | — |
| Eficiencia de flota | 2 | Factor logistico 2025: 9.14% (meta: 8%, referencia historica: 5%). Erosion por: 2 anos sin incremento de precios, mix de destinos foraneos costosos (Merida >20%), mix de productos baratos. Se mide por destino. Subsidio cruzado entre destinos (Mexico/Chalco subsidian foraneos). | Rodolfo Vega | 2026-04-08 |
| TMS | 3 | Sistema de asignacion de transportistas digitalizado: asigna automaticamente segun regla de rotacion y notifica al transportista con cita (fecha, hora, carga). Tabulador de flete negociado anualmente. | Rodolfo Vega | 2026-04-08 |
| Seguimiento de rutas | 2 | No se evidencio GPS ni tracking en tiempo real de los transportistas terceros. Se mide cumplimiento por transportista con cargos por incidencias, danos en operacion. Pero sin visibilidad en ruta. | Rodolfo Vega | 2026-04-08 |
| Mantenimiento de flota | Pendiente de evaluacion | No aplica directamente — flota tercerizada. Se exige a transportistas cumplimiento legal completo (SAT, permisos, contrato con penalidades). | — | — |

**Promedio:** 2.4 (sobre 5 evaluados)
**Laggers principales:**
- Factor logistico 9.14% vs meta de 8% sobre ~$1,800M de facturacion = ~$20M de oportunidad anual
- 2 anos sin incremento de precios al cliente mientras costo de flete sube — erosion acumulativa de margen logistico
- On-time delivery ~50% (penalizado por entregas anticipadas, que tampoco es ideal para el cliente)
- Sin GPS ni tracking en tiempo real de transportistas terceros
- Sin analisis formal de make-or-buy (flota propia vs terceros por ruta/zona)

**Best practices aplicables:**
- Costo por tarima entregada como KPI central, desglosado por destino: hacer visible la erosion por mix geografico
- Negociacion inmediata de incremento de precios al cliente para recuperar al menos la inflacion acumulada de flete (2+ anos)
- Analisis de make-or-buy por ruta: backhaul Walmart es mas caro en foraneos — optimizar asignacion
- GPS/tracking en transportistas principales para visibilidad en ruta y ETA al cliente
- Proof of delivery digital para eliminar la discrepancia OTIF interno vs cliente

---

## Pilar 11: Digitalizacion / IT

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| Data analytics | 1 | Todos los analisis comerciales se hacen en Excel con archivos pesados que tardan en cargar. No existe Power BI ni herramientas de BI. Hugo construyo dashboards rudimentarios en 3 meses porque no existia nada. La plataforma Madrid (Retail Link de Sam's) no se explota. No existe infraestructura de Sales Intelligence. | Hugo Ambrosi | 2026-04-08 |
| Automatizacion | 1 | Reportes manuales. El reporte a direccion es una presentacion (PowerPoint) con indicadores mensuales — no hay dashboard en tiempo real. Proceso de captura de datos manual en produccion. No se evidencio RPA ni automatizacion de procesos. | Rodolfo Vega, Hugo Ambrosi | 2026-04-08 |
| Sistemas de informacion | 2 | ERP existe (no se especifico cual) para finanzas y operaciones basicas. Sistema de asignacion de transportistas digitalizado. CMMS migrando de MP v10 a Fractal. Pero mucho trabajo manual en paralelo al sistema. Excel como herramienta dominante para todo analisis. | Marco Barcenas, Rodolfo Vega | 2026-04-08 |
| IoT / Tech 4.0 | 1 | Cero IoT evidenciado en planta. No hay sensores de monitoreo de condicion en equipos. No hay captura automatica de datos de produccion. PLCs (si existen) no conectados a sistemas de informacion. | Rodolfo Vega | 2026-04-08 |
| Arquitectura de sistemas | Pendiente de evaluacion | No se recogio evidencia suficiente sobre la arquitectura de sistemas (integraciones, flujos de datos, infraestructura). Requiere entrevista con Gerente de TI. | — | — |
| Infraestructura de datos | Pendiente de evaluacion | No se evidencio data warehouse, data lake ni single source of truth. Cada area maneja sus propios archivos. Requiere entrevista con Gerente de TI. | — | — |

**Promedio:** 1.3 (sobre 4 evaluados)
**Laggers principales:**
- "Nuestro BI es Excel" — todo analisis en archivos pesados, sin Power BI ni dashboards automatizados
- Cero IoT en planta: no hay captura automatica de datos de produccion ni monitoreo de condicion de equipos
- Plataforma Madrid (Retail Link Sam's) no se explota — fuente de datos critica subutilizada
- Reportes manuales a direccion (PowerPoint mensual); no hay dashboards en tiempo real para ninguna area
- Migracion de CMMS bloqueada por licencias — unico proyecto de digitalizacion visible esta estancado

**Best practices aplicables:**
- Power BI como primera ola de digitalizacion: conectar datos de ventas (Sam's Retail Link), produccion y financieros en dashboards automatizados
- Single source of truth para KPIs del negocio — eliminar versiones multiples de la verdad
- Roadmap de digitalizacion con business case por proyecto, priorizado por ROI
- Explotar plataforma Madrid: con un analista de Sales Intelligence se pueden generar insights de pricing, quiebres, desarrollo de categoria
- Resolver tema de licencias de Fractal como quick win para habilitar digitalizacion de mantenimiento

---

## Pilar 12: Estructura, Gobierno y Capital Humano

| Sub-modulo | Nivel | Evidencia | Fuente | Fecha eval. |
|------------|-------|-----------|--------|-------------|
| Desarrollo de lideres | 2 | Hugo trae mentalidad de empresa grande (10 anos PepsiCo) y esta intentando implementar procesos. Rodolfo tiene 21 anos de experiencia como pilar institucional. Pero no se evidencio programa formal de desarrollo de lideres, coaching ni plan de sucesion. Vacantes criticas (Gte. Produccion, Jefe Produccion, Gte. Compras) sin cubrir. | Hugo Ambrosi, Rodolfo Vega | 2026-04-08 |
| Manejo del cambio | 2 | Hugo esta impulsando cambio en el area comercial (de cero estructura a CPFR, KAM, dashboards). Pero no se evidencio modelo de cambio formal ni comunicacion estructurada. "Anteriormente era literal asi, con el dedo. Y no, asi no funciona." Resistencia implicita: el KAM Klaus no funciono en <3 meses; equipo de perfiles "coordinador hacia abajo". | Hugo Ambrosi | 2026-04-08 |
| Gobierno operativo | 2 | Existe reporte mensual a direccion con indicadores (produccion, fill rate, paros, calidad, personal). Pero decisiones altamente centralizadas en 1-2 personas. David Padilla (DGA) tomo decision unilateral que costo ~$400M/ano. No hay comite comercial con reglas de escalamiento. No se evidenciaron tier meetings formales. Organigrama con errores (faltaban jefaturas, lineas de reporte equivocadas). | Marco Barcenas, Rodolfo Vega | 2026-04-08 |
| Indicadores de gestion | 2 | KPIs existen para produccion (paros, cumplimiento, fill rate) y para finanzas (costo estandar, inflacion interna, P&L detallado). Pero no hay metas formales para todos, no hay cascadeo, no hay BSC. Cada area mide lo suyo sin vision integrada. El indicador mas critico — productividad de MO — no existe. | Marco Barcenas, Rodolfo Vega | 2026-04-08 |
| Gestion de talento | 1 | Vacantes criticas sin cubrir: Gte. Produccion, Jefe Produccion, Gte. Compras (cronico). KAM de Sam's fallido en <3 meses. "La gran mayoria de los perfiles son coordinador hacia abajo. Muchos no llegan ni analista ni coordinador." Sin plan de sucesion para personas clave (Marco, Rodolfo). Rodolfo sin asistente. | Hugo Ambrosi, Rodolfo Vega | 2026-04-08 |
| Compensacion variable | Pendiente de evaluacion | No se discutio esquema de incentivos ni comisiones del equipo comercial. No se recogio evidencia de compensacion variable ligada a KPIs. | — | — |
| Cultura organizacional | 2 | Cultura informal definida por la familia fundadora. Politica de bienestar (solo turno matutino L-V para mujeres operarias). Centralismo extremo: Marco revisa "el detalle de todo, 100%". Las decisiones se toman por el dueno/director. Hugo: "Data antes que opinion" como filosofia nueva, pero la cultura historica es de gestion "con el dedo". | Marco Barcenas, Hugo Ambrosi, Rodolfo Vega | 2026-04-08 |

**Promedio:** 1.8 (sobre 6 evaluados)
**Laggers principales:**
- Centralizacion extrema: Marco revisa 100% del detalle financiero Y negocia con proveedores Y gestiona compras estrategicas. Rodolfo sostiene toda la operacion con 21 anos de conocimiento. Riesgo persona-clave critico
- Vacantes cronicas en posiciones clave: Gte. Produccion, Jefe Produccion, Gte. Compras (han rotado varios sin exito)
- Decision unilateral de David Padilla (DGA) costo ~$400M/ano — ausencia de gobierno corporativo en la gestion de la relacion con el cliente ancla
- Sin plan de sucesion para roles criticos; sin BSC ni cascadeo de indicadores
- Perfiles del equipo en general de bajo calibre: "coordinador hacia abajo"

**Best practices aplicables:**
- Tier meetings formales: T1 diaria en piso (15 min), T2 semanal gerencial (1 hr), T3 mensual directiva (2 hrs), T4 trimestral estrategica
- Plan de sucesion inmediato para las 3-4 posiciones mas criticas (Marco, Rodolfo, Aide Gomez); cobertura urgente de vacantes
- BSC con cascadeo desde estrategia hasta indicadores operativos; KPIs por area con meta, frecuencia y responsable
- Comite comercial formal con reglas de escalamiento — para que nunca mas una decision individual ponga en riesgo la operacion
- Programa de desarrollo de lideres: identificar talento con potencial para cubrir gaps y construir capa intermedia de gestion

---

## Historial de Actualizaciones

| Fecha | Evento | Pilares actualizados |
|-------|--------|---------------------|
| 2026-04-08 | Creacion del documento. Evaluacion pendiente — requiere reprocesar entrevistas y documentos con criterios CMM. | — |
| 2026-04-08 | Primera evaluacion completa. Procesadas 3 entrevistas (Marco Barcenas Dir. Finanzas 18-mar, Hugo Ambrosi Dir. Comercial 06-abr, Rodolfo Vega Dir. Operaciones 08-abr) + 2 analisis (financiero detallado, comercial detallado Sam's). Se evaluaron 64 de 80 sub-modulos totales. Promedio general: 1.9. | 01, 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, 12 |
