# 05A — ANDRÓMEDA (META ADS): REGLAS OPERATIVAS

**Fuentes:**
- Atria, "Andromeda Meta Ads: The Creative Strategy Guide for 2026" (27 abr 2026), con datos técnicos del Meta Engineering Blog (2 dic 2024).
- Confect, "Meta Andromeda — The ultimate guide to Meta Ads in 2026" (10 mar 2026). Estudio sobre 3.014 anunciantes e-commerce. Sesgo: vende anuncios de catálogo; datos correlacionales. Solo se extrae lo aplicable a lead gen inmobiliario (sección 12).
- 6thMan, "Meta Andromeda" (PDF comercial, sin datos ni fuentes). Solo se extrae la definición de variedad real en vídeo y el diseño sin sonido (sección 4).
- Ayuda de Meta Business, fase de aprendizaje (vía fuentes secundarias, 2026).
**Extracción:** 29 sept 2026. Solo contenido operativo; excluida toda referencia a productos de las empresas emisoras.
**Sustituye a:** documento `Andromeda Meta` (borrado; ver sección 13).

-----

## 1. QUÉ ES Y DÓNDE ACTÚA

Andrómeda es el motor de **recuperación de anuncios** de Meta, presentado a finales de 2024 y desplegado globalmente en octubre de 2025. Actúa **antes** de la subasta, no dentro de ella.

```
FASE 1 — RECUPERACIÓN (Andrómeda)
Decenas de millones de anuncios elegibles → ~1.000 candidatos por usuario, en <300 ms
       │
       ▼
FASE 2 — RANKING (subasta clásica)
eCPM, CTR previsto, probabilidad de conversión → 1 anuncio gana la impresión
```

**Consecuencia crítica:** si un anuncio no pasa la Fase 1, la puja, la segmentación y el presupuesto son irrelevantes. Nunca llega a competir.

**Cambio de pregunta:**
- Antes: ¿a quién le enseño este anuncio? (lógica de audiencia)
- Ahora: ¿qué anuncio le enseño a esta persona concreta ahora? (lógica de creatividad)

Datos de Meta: modelos de recuperación 10.000x más complejos, +6% de recall y +8% de calidad de anuncios en segmentos seleccionados.

-----

## 2. EL ENTITY ID — EL CONCEPTO QUE LO GOBIERNA TODO

Andrómeda agrupa los anuncios por **similitud semántica** en un árbol jerárquico. Los anuncios conceptualmente iguales reciben **un único Entity ID** = una sola entrada en la recuperación.

- 50 variantes del mismo gancho y la misma oferta = 1 Entity ID = 50 anuncios peleando por 1 plaza.
- 10 conceptos distintos = 10 entradas independientes.

La red neuronal detecta similitud a nivel de **idea**, no solo visual. No crean un Entity ID nuevo:
- Cambiar el color o el texto del titular
- Cambiar una palabra
- Cambiar la música de fondo
- Cambiar el formato (vídeo / imagen / carrusel) del mismo concepto

|                 |CONCEPTO (Entity ID nuevo)                      |VARIACIÓN (mismo Entity ID)                  |
|-----------------|------------------------------------------------|---------------------------------------------|
|Qué es           |Ángulo, gancho o buyer persona distinto         |Retoque cosmético de un concepto existente   |
|Ejemplo          |Anuncio de dolor vs. aspiracional vs. prueba social|Titular A vs. titular B del mismo anuncio de dolor|
|Efecto           |Gana una entrada propia en la recuperación      |Compite consigo mismo por una entrada        |
|Qué hacer        |Producir más                                    |Limitar; testear dentro del concepto         |

**Regla:** la diversidad creativa es la nueva segmentación. No le dices a Meta a quién llegar; le das señales distintas para que lo descubra.

Cada interacción es una señal sobre el perfil del usuario (guardar ≠ clic ≠ ver el 90% del vídeo). Un solo ángulo = señal estrecha. Muchos conceptos = datos de comportamiento diversos = mejor modelo de quién compra.

-----

## 3. ESTRUCTURA DE CAMPAÑA

**Por defecto:** 1 campaña por objetivo + segmentación amplia + Advantage+ (ubicaciones) + presupuesto a nivel de campaña (CBO).

**Por qué consolidar:**
- Cada conjunto de anuncios es un problema de aprendizaje separado → la señal se divide y cada uno tarda más en aprender.
- Varios conjuntos apuntando a los mismos usuarios → solapamiento: pujas contra ti mismo y sube el coste.

