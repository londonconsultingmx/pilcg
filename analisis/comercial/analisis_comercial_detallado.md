# Análisis Comercial Detallado — Ventas Piso & Formato de Stock
## PI Group SA de CV | Project Shine | LCG MX
**Fecha de análisis:** 8 abril 2026
**Fuentes:** Ventas Piso.xlsx (13 MB), Formato de Stock.xlsx (38 MB)
**Período cubierto:** Febrero 2025 — Abril 2026 (Sam's Club fiscal weeks W01-W52 2025 + W01-W09 2026)

---

## 1. Resumen Ejecutivo

Estos dos archivos contienen la totalidad de la operación comercial de PI Group con Sam's Club México: ventas sell-through por SKU/semana (Ventas Piso) e inventarios/stock en piso por club/SKU (Formato de Stock). **Toda la data es exclusivamente de Sam's Club** — no hay un solo registro de otro cliente, lo cual confirma la concentración absoluta del canal.

### Hallazgos críticos para el fondo:

1. **Sell-through anual 2025: $2,361 MM MXN** a precio de retail en Sam's Club (~$1,850-1,950 MM a precio de fábrica estimado).
2. **Run-rate 2026 plano vs 2025** (+0.7% semanal), sin crecimiento orgánico visible.
3. **$648.5 MM MXN en SKUs cancelados** durante el período — transiciones masivas de portafolio en curso.
4. **$149 MM MXN en productos descontinuados sin reemplazo directo** (Lavanda, Pino, Ropa Oscura).
5. **El costo de los nuevos SKUs de Detergente es 12% mayor** que los que reemplazan — presión directa sobre margen.
6. **Fill rate promedio: 95.2%** con caídas severas a 65-75% en 5+ semanas del año — pérdida de venta evitable.
7. **Sobreinventario crónico en Automotriz**: Desengrasante y Abrillantador con +90 días de inventario promedio, vs. ideal de 18 días.
8. **Top 5 SKUs = 65.1% de la venta** — concentración extrema dentro de un portafolio ya concentrado en un solo cliente.

---

## 2. Descripción de las Fuentes

### 2.1 Ventas Piso.xlsx (13.3 MB)

| Hoja | Registros | Descripción |
|------|-----------|-------------|
| **Data Base** | 8,668 | Datos raw de sell-through (ventas + unidades por SKU, fecha, semana) |
| **Hoja Trabajada** | 30,060 | Data enriched: ventas, unidades, semana, status, forecast, YoY, categoría |
| **Artículos** | 32 | Catálogo maestro de SKUs: pricing, costo, margen, litraje, pzs/tarima |
| Sheet4 / Sheet1 | Pivots | Tablas resumen (ventas por producto, por semana) |
| DashBoard | 127 | Dashboard visual (referencias a pivots) |
| Calendario | 764 | Calendario de semanas fiscales Sam's (dic 2024 — ene 2027) |

**Hoja clave:** "Hoja Trabajada" — contiene la data principal con 30,060 registros de sell-through.

### 2.2 Formato de Stock.xlsx (39.8 MB)

| Hoja | Registros | Descripción |
|------|-----------|-------------|
| **Data Base** | 33,332 | Inventario por SKU/club: OH (on-hand), OO (on-order), pipeline, DDI, forecast, in-stock |
| **Datos de la Tabla \| SOH** | 5,500 | Stock on-hand por SKU/club con variación vs período anterior |
| **DT Sell Out** | 25,759 | Sell-out semanal por SKU/club (10 semanas: W52/2025 — W09/2026) |
| **SO 52W** | 2,597 | Sell-out histórico 52 semanas por combinación SKU-club |
| **FR** | 15 | Fill rate semanal por producto (52 semanas) |
| **Combinaciones Activas** | 2,594 | Combinaciones SKU-club activas |
| **Club's 25** | 184 | Directorio completo de clubs Sam's (con CEDIS, estado, gerente) |
| **Artículos** | 32 | Catálogo maestro (duplicado del otro archivo con campos adicionales) |
| **Score** | 30 | Scorecard consolidado: in-stock, FR, OH, OO, DDI por producto |
| Nivelación | 147 | Cálculos de nivelación/reabasto por CEDIS y producto |
| Días de Inventario | 185 | Histórico de DDI |
| Otros (8 hojas) | Varios | Pivots, mapas, forecasts intermedios |

---

## 3. Análisis de Ventas (Sell-Through)

### 3.1 Ventas Totales por Año

| Métrica | 2025 (52 sem) | 2026 (W01-W09) | 2026 anualizado |
|---------|--------------|----------------|-----------------|
| Ventas retail (MXN MM) | $2,361.0 | $411.7 | ~$2,378* |
| Unidades | 14,886,395 | 2,735,880 | ~15,818,000* |
| Promedio semanal (MXN MM) | $45.4 | $45.7 | — |

*Anualización simple sobre 9 semanas. El run-rate semanal de 2026 es apenas 0.7% superior al de 2025 — **crecimiento esencialmente nulo.**

**Nota:** 2026 incluye semanas W48-W52 con ~$198 MM adicionales que corresponden al cierre del año fiscal Sam's (ene-feb 2026) mapeado a calendar year 2025. La data total 2026 en el archivo suma $629.2 MM.

### 3.2 Ventas por Producto (2025 + 2026 YTD)

| # | Producto | Ventas (MXN MM) | % Total | % Acumulado | Unidades | Precio Prom/Ud | Status |
|---|----------|----------------|---------|-------------|----------|---------------|--------|
| 1 | Detergente 10L | $511.6 | 17.1% | 17.1% | 2,365,275 | $216 | Transición |
| 2 | Lavatrastes 2.9L | $498.9 | 16.7% | 33.8% | 6,046,298 | $83 | Activo |
| 3 | Detergente 20L | $349.5 | 11.7% | 45.5% | 819,991 | $426 | Transición |
| 4 | Suavizante 10L | $347.2 | 11.6% | 57.1% | 1,990,550 | $174 | Transición |
| 5 | Suavizante 20L | $240.7 | 8.0% | 65.1% | 711,343 | $338 | Transición |
| 6 | Temporal (limpiadores) | $230.3 | 7.7% | 72.8% | 1,694,124 | $136 | Mixto |
| 7 | Baños y Azulejos 5+1L | $150.9 | 5.0% | 77.8% | 933,789 | $162 | Activo |
| 8 | Blanqueador 20L | $117.5 | 3.9% | 81.7% | 623,303 | $188 | Activo |
| 9 | Desengrasante Bipack 5+1L | $98.6 | 3.3% | 85.0% | 648,050 | $152 | Activo |
| 10 | Limpiador de Vidrios 5+1L | $82.6 | 2.8% | 87.8% | 733,931 | $113 | Activo |
| 11 | Quitamanchas 10L | $77.9 | 2.6% | 90.4% | 382,968 | $203 | Activo |
| 12 | Desengrasante Concentrado 10L | $73.1 | 2.4% | 92.8% | 315,780 | $231 | Activo |
| 13 | Lavanda 10L | $62.0 | 2.1% | 94.9% | 509,512 | $122 | **CANCELADO** |
| 14 | Shampoo Automotriz 10L | $34.3 | 1.1% | 96.0% | 211,998 | $162 | Transición |
| 15 | Pino 10L | $29.5 | 1.0% | 97.0% | 215,195 | $137 | **CANCELADO** |
| 16 | Ropa Oscura 10L | $23.4 | 0.8% | 97.8% | 117,118 | $200 | **CANCELADO** |
| 17 | Lavanda 20L | $20.2 | 0.7% | 98.5% | 85,936 | $235 | **CANCELADO** |
| 18 | Desengrasante Automotriz 5L | $17.7 | 0.6% | 99.1% | 139,773 | $126 | Activo |
| 19 | Pino 20L | $14.3 | 0.5% | 99.6% | 48,598 | $294 | **CANCELADO** |
| 20 | Abrillantador Automotriz 5+1L | $10.0 | 0.3% | 99.9% | 52,075 | $191 | Activo |

### 3.3 Concentración de Producto (Pareto)

- **Top 3 productos = 45.5% de la venta** (Detergente 10L + Lavatrastes + Detergente 20L)
- **Top 5 productos = 65.1%** (+ Suavizante 10L y 20L)
- **Top 10 productos = 87.8%**

**Implicación:** Dentro de un negocio ya mono-cliente (Sam's Club), la venta se concentra en 5 SKUs de commodity (detergente, lavatrastes, suavizante). Una pérdida de cualquiera de estos SKUs tendría impacto catastrófico.

### 3.4 Análisis por Categoría

| Categoría | Ventas (MXN MM) | % Total | Productos |
|-----------|----------------|---------|-----------|
| Detergentes | $861.2 | 28.8% | Det. 10L + Det. 20L |
| Suavizantes | $587.9 | 19.7% | Suav. 10L + Suav. 20L |
| Lavatrastes | $498.9 | 16.7% | Lavatrastes 2.9L |
| Especialidades Limpieza | $483.1 | 16.2% | Baños, Vidrios, Desg. Bipack, Conc., Quitamanchas |
| Temporales/Promocional | $230.3 | 7.7% | Limpiadores temporales |
| Limpiadores Descontinuados | $126.0 | 4.2% | Lavanda, Pino (cancelados) |
| Superficies (Blanqueador) | $117.5 | 3.9% | Blanqueador 20L |
| Automotriz | $61.9 | 2.1% | Shampoo, Desengrasante, Abrillantador |
| Especialidades Lavandería | $23.4 | 0.8% | Ropa Oscura (cancelado) |

**Hallazgo clave:** Detergentes + Suavizantes + Lavatrastes = 65.2% de la venta. Son commodities de bajo margen. Las Especialidades (16.2%) tienen mejores márgenes pero menor escala.

---

## 4. Análisis de Márgenes y Precios

### 4.1 Margen Comercial Sam's (margen del retailer, no de PI Group)

| Producto | Margen Sam's | Precio Retail | Costo a Sam's | Costo/Litro |
|----------|-------------|---------------|--------------|-------------|
| Limpiador Brisa de Mar 10L | 25.9% | $142 | $90.69 | $9.07 |
| Limpiador Lavanda 10L (CANC) | 25.9% | $142 | $90.69 | $9.07 |
| Desengrasante Multiusos 5+1L | 25.1% | $163 | $114.71 | $19.12 |
| Desengrasante Automotriz 5L | 23.2% | $149 | $98.63 | $19.73 |
| Blanqueador 20L | 18.9% | $216 | $150.98 | $7.55 |
| Quitamanchas 10L | 18.7% | $228 | $159.89 | $15.99 |
| Suavizante 10L (CANC) | 15.5% | $199 | $145.02 | $14.50 |
| Suavizante 20L (CANC) | 15.1% | $392 | $286.85 | $14.34 |
| Shampoo Automotriz 10L | 14.9% | $169 | $124.05 | $12.40 |
| Lavatrastes 2.9L | 14.8% | $98.99 | $72.75 | $25.09 |
| Ropa Oscura 10L (CANC) | 14.8% | $200 | $170.50 | $17.05 |
| Abrillantador 5+1L | 14.6% | $199 | $146.54 | $24.42 |
| Pino 10L (CANC) | 13.8% | $156 | $115.96 | $11.60 |
| Pino 20L (CANC) | 13.3% | $345 | $257.73 | $12.89 |
| Detergente 20L (CANC) | 12.9% | $442 | $332.01 | $16.60 |
| Detergente 10L Azul (CANC) | 12.7% | $233 | $175.30 | $17.53 |

**Nota:** Estos son los márgenes de Sam's Club sobre el producto PI Group. El margen de PI Group sobre su costo de producción es diferente y no está en estos archivos.

### 4.2 Revenue por Litro (precio de retail)

| Rango | Productos | Rev/Litro |
|-------|-----------|-----------|
| Alto ($25+) | Abrillantador, Lavatrastes, Baños, Deseng. Bipack, Deseng. Auto | $25-32/L |
| Medio ($15-25) | Detergentes, Quitamanchas, Ropa Oscura, Deseng. Concentrado, Limpiador Vidrios | $15-22/L |
| Bajo (<$15) | Suavizantes, Shampoo Auto, Pino, Temporal, Lavanda, Blanqueador | $9-17/L |

**Promedio ponderado: $19.14/litro.** Blanqueador es el producto con menor valor por litro ($9.42/L) — básicamente agua con cloro en volumen masivo.

### 4.3 Impacto de Transiciones de SKU en Costos

Las transiciones de Detergente (azul -> blanco) implican un **incremento de costo del 12%:**

| Producto | Costo Anterior | Costo Nuevo | Incremento |
|----------|---------------|-------------|------------|
| Detergente 10L | $175.30 | $196.34 | +$21.04 (+12.0%) |
| Detergente 20L | $332.01 | $371.85 | +$39.84 (+12.0%) |

**Impacto estimado:** Con ~2.4M unidades de Det. 10L y ~820K de Det. 20L anuales, el incremento de costo es de ~$50-83 MM MXN/año que se absorbe entre PI Group y Sam's. Esto erosiona directamente el margen si no se ajusta el precio de venta.

---

## 5. Análisis de SKUs Cancelados y Portafolio en Transición

### 5.1 Magnitud de las Cancelaciones

| SKU Cancelado | Venta 2025 (MXN MM) | Unidades | Tiene Reemplazo |
|---------------|---------------------|----------|-----------------|
| Detergente 10L (Azul) | $157.4 | 770,238 | Si (Blanco, +12% costo) |
| Temporal (varios) | $114.7 | 852,229 | Parcial (rotación de temporales) |
| Detergente 20L (antiguo) | $99.8 | 256,830 | Si (nuevo, +12% costo) |
| Suavizante 10L (antiguo) | $76.4 | 458,573 | Si (nuevo, mismo costo) |
| Lavanda 10L | $62.0 | 509,512 | **No directo** |
| Suavizante 20L (antiguo) | $50.8 | 153,386 | Si (nuevo, mismo costo) |
| Pino 10L | $29.5 | 215,195 | **No** |
| Ropa Oscura 10L | $23.4 | 117,118 | **No** |
| Lavanda 20L | $20.2 | 85,936 | **No** |
| Pino 20L | $14.3 | 48,598 | **No** |
| **TOTAL** | **$648.5** | — | — |

### 5.2 Productos Sin Reemplazo

**$149.4 MM MXN en ventas anuales de retail de productos discontinuados sin reemplazo directo:**

- Lavanda 10L ($62.0 MM) — parcialmente cubierto por Brisa de Mar (limpiador temporal)
- Pino 10L ($29.5 MM) — sin reemplazo
- Ropa Oscura ($23.4 MM) — sin reemplazo
- Lavanda 20L ($20.2 MM) — sin reemplazo
- Pino 20L ($14.3 MM) — sin reemplazo

**Riesgo:** Si estos productos no se reemplazan, Sam's Club podría asignar ese espacio en anaquel a competidores. El "TEMPORAL" parece ser el mecanismo de reemplazo parcial (limpiadores estacionales de $230 MM anuales), pero no cubre el formato 20L ni la categoría Ropa Oscura.

### 5.3 Status del Portafolio Actual

De los 20 productos con venta (excluyendo Muestra):
- **12 SKUs ACTIVOS** = $1,737 MM (58% de venta)
- **8 SKUs CANCELADOS** = $648 MM (22% de venta)
- **Temporal (mixto)** = $230 MM (8% activo, 8% cancelado)

**El 22% de la venta está en SKUs en proceso de cancelación/transición.** Esto genera riesgo operativo significativo durante el proceso de switchover.

---

## 6. Análisis de Tendencia (YoY)

### 6.1 Comparación Semana por Semana (mismas semanas W01-W09)

| Producto | 2025 (MXN MM) | 2026 (MXN MM) | Cambio YoY |
|----------|--------------|--------------|------------|
| Lavatrastes | $102.8 | $116.5 | **+13.3%** |
| Detergente 10L | $132.4 | $111.1 | **-16.1%** |
| Suavizante 10L | $79.7 | $83.1 | +4.3% |
| Detergente 20L | $82.3 | $72.2 | **-12.3%** |
| Suavizante 20L | $53.7 | $54.2 | +0.9% |
| Temporal | $47.3 | $49.8 | +5.4% |
| Baños y Azulejos | $31.9 | $33.3 | +4.4% |
| Blanqueador | $25.3 | $23.5 | -7.3% |
| Quitamanchas | $19.8 | $16.5 | **-16.8%** |
| Abrillantador | $2.7 | $2.1 | **-20.5%** |
| Lavanda 10L | $58.7 | $0.0 | **-100%** |
| Pino 10L + 20L + Lavanda 20L + Ropa Oscura | $115.6 | $0.0 | **-100%** |

**Total comparable: $788.7 MM (2025) vs $629.2 MM (2026) = -20.2% decline.**

**Pero:** La caída se explica principalmente por las discontinuaciones. Excluyendo productos cancelados sin reemplazo, el comparable es más cercano a -5% a -8%.

### 6.2 Productos en Crecimiento
- **Lavatrastes +13.3%** — el SKU más robusto, 100% club coverage, sin transiciones
- **Temporal +5.4%** — compensando parcialmente las discontinuaciones
- **Suavizante 10L +4.3%** — transición exitosa al nuevo SKU

### 6.3 Productos en Declive (excluyendo cancelados)
- **Detergente 10L -16.1%** — impactado por la transición azul→blanco
- **Detergente 20L -12.3%** — mismo fenómeno de transición
- **Quitamanchas -16.8%** — declive orgánico preocupante
- **Abrillantador -20.5%** — categoría automotriz en contracción

### 6.4 Estacionalidad (2025, ventas mensuales MXN MM)

| Mes | Ventas | Índice |
|-----|--------|--------|
| Enero | $241.2 | 1.23 |
| Febrero | $193.5 | 0.98 |
| Marzo | $247.7 | 1.26 |
| Abril | $178.6 | 0.91 |
| Mayo | $189.3 | 0.96 |
| Junio | $172.7 | 0.88 |
| Julio | $178.9 | 0.91 |
| Agosto | $192.5 | 0.98 |
| Septiembre | $177.3 | 0.90 |
| Octubre | $183.6 | 0.93 |
| Noviembre | $184.7 | 0.94 |
| Diciembre | $220.9 | 1.12 |

**Picos en enero y marzo** (inicio de año fiscal Sam's + temporada de limpieza de primavera). **Valle en junio-septiembre.** Estacionalidad moderada (rango 0.88-1.26x).

---

## 7. Análisis de Inventarios y Stock en Piso

### 7.1 Inventario On-Hand por Producto

| Producto | OH (unidades) | OO (pedido) | Pipeline Total | DDI Promedio | DDI Ideal |
|----------|--------------|-------------|---------------|-------------|-----------|
| Lavatrastes | 287,249 | 110,376 | 397,625 | 23.7 | 18 |
| Detergente 10L | 109,485 | 22,440 | 131,925 | 21.5 | 18 |
| Suavizante 10L | 92,669 | 30,361 | 123,030 | 21.6 | 18 |
| Baños y Azulejos | 53,332 | 11,484 | 64,816 | 31.2 | 18 |
| Limpiador Vidrios | 45,907 | 9,512 | 55,419 | 34.8 | 18 |
| Detergente 20L | 38,806 | 6,912 | 45,718 | 26.2 | 18 |
| Desengrasante Bipack | 35,482 | 11,252 | 46,734 | 36.0 | 18 |
| Suavizante 20L | 33,614 | 10,560 | 44,174 | 25.6 | 18 |
| Blanqueador | 30,956 | 6,336 | 37,292 | 29.9 | 18 |
| Desengrasante Auto | 23,365 | 6,552 | 29,917 | **96.3** | 18 |
| Desengrasante Conc. | 22,202 | 6,180 | 28,382 | 45.4 | 18 |
| Quitamanchas | 22,104 | 4,740 | 26,844 | 29.6 | 18 |
| Shampoo Auto | 19,670 | 8,800 | 28,470 | 51.5 | 18 |
| Abrillantador Auto | 13,993 | 1,392 | 15,385 | **125.2** | 18 |
| Temporal | 4,514 | 48,150 | 52,664 | 13.0 | 18 |

### 7.2 Sobreinventario Crónico (Banderas Rojas)

**Productos con DDI promedio > 3x el ideal (>54 días):**

| Producto | DDI Promedio | DDI Max | % Clubs con DDI > 30 | Diagnóstico |
|----------|-------------|---------|----------------------|-------------|
| Abrillantador Auto | **125 días** | 618 días | 98.6% | Sobreinventario masivo |
| Desengrasante Auto | **96 días** | 519 días | 98.8% | Sobreinventario masivo |
| Shampoo Auto | **52 días** | 205 días | 90.9% | Sobreinventario significativo |

**Toda la categoría Automotriz tiene sobreinventario crónico.** El Abrillantador tiene 125 días de inventario promedio (7x el ideal de 18 días). Algunos clubs tienen hasta **618 días** de inventario — casi 2 años.

**Implicación financiera:** El sobreinventario genera:
- Capital de trabajo atrapado
- Riesgo de devoluciones/destrucción
- Señal de que Sam's podría reducir pedidos futuros o cancelar SKUs

### 7.3 Subinventario (Riesgo de Desabasto)

| Producto | DDI Promedio | % Clubs con stockout | Riesgo |
|----------|-------------|---------------------|--------|
| Temporal | 13.0 | 25.3% | Alto — 1 de 4 clubs sin stock |

Los productos temporales/estacionales tienen un modelo de reabasto deficiente: 25% de stockout rate indica pérdida de venta significativa.

### 7.4 OH/Forecast Ratio (semanas de cobertura)

| Producto | OH | FCST Semanal | Semanas de Cobertura |
|----------|-----|-------------|---------------------|
| Lavatrastes | 287,249 | 10,866 | **26.4 semanas** |
| Detergente 10L | 109,485 | 7,401 | **14.8 semanas** |
| Suavizante 10L | 92,669 | 9,455 | 9.8 semanas |
| Temporal | 4,514 | 12,072 | **0.4 semanas** |

**Lavatrastes tiene 26 semanas de cobertura** (6 meses) — sobreinventario importante. En contraste, Temporal tiene menos de medio semana de cobertura — desabasto sistemático.

---

## 8. Análisis de Fill Rate

### 8.1 Fill Rate Promedio por Producto

| Producto | FR Promedio (52 sem) | Clasificación |
|----------|---------------------|---------------|
| Desengrasante Concentrado 10L | 98.1% | Bueno |
| Desengrasante Bipack 5+1L | 97.9% | Bueno |
| Limpiador Vidrios 5+1L | 97.9% | Bueno |
| Blanqueador 20L | 97.3% | Bueno |
| Baños y Azulejos 5+1L | 96.6% | Aceptable |
| Quitamanchas 10L | 96.5% | Aceptable |
| Shampoo Auto 10L | 95.3% | Aceptable |
| **Promedio total** | **95.2%** | **Aceptable** |
| Lavatrastes 2.9L | 94.8% | Aceptable |
| Suavizante 20L | 94.6% | Aceptable |
| Suavizante 10L | 94.2% | Mejorable |
| Desengrasante Auto 5L | 94.1% | Mejorable |
| Detergente 10L | 94.0% | Mejorable |
| Abrillantador 5+1L | 91.8% | **Deficiente** |
| Detergente 20L (Color) | 89.1% | **Deficiente** |

### 8.2 Semanas Críticas de Fill Rate

El fill rate cae por debajo de 80% en 5 semanas del año:

| Semana | FR Promedio | Contexto Probable |
|--------|-----------|-------------------|
| W47 | **65.4%** | Pre-navidad |
| W35 | **75.1%** | Fin de agosto |
| W22 | **75.3%** | Fin de mayo |
| W48 | **75.7%** | Navidad-Año Nuevo |
| W21 | **79.4%** | Mayo |

**Estas 5 semanas representan ~$225 MM en ventas.** Con un fill rate de ~75% vs. el 95% promedio, la pérdida de venta estimada es de **$45-55 MM MXN/año por desabastos estacionales.**

### 8.3 Fill Rate Reciente (Score Sheet, últimas 4 semanas)

| Producto | In-Stock | FR Período | Estado |
|----------|----------|-----------|--------|
| Lavatrastes | 100% | 98.8% | OK |
| Suavizante 10L | 100% | 100.0% | OK |
| Detergente 10L | 100% | 99.9% | OK |
| Desengrasante Conc. | 100% | 96.8% | Alerta menor |
| Baños y Azulejos | 100% | 98.5% | OK |
| Blanqueador | 100% | 99.7% | OK |

---

## 9. Análisis de Distribución Geográfica

### 9.1 Red de Distribución Sam's Club

| CEDIS | OH (unidades) | # Clubs | % del inventario |
|-------|--------------|---------|-----------------|
| SMO (CDMX) | 220,103 | 48 | 25.7% |
| Guadalajara | 145,692 | 28 | 17.0% |
| Chalco | 128,854 | 25 | 15.1% |
| Monterrey | 85,891 | 20 | 10.0% |
| Culiacán | 73,418 | 16 | 8.6% |
| Chihuahua | 70,479 | 15 | 8.2% |
| Villahermosa | 57,014 | 13 | 6.7% |
| Mérida | 55,014 | 11 | 6.4% |

**Total: 176 clubs activos** en 32 estados, atendidos desde 8 CEDIS de Sam's.

### 9.2 Top Estados por Inventario

| Estado | OH (unidades) | # Clubs |
|--------|--------------|---------|
| Estado de México | 94,760 | 23 |
| Ciudad de México | 92,616 | 17 |
| Jalisco | 66,410 | 11 |
| Nuevo León | 45,389 | 11 |
| Veracruz | 36,897 | 7 |
| Sonora | 36,089 | 8 |

**EdoMex + CDMX = 21.9% del inventario** — concentración en el Valle de México coherente con densidad de clubs.

### 9.3 Clubs con Sobreinventario

| Club | DDI Promedio | Diagnóstico |
|------|-------------|-------------|
| SM Morelia Reforma | 75.8 | Sobreinventario severo |
| SM GDL Mariano Otero | 70.3 | Sobreinventario severo |
| SM Ecatepec Centro | 68.9 | Sobreinventario severo |
| SM Tuxpan | 65.7 | Sobreinventario severo |
| SM Santa Elena | 61.6 | Sobreinventario |
| SM Delicias | 61.5 | Sobreinventario |

15 clubs tienen DDI promedio > 55 días (3x el ideal). Estos clubs probablemente devuelven producto o requieren ajuste en el modelo de reabasto.

---

## 10. Análisis de Volumen Físico

### 10.1 Volumen Total

- **Litros vendidos (2025 + 2026 YTD): 156.2 millones de litros**
- **Promedio ponderado: $19.14 MXN/litro** a precio de retail

### 10.2 Concentración de Volumen

| Producto | Litros (MM) | % Volumen | % Venta |
|----------|------------|-----------|---------|
| Detergente 10L | 23.7 | 15.1% | 17.1% |
| Suavizante 10L | 19.9 | 12.7% | 11.6% |
| Lavatrastes 2.9L | 17.5 | 11.2% | 16.7% |
| Temporal 10L | 16.9 | 10.8% | 7.7% |
| Detergente 20L | 16.4 | 10.5% | 11.7% |
| Suavizante 20L | 14.2 | 9.1% | 8.0% |
| Blanqueador 20L | 12.5 | 8.0% | 3.9% |

**Blanqueador ocupa 8% del volumen pero solo 3.9% de la venta** — producto de alto volumen / bajo valor ($9.42/L) que ocupa capacidad de producción, almacenamiento y transporte de forma desproporcionada.

---

## 11. Banderas Rojas y Anomalías

### BANDERA 1: Portafolio en Transición Masiva
- **22% de la venta ($648 MM) en SKUs cancelados.** Esto es una reestructuración de portafolio mayor, no una transición menor.
- Los nuevos detergentes cuestan 12% más, comprimiendo margen.
- 5 productos (~$149 MM) cancelados sin reemplazo directo.

### BANDERA 2: Categoría Automotriz en Declive con Sobreinventario
- Ventas cayendo 10-20% YoY en los 3 SKUs automotrices.
- Inventario de 96-125 días (5-7x el ideal).
- Solo 2.1% de la venta total — candidata a racionalización o discontinuación.
- Sam's podría forzar devoluciones o cancelar la categoría.

### BANDERA 3: Fill Rate con Caídas Severas
- 5 semanas/año con FR < 80% = ~$45-55 MM en venta potencial perdida.
- Patrón estacional sugiere problemas de planeación de producción, no de demanda.
- El FR de Detergente Color (89.1%) y Abrillantador (91.8%) están consistentemente por debajo del benchmark.

### BANDERA 4: Dependencia de Productos Temporales como Parche
- $230 MM en "Temporales" (7.7% de venta) — limpiadores estacionales que rotan sabores.
- 25% de stockout rate en clubs — el modelo de reabasto no funciona para estos SKUs.
- Parecen usarse para cubrir el espacio de Lavanda/Pino discontinuados, no como estrategia deliberada.

### BANDERA 5: Sobreinventario de Lavatrastes
- 26 semanas de cobertura (6 meses de inventario).
- Es el SKU #2 en venta y #1 en unidades — cualquier ajuste de inventario genera devoluciones masivas.
- Contrasta con Temporal que tiene 0.4 semanas (3 días).

### BANDERA 6: Crecimiento Cero
- Run-rate semanal 2026 vs 2025: +0.7% — esencialmente plano.
- Ajustando por inflación (~5% anual), hay **contracción real de ~4%.**
- Sin nuevo producto o nuevo canal, no hay motor de crecimiento.

---

## 12. Implicaciones para el Inventario de Oportunidades

### OPP-001 (Refinamiento): Reducción de Devoluciones
Los sobreinventarios (Automotriz, Lavatrastes) son precursores de devoluciones. Un modelo de reabasto optimizado podría reducir devoluciones en $20-40 MM.

### OPP-005 (Refinamiento): Diversificación de Clientes
Estos archivos confirman que PI Group opera como un **proveedor cautivo** de Sam's Club. No hay visibilidad de ventas a otros canales. La data de "Ventas Piso" ES el Retail Link de Sam's — PI Group ve la venta de su producto a nivel de tienda individual.

### OPP-NEW-A: Optimización de Portafolio (Racionalización Automotriz)
- Eliminar o reducir Abrillantador ($10 MM venta, 125 días inventario) y Desengrasante Automotriz ($17.7 MM, 96 días).
- Liberar espacio en anaquel para productos de mayor rotación/margen.
- Impacto: Reducción de capital de trabajo atrapado + mejora en mix de margen.

### OPP-NEW-B: Mejora de Fill Rate en Semanas Críticas
- Las 5 semanas con FR < 80% generan $45-55 MM en pérdida de venta estimada.
- Requiere ajuste en planeación de producción y acumulación de inventario pre-temporada.
- Quick win con impacto directo en top line.

### OPP-NEW-C: Captura de Margen en Transición de Detergentes
- El costo nuevo es 12% mayor. Si PI Group no renegociaba precio con Sam's, absorbe toda la erosión.
- Detergentes = $861 MM en venta. Un 12% de impacto en costo sobre el ~60% que es materia prima = ~$60 MM en erosión de margen potencial.
- Oportunidad de renegociación o reformulación.

### OPP-NEW-D: Rebalanceo de Inventario
- Reducir OH de Lavatrastes (de 26 a 12 semanas = liberar ~143K unidades).
- Incrementar OH de Temporal (de 0.4 a 4 semanas).
- Impacto: Mejora en fill rate de Temporales + liberación de capital de trabajo.

---

## 13. Datos Pendientes para Validar

| Dato | Fuente Requerida | Pilar |
|------|-----------------|-------|
| Ventas a otros clientes (no Sam's) | Dir. Comercial (Hugo Ambrosi) | 01, 02 |
| Margen bruto de PI Group (no margen de Sam's) | Dir. Finanzas (Marco Bárcenas) | 01 |
| Razón de cancelación de Lavanda/Pino/Ropa Oscura | Dir. Comercial o I+D | 01, 07 |
| Plan de reemplazo para productos discontinuados | Dir. Comercial | 01, 02 |
| Impacto de transición Detergente en precio a Sam's | Dir. Comercial / Finanzas | 01, 08 |
| Costo de producción por SKU (no costo a Sam's) | Dir. Operaciones / Finanzas | 04, 08 |
| Devoluciones históricas por producto | Dir. Comercial / Logística | 02, 06 |
| Plan de racionalización Automotriz | Dir. Comercial | 01 |
| Capacidad de producción por línea/producto | Dir. Operaciones | 03, 04 |
| Nivel de OTIF a CEDIS Sam's | Dir. Logística | 02, 10 |

---

## 14. Conexión con Pilares del Modelo Macro LCG

| Hallazgo | Pilar(es) |
|----------|-----------|
| Portafolio en transición masiva (22% cancelado) | 01 Inteligencia Comercial, 07 Innovación |
| Concentración en 5 SKUs = 65% venta | 01 Inteligencia Comercial |
| Concentración 100% Sam's Club | 01 Inteligencia Comercial, 02 Ejecución Comercial |
| Crecimiento real negativo (~-4%) | 01 Inteligencia Comercial |
| Fill rate con caídas estacionales a 65-75% | 02 Ejecución Comercial, 03 Planeación |
| Incremento 12% en costo Detergentes nuevos | 07 Innovación, 08 Abastecimiento |
| Sobreinventario Automotriz (96-125 DDI) | 09 Almacenes, 02 Ejecución Comercial |
| Subinventario Temporales (0.4 sem cobertura) | 03 Planeación, 09 Almacenes |
| 156M litros/año producidos y distribuidos | 04 Producción, 10 Distribución |
| Discontinuación de $149 MM sin reemplazo | 07 Innovación, 01 Intel. Comercial |

---

*Análisis generado a partir de datos extraídos programáticamente de ambos archivos Excel. Todas las cifras de venta son a precio de retail Sam's Club (sell-through). Para obtener la venta neta de PI Group, se requiere aplicar el margen de Sam's (12-26% según producto).*
