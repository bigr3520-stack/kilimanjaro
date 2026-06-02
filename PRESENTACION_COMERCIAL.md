# Kilimanjaro — Propuesta de Rediseño Web

## Para: Franco y Rodrigo (dueños de Kilimanjaro Tienda de Cultivo)
## De: Nebari Design

---

## La situación actual

Hoy la página está hecha con **WordPress + WooCommerce + Divi**. El WordPress funciona bien como tienda (gestión de productos, carrito, pagos), pero el frontend tiene varios problemas:

- **Lento**: Divi carga mucho CSS/JS que no se usa, penalizando el SEO
- **Genérico**: El diseño no se diferencia de otros grow shops
- **Sin identidad visual fuerte**: Los colores del logo (verde #00cc66, rosado #e84393, amarillo #f5c542) no se aprovechan
- **Baja conversión**: Sin CTAs claros ni elementos de prueba social
- **Sin analytics**: No hay forma de medir lo que funciona

---

## La solución: Landing page + WordPress de fondo

Creamos una **landing page moderna y disruptiva** que se conecta con el WordPress existente. El WordPress sigue manejando la tienda, el blog y los productos. La landing page es la puerta de entrada que convierte visitantes en consultas de WhatsApp.

### Qué cambió

| Aspecto | Antes (WordPress + Divi) | Después (Landing page) |
|---|---|---|
| Velocidad | Lento (Divi pesado) | Carga instantánea (CSS puro, sin frameworks) |
| Diseño | Genérico | Oscuro + colores del logo + animaciones |
| WhatsApp | Botón básico | 7 puntos de contacto + tracking |
| SEO | Básico | Schema.org (Store, Product, FAQ, WebSite) |
| Analytics | Ninguno | GA4 con eventos por cada clic |
| Móvil | Aceptable | Sticky CTA, menú overlay, diseño responsive |

---

## Lo que hicimos concreto

### Diseño visual
- Dark theme (#0d1117) con acentos del logo (verde, rosado, amarillo)
- Preloader animado con logo "K"
- Partículas flotantes en hero
- Barra de progreso de scroll con gradiente
- Animaciones de entrada (scroll reveal, parallax)
- Cursor custom con efecto de diferencia
- Carrusel infinito de testimonios y badges de confianza

### Copywriting pensado
- "De cultivadores / para cultivadores. / Sin vueltas." — posicionamiento directo
- Copy local argentino, sin frases genéricas de IA
- Testimonios reales que suenan auténticos
- FAQ que elimina objeciones antes de que surjan

### SEO al día
- Schema markup: LocalBusiness, WebSite (con SearchAction), Product (con AggregateOffer), FAQPage
- Meta tags optimizados
- Alt texts descriptivos en todas las imágenes
- Headings jerarquizados correctamente (H1 → H2 → H3)
- Preconnect + dns-prefetch al WordPress
- Preload de imagen hero con fetchpriority high

### Analytics listo para activar
- Google Analytics 4 incorporado (solo falta el ID real)
- Eventos de dataLayer en cada interacción clave:
  - Clics en WhatsApp (header, hero, productos, about, flotante, sticky)
  - Clics en "Explorar tienda"
  - Consultas de producto
  - Compras de producto
  - Suscripciones a newsletter
  - Clics en blog y catálogo

### CRO aplicado (conversión)
- **Prueba social**: Contador de productos, categorías, notificación de compra en vivo
- **CTAs estratégicos**: WhatsApp en 7 lugares distintos, cada uno con su propio tracking
- **Sticky CTA mobile**: Siempe visible mientras scrolleás
- **FAQ eliminando objeciones**: Envíos, stock, pagos, horarios
- **Urgencia**: Badges de "Más vendido", "Nuevo", "Oferta"

---

## Cómo funciona la integración

```
Usuario entra → Landing page (GitHub Pages)
                    ↓
            Clica en producto → Va al WordPress a la página del producto
            Clica en categoría → Va al WordPress a la categoría
            Clica en blog → Va al WordPress al artículo
            Clica en WhatsApp → Abre chat directo con tracking
```

El WordPress **no se toca**. La landing page es una capa frontal que redirige al WordPress cuando es necesario.

---

## Lo que necesitamos de ustedes

### 1. Google Analytics ID (gratis, lo creás vos)
- Ir a https://analytics.google.com
- Crear propiedad → obtener el ID (formato G-XXXXXXXXX)
- Nos lo pasás y lo activamos en 2 minutos

### 2. Hosting definitivo (opcional)
Hoy está hosteado en GitHub Pages (gratis). Si quieren algo propio, se puede migrar fácil.

---

## Hosting actual y demo

La página ya está online y funcionando en:

**https://bigr3520-stack.github.io/kilimanjaro**

Si quieren verla en vivo, abran ese link desde el celular y desde la compu.

---

## Próximos pasos posibles

Ya implementado:
- Landing page completa con todas las secciones
- Analytics con tracking de eventos
- SEO y schema markup
- Diseño responsive
- Hosting gratuito en GitHub Pages

Para una segunda etapa podríamos sumar:
- **PWA (Progressive Web App)**: La página se puede "instalar" como app en el celu
- **Formulario de contacto web** (hoy todo va por WhatsApp)
- **Buscador de productos** en la misma landing
- **Términos y condiciones / Legales**
- **Página de "gracias por tu compra"**

---

## En resumen

- ✅ Diseño moderno, dark theme, colores del logo
- ✅ Carga rápida (sin frameworks pesados)
- ✅ SEO optimizado (Schema, metas, headings)
- ✅ Analytics listo (GA4 con eventos)
- ✅ Copy pensado para el público argentino
- ✅ Hosteado y funcionando
- ❌ Solo falta tu ID de Google Analytics

Estamos listos para cuando quieran dar el paso.

---

**Contacto técnico:** Nebari Design
**Repositorio:** https://github.com/bigr3520-stack/kilimanjaro