**Cuándo SÍ se justifican varias campañas / conjuntos:** objetivos realmente distintos — prospección vs. retargeting, mercados distintos, etapas del embudo con eventos de conversión distintos.

**Test:** ¿sirven a propósitos distintos, o son audiencias distintas para el mismo propósito? Si es lo segundo → consolidar.

**Segmentación amplia:** mínima acumulación de intereses, sin restricciones demográficas estrechas. El algoritmo encuentra a los compradores mejor que las audiencias manuales, pero solo si le dejas explorar.

-----

## 4. VOLUMEN Y PRODUCCIÓN CREATIVA

**Punto de partida:** 5-10 conceptos realmente distintos por campaña. Cada uno con una estrategia de mensaje diferente, p. ej.:
- Uno que abre con un dolor concreto
- Uno de prueba social
- Uno de transformación / resultado
- Uno que responde a una objeción frecuente

Definir desde el principio qué intenta **probar** cada concepto.

**Qué cuenta como concepto distinto en un Reel (checklist de grabación):** tiene que cambiar el conjunto, no un elemento suelto:
- Escena / localización
- Gancho de los primeros 3 segundos
- Guion
- Voz / quién habla o cómo se dirige al espectador
- Ritmo de montaje
- Ángulo psicológico

El mismo guion grabado en otro sitio, o el mismo Reel con otro texto encima, probablemente cae en el mismo Entity ID.

**Diseño sin sonido:** cada Reel debe entenderse con el audio apagado (texto en pantalla o subtítulos en los tramos clave). Nunca overlay manual y subtítulo automático en el mismo tramo.

**Diversidad de formato (dentro de cada concepto):** vídeo + imagen estática + carrusel. Comparten Entity ID, pero permiten a Meta probar entrega en ubicaciones y contextos distintos. Advantage+ reparte entre superficies solo si le das formatos con los que trabajar. Exportar nativo en 9:16, 4:5 y 1:1.

**Ritmo de refresco:** Andrómeda detecta la fatiga antes que el sistema anterior. Revisión cada **2-3 semanas** en campañas de prospección activas. Cuando cae el *First-Time Impression Ratio* → conceptos nuevos, no variantes del mismo. (Las guías de e-commerce piden 10-30 creatividades/mes y refresco semanal; no es realista para una operación de una persona.)

-----

## 5. DATOS DE CONVERSIÓN

Andrómeda entrena con resultados de conversión. Datos incompletos = modelo sesgado de quién compra = entrega a la gente equivocada, por buena que sea la creatividad.

**Mínimo técnico:**
1. Píxel en todos los eventos clave
2. Conversions API (CAPI) enviando espejo server-side de esos eventos
3. Deduplicación confirmada (que no se cuente dos veces)

-----

## 6. MÉTRICAS NUEVAS EN ADS MANAGER

|Métrica                     |Qué indica                                              |Acción                                  |
|----------------------------|--------------------------------------------------------|----------------------------------------|
|Creative Similarity         |Parecido entre anuncios del mismo conjunto. Alto = probable Entity ID único|Si es alto → reconstruir conceptos      |
|Creative Fatigue / Ad Fatigue|El anuncio se ha mostrado demasiado a los mismos usuarios|Refrescar con concepto nuevo            |
|Top Creative Themes         |Qué tipos de creatividad reciben más presupuesto        |Informar qué producir después           |
|First-Time Impression Ratio |% de impresiones a usuarios que no lo habían visto      |Si cae → refresco                       |

-----

## 7. PROTOCOLO DE TESTING

- **Testear conceptos, no variantes.** Titular A vs. B sobre el mismo mensaje = dos entradas para el mismo asiento.
- Una hipótesis clara por test. Una variable.
- Mínimo **~1.000 impresiones por concepto** antes de concluir.
- Mínimo **5-7 días** de ejecución antes de declarar ganador. Andrómeda da señal antes, pero la varianza temprana no es insight.
- Registrar cada resultado en un log compartido.

-----

## 8. PRESUPUESTO Y FASE DE APRENDIZAJE

