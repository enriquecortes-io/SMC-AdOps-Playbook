# SMC Official Ad Platform Knowledge Base

Documentación oficial y verificada de Meta Ads y Google Ads para campañas de Santa María Collection.

## META ADS (Facebook, Instagram, Audience Network)

### Estructura de Campañas
- **Campaign Level**: Objetivo publicitario (conversión, tráfico, reconocimiento)
- **Ad Set Level**: Audiencia, ubicación, presupuesto, pujas, horarios
- **Ad Level**: Creatividad, copy, CTA, landing page

### Objetivos de Campaña
- **Awareness**: Reconocimiento de marca
- **Consideration**: Tráfico a web, leads, visualización de contenido
- **Conversion**: Compras, leads cualificados, reservas

### Audiencias
- **Core Audience**: Intereses, comportamientos, demografía específica
- **Custom Audience**: Email lists, phone numbers, retargeting
- **Lookalike Audience**: Similar a 1-10% de tu mejor audiencia

### Formatos Publicitarios
- Single Image (1200x628px recomendado)
- Video (mínimo 1080p, 15-120 segundos)
- Carousel (5-10 cards)
- Collection (3 productos + cover)
- Stories (1080x1920px vertical)
- Reels (9:16 vertical)

### Pixel de Meta
- Evento de Vista de Página
- Evento de Lead
- Evento de Compra/Reserva
- Custom Conversions basado en URL

### Estrategia de Pujas
- Lowest Cost (automática)
- Cost Cap (máximo costo por conversión)
- ROAS Target (retorno objetivo)
- Bid Cap (máximo costo por acción)

### Políticas y Restricciones
- Máximo 125 caracteres en titular
- Máximo 27 caracteres en copy principal (Facebook)
- Máximo 30 caracteres en CTA
- Prohibido: antes/después, comparativas falsas, contenido sensacional
- Real estate: documentos de propiedad, licencia, autorización requerida

### Capacidades Avanzadas
- Conversions API: Seguimiento servidor-side
- Lead Ads: Formularios nativos en plataforma
- Dynamic Ads: Retargeting con catálogo de propiedades
- Test & Learn: Experimentos controlados con holdout groups

---

## GOOGLE ADS

### Estructura de Campañas
- **Campaign Level**: Tipo (Search, Display, Video), presupuesto, geo-targeting
- **Ad Group Level**: Keywords, anuncios relacionados, pujas
- **Ad Level**: Titular, descripción, URL final, URL de display

### Tipos de Campañas

#### Search
- Search Network (búsquedas de Google)
- Display Network (sitios asociados)
- Keywords: Broad, Phrase Match, Exact Match, Broad Match Modifier
- Quality Score: 1-10 (impacta CPC y posición)

#### Display
- Audiencias: Custom Intent, Custom Affinity, In-market, Demographics
- Placements: Sitios específicos o redes temáticas
- Formatos: Text, Image, Rich Media (300x250, 728x90, 160x600)

#### Video
- YouTube In-stream (antes, durante, después de video)
- YouTube Bumper Ads (6 segundos)
- Display Video (formato responsive)

#### App Campaigns
- Instalaciones o engagement en apps

### Extensiones de Anuncios
- Sitelink: Enlaces adicionales a páginas internas
- Callout: Puntos de venta clave (15-25 caracteres)
- Structured Snippet: Categorías de productos/servicios
- Call Extension: Número de teléfono directo
- Location Extension: Ubicación física
- Price Extension: Precios de productos
- Promotion Extension: Descuentos y ofertas

### Seguimiento y Conversiones
- Google Ads Conversion Tracking: pixel universal
- Global Site Tag (gtag.js)
- Event Tracking: conversiones personalizadas
- Importar conversiones desde Google Analytics 4

### Estrategias de Pujas (Google Search)
- Manual CPC: Control total de pujas
- Enhanced CPC: Ajustes automáticos hasta 30%
- Target CPA: Costo objetivo por conversión
- Target ROAS: Retorno objetivo
- Maximize Clicks: Volumen máximo
- Maximize Conversions: Conversiones máximas

### Calidad y Relevancia
- Quality Score (1-10): Impacta CPC y posición de anuncio
- Expected CTR: Histórico vs. esperado
- Ad Relevance: Relevancia anuncio-keyword
- Landing Page Experience: Velocidad, relevancia, móvil

### Políticas de Google Ads
- Real estate requiere verificación de empresa
- Prohibido: Propiedad subasta, timeshares no autorizados
- Documentación: Licencia, acreditación, proof of entity
- Prohibido en ciertos países/regiones

### Remarketing (Retargeting)
- Standard Remarketing: Display ads a visitantes previos
- Dynamic Remarketing: Anuncios personalizados con productos vistos
- Video Remarketing: Anuncios en YouTube
- Customer Match: Retarget email lists

### Google Shopping (si aplica)
- Requiere Google Merchant Center
- Catálogo de propiedades con precios, imágenes, descripción

---

## SEGUIMIENTO Y MEDICIÓN

### Métricas Clave
- **Impressions**: Veces que se mostró el anuncio
- **Clicks**: Clics totales en el anuncio
- **CTR**: Porcentaje de clics (Clicks/Impressions)
- **CPC**: Costo promedio por click
- **Conversions**: Acciones completadas (leads, reservas, contactos)
- **CPA**: Costo por acción/conversión
- **ROAS**: Retorno sobre gasto publicitario
- **CAC**: Costo de adquisición de cliente

### Atribución
- Last-click: Última interacción antes de conversión
- First-click: Primer touchpoint
- Linear: Peso igual a todos touchpoints
- Time-decay: Mayor peso a última interacción

### UTM Parameters
- utm_source=google (o facebook, etc)
- utm_medium=cpc (o cpm, organic)
- utm_campaign=smc-miami-q3
- utm_content=ad_variant_name
- utm_term=keyword_name (Google Search)

---

## CAPACIDADES AVANZADAS POR PLATAFORMA

### Meta: Conversions API
- Envía eventos servidor-side directamente a Meta
- Mejora tracking offline y móvil
- Aumenta volumen y precisión de datos
- Requiere implementación técnica

### Google: Enhanced Conversions
- Enriquece datos de conversión con información de cliente
- Mejor atribución y modelado
- Requiere hash seguro de email/teléfono

### Google: AI-Powered Solutions
- Smart Bidding: Máquina aprende y optimiza pujas
- Performance Max: Campaña única, múltiples formatos y canales
- Demand Gen: Audience + creative + automation

### Meta: Advantage+ Shopping Ads
- Upload catálogo + creatividades
- Meta optimiza automáticamente
- Múltiples formatos en una campaña

---

## COMPLIANCE Y PRIVACIDAD

### Privacy Changes
- iOS 14.5+: ATT (App Tracking Transparency)
- Privacy Sandbox: Chrome, cookies de terceros en fase out
- GDPR, CCPA: Consentimiento explícito requerido
- Conversions API: Solución recomendada para tracking post-ATT

### Documentación Requerida (Real Estate)
- Proof of entity (LLC, Inc, etc)
- Business license or registration
- Property authorization letter (si promocionas propiedad de tercero)
- Compliance with local real estate regulations

---

## RECURSOS OFICIALES

- Meta Business Suite: business.facebook.com
- Google Ads Help Center: support.google.com/ads
- Meta Ads Manager Learning Hub: facebook.com/business/learning
- Google Ads Academy: skillshop.withgoogle.com
- Documentación de APIs: developers.facebook.com, developers.google.com