- Meta necesita **~50 eventos de optimización por conjunto de anuncios en una ventana móvil de 7 días** tras la última edición significativa.
- **No es acumulado:** 50 leads en un mes no sacan del aprendizaje. Caer por debajo de 50 en cualquier ventana de 7 días puede devolver al aprendizaje.
- **Se cuenta por conjunto de anuncios, no por campaña.** Cada conjunto necesita sus propios 50.
- **Reinician el contador:** cambios de presupuesto >20%, de segmentación, de estrategia de puja o de evento de optimización.
- **Presupuesto mínimo por conjunto** = (CPL objetivo × 50) / 7.
- **"Aprendizaje limitado"** = Meta prevé que no llegarás a 50. No significa que el anuncio sea malo ni que deje de entregar: optimiza de forma más conservadora. Si el coste y la calidad del lead a 30 días son buenos, se mantiene.
- 10 $/día raramente da señal suficiente. Punto de partida según Atria: **30-50 $/día por campaña**.
- **No se puede desactivar el aprendizaje ni hacer segmentación manual** (además, la categoría Vivienda la restringe). Con presupuesto bajo, ver sección 14.

-----

## 9. CHECKLIST PRE-LANZAMIENTO / REVISIÓN

**Estructura**
- [ ] 1 campaña por objetivo de conversión
- [ ] Segmentación amplia, sin apilar intereses
- [ ] Ubicaciones Advantage+ activas
- [ ] Presupuesto a nivel de campaña (CBO)

**Creatividad**
- [ ] Mínimo 5 conceptos distintos, cada uno con gancho y propuesta de valor propios
- [ ] Cada concepto cambia escena, gancho, guion, voz, ritmo y ángulo (no solo uno)
- [ ] Cada Reel se entiende con el sonido apagado
- [ ] Al menos 1 vídeo, 1 imagen estática y 1 carrusel
- [ ] Cada pieza exportada nativa en 9:16, 4:5 y 1:1
- [ ] Creative Similarity revisado; si es alto, reconstruir

**Tracking**
- [ ] Píxel en eventos clave
- [ ] CAPI activo con espejo server-side
- [ ] Deduplicación confirmada

**Refresco y escalado**
- [ ] Revisión creativa cada 2-3 semanas
- [ ] First-Time Impression Ratio vigilado
- [ ] Conceptos, no variantes; 1 hipótesis por test; 5-7 días mínimo

-----

## 10. IMPACTO EN EL SETUP ACTUAL DE SOLENA (análisis propio, no de la fuente)

|Setup actual                                             |Choque con Andrómeda                                                                 |
|---------------------------------------------------------|-------------------------------------------------------------------------------------|
|AS1 = 1 Reel + 3 textos del mismo ángulo Autoridad        |Es **1 concepto = 1 Entity ID**. Los 3 textos son variaciones, no suman entradas.   |
|€20/día en AS1                                           |50 leads/semana exigiría CPL ≈ €2,80 (€140/50). Casi seguro queda en "aprendizaje limitado". |
|Plan 50/30/20 entre 3 conjuntos                          |Divide una señal ya insuficiente en tres. Cada conjunto aún más lejos del umbral.   |
|AS2/AS3 = retargeting de visionado ≥50% (excl. leads)    |Justificado por la fuente (retargeting ≠ prospección), pero con €20/día las audiencias serán muy pequeñas. |
|Formato "imagen o vídeo único", sin carrusel             |Falta diversidad de formato dentro de cada concepto.                                 |
|Categoría especial Vivienda                               |A favor: ya obliga a segmentación amplia (lo que Andrómeda pide).                   |
|Formulario instantáneo (lead ads), no web                 |Los eventos de píxel e-commerce no aplican. El equivalente es devolver la calidad del lead a Meta vía CAPI desde el CRM (conecta con el proyecto de server-side tracking). |

**Tensión de fondo con el framework de ciclos angulares:** el ciclo impone un **orden** de ángulos (Autoridad → Coste → Confianza) mediante retargeting. Andrómeda rinde mejor con **varios conceptos juntos** en una estructura consolidada, pero no garantiza orden. La regla "un impacto = un ángulo" sí encaja perfectamente con la lógica de Entity ID. Decisión pendiente: secuencia forzada con poco presupuesto vs. consolidación con más señal.

-----

## 11. DECISIONES DERIVADAS PARA SOLENA

1. AS1 en Aprendizaje limitado es lo esperable con €20/día. Juzgarlo por coste y calidad del lead a 2-4 semanas, no por el estado de aprendizaje. Editar lo mínimo.
2. Reels 2 y 3: meterlos en el mismo conjunto que el Reel 1 (o subir presupuesto), no en conjuntos separados que dividan los €20/día.
3. Producir conceptos nuevos cada 2-3 semanas (ver sección 12), aplicando el checklist de variedad real de la sección 4.
4. Exportar cada Reel en 9:16, 4:5 y 1:1 nativos, entendible sin sonido.

-----

## 12. APRENDIZAJES DEL ESTUDIO CONFECT (aplicables a inmobiliario)

|Hallazgo                                                                 |Aplicación                                                          |
|-------------------------------------------------------------------------|--------------------------------------------------------------------|
|1 conjunto con 25 creatividades distintas: +17% conversiones y −16% coste vs. 5 conjuntos (test controlado de Five Nine Strategy)|Consolidar. No fragmentar en AS1/AS2/AS3 con presupuesto bajo.     |
|Vida útil de un anuncio: de 6-8 semanas a 2-4 semanas                    |Calendario de producción: conceptos nuevos cada 2-3 semanas. Los 3 Reels actuales caducan ≈ mediados de octubre 2026.|
|Los anuncios alcanzan su pico en la semana 1 y luego se estancan         |En e-commerce: cambiar si no rinde en 1 semana. **En Solena NO aplica** con €20/día: 1 semana de leads es ruido. Mantener 2-4 semanas.|
|Productos de gama alta: −17% ROAS. El tráfico es más frío y el ticket alto necesita confianza y varios impactos|Refuerza los ciclos con retargeting para TEM. Un solo impacto no basta en lujo.|
|Páginas de categoría como destino: −24%. Ficha de producto y home mejoran|Web TEM: anuncios a `/listings/[propiedad]/` o a la home, nunca a `/propiedades/[zona]/`.|
|Imagen/vídeo único: −17%. Carrusel y colección aguantan mejor            |Probar carrusel dentro de cada concepto.                            |
|Creatividades diseñadas nativas por ubicación (1:1, 4:5, 9:16) rinden mejor que recortadas|Exportar cada Reel en 9:16, 4:5 y 1:1 nativos. Trabajo de edición, no de grabación.|
|Segmentación amplia: +49% ROAS vs. lookalikes (dato Lebesgue)            |La categoría Vivienda ya obliga a amplia.                           |
|Los mejores anunciantes tienen más anuncios activos, pero volumen sin diversidad no sirve (clustering)|Más conceptos, no más variantes.                                   |

**KPIs nuevos a añadir al seguimiento:**
- Número de anuncios activos (conceptos distintos en circulación)
- Ritmo de refresco (conceptos nuevos lanzados por mes)
- Tasa de conversión post-clic (formulario / web)

**Pendiente de verificar:** Meta tiene anuncios dinámicos de inmuebles (catálogo de listings). Podría dar diversidad creativa a TEM sin grabar más. Comprobar compatibilidad con la categoría especial Vivienda en la UE.

**No aplicable:** anuncios de catálogo de e-commerce, reglas de diseño, product assets, tamaño de catálogo, puja por ROAS, Advantage+ Shopping.

-----

## 13. REVISIÓN DEL DOCUMENTO ANTERIOR (`Andromeda Meta`, borrado)

- **Fecha "octubre 2025":** correcta. Anuncio técnico y cuentas piloto a finales de 2024; despliegue global completado en octubre 2025.
- **Variantes = hooks distintos del mismo reel:** según la lógica de Entity ID, cambiar solo el gancho de texto del mismo reel probablemente cae en el mismo cluster. Lo que suma son conceptos distintos.
- **"ROAS +7-22%":** cifra sin fuente. No usar.
- **Reels "esperanza / miedo / referral":** desactualizado; el setup vigente es Autoridad / Coste / Confianza.

-----

## 14. OPCIONES CON PRESUPUESTO BAJO (≈ €20/día) — análisis propio, sin decidir

**Opción A — Mantener lead ads y medir por resultado.**
Aceptar "Aprendizaje limitado". Juzgar por CPL y calidad del lead (zona + P2 del formulario) a 2-4 semanas. Si el CPL es asumible y los leads son de zona, funciona.

**Opción B — Optimizar por un evento barato y convertir a mano.**
- AS1 optimizado por reproducciones de vídeo (ThruPlay) en lugar de leads. Evento barato → supera los 50/semana → Meta aprende de verdad.
- Conversión fuera de la prospección: conjunto pequeño de formulario solo a quien vio el vídeo + WhatsApp + orgánico.
- Encaja con los ciclos angulares: Meta distribuye barato, la persuasión se hace en el retargeting y en la conversación directa.
- Coste: Meta optimiza para gente que ve vídeos, no para propietarios que venden. La calidad depende de que el gancho del Reel filtre (dirigido explícitamente a propietarios).

**Criterio:** no tocar AS1 hasta tener ~2 semanas de datos (≈ 11 oct 2026). Si el CPL no compensa → probar Opción B.

**Recordatorio:** Meta no debe ser el único canal. Con poco presupuesto, referenciadores, portales y contacto directo suelen dar leads más baratos.
