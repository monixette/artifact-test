# Taller: Chatbots con IA en tu Sitio Web
## Contenido para Google Slides

> Cada bloque `---` representa un slide.
> Los textos están listos para copiar-pegar.
> Las notas del presentador van al final de cada slide.

---

## SLIDE 1 — Portada

**Eyebrow:** TALLER INTERACTIVO · LIFESTRATEGICS 2026

**Título:**
Chatbots con IA en tu Sitio Web

**Subtítulo:**
De Custom GPTs a plataformas embebibles: cómo crear un asistente que responda con tu conocimiento y viva en tu página.

**Visual sugerido:** fondo oscuro, partículas, logo LifeStrategics

---

## SLIDE 2 — Agenda

**Título:** ¿Qué vamos a ver hoy?

| # | Bloque | Tiempo |
|---|---|---|
| 🧠 | Entender RAG | 15 min |
| 🌳 | Árboles de decisión | 15 min |
| 🛠️ | Opciones y herramientas | 15 min |
| 🚀 | Ejercicio práctico | 30 min |

---

## SLIDE 3 — ¿Qué hay detrás de un chatbot "inteligente"?

**Número de sección:** 01 · COMPRENDER

**Título:** ¿Qué hay detrás de un chatbot "inteligente"?

**Texto:**
Cuando un chatbot responde sobre TU negocio, no es magia — es una técnica llamada RAG (Retrieval Augmented Generation).

**Notas del presentador:**
Explicar que RAG no es entrenar una IA desde cero (eso cuesta millones). Es darle un "cheat sheet" con tu información cada vez que alguien pregunta.

---

## SLIDE 4 — RAG: Los 4 pasos

**Título:** Cómo funciona RAG

**4 columnas / bloques:**

| Paso | Icono | Título | Descripción |
|---|---|---|---|
| 1 | 📄 | Ingestión | Tus PDFs, FAQs, manuales se "pican" en fragmentos y se convierten en vectores numéricos |
| 2 | 🔍 | Búsqueda | Cuando alguien pregunta, el sistema busca fragmentos relevantes por significado (no palabras exactas) |
| 3 | 📋 | Contexto | Los fragmentos encontrados se inyectan en el prompt: "responde con base en esto" |
| 4 | 💬 | Respuesta | La IA genera una respuesta natural usando esos fragmentos como fuente |

---

## SLIDE 5 — Analogía RAG

**Título:** Piénsalo así...

**Texto principal:**
Imagina que contratas a un asistente super inteligente que nunca ha trabajado en tu empresa.

Le das un manual de tu negocio y le dices: "cuando te pregunten algo, primero busca en este manual."

**Eso es RAG:** dar contexto específico a una IA general.

**Punto clave:**
No estás "entrenando" una IA desde cero. Estás dándole un cheat sheet cada vez que alguien pregunta. Por eso puedes actualizar la información sin re-entrenar nada.

---

## SLIDE 6 — Árboles de decisión: dos modos

**Número de sección:** 02 · DECIDIR

**Título:** Árboles de decisión: guiando al usuario

**Texto intro:**
Un chatbot inteligente combina dos modos: rutas predefinidas (árbol lógico) y consultas abiertas (lenguaje natural). Lo ideal es tener ambos.

---

## SLIDE 7 — Modo 1 vs Modo 2

**Layout:** dos columnas

**Columna izquierda — MODO 1 · ÁRBOL LÓGICO**

🌳 Rutas predefinidas

El chatbot guía al usuario con opciones tipo botón:
"¿Qué necesitas?" → "Precios" / "Fases" / "Soporte"

- Experiencia controlada y predecible
- Ideal para flujos de soporte
- Reduce errores de interpretación
- El usuario no necesita saber qué preguntar

**Columna derecha — MODO 2 · LENGUAJE NATURAL**

💬 Consultas abiertas

El usuario escribe libremente: "¿cuánto cuesta la Fase 2?" y el chatbot busca en tu base de conocimiento (RAG).

- Flexibilidad total para el usuario
- Maneja preguntas impredecibles
- Requiere buena base de conocimiento
- Respuestas más naturales y conversacionales

---

## SLIDE 8 — La combinación ganadora

**Título:** 🎯 La combinación ganadora

**Texto:**
Un chatbot profesional ofrece ambos modos.

Al iniciar, presenta botones con las opciones principales (árbol).
Pero si el usuario prefiere escribir, el RAG responde igualmente.

Esto cubre el 100% de los escenarios.

---

## SLIDE 9 — Ejemplo: Árbol de IDEOFACTO

**Título:** Ejemplo interactivo: árbol de navegación

**Diagrama de árbol (puede ser visual):**

```
¿En qué puedo ayudarte?
├── 📋 Fases y precios
│   ├── 🎴 Kit de tarjetas — $500 MXN
│   ├── 📋 Fase 1 — $3,000 MXN
│   ├── 📐 Fase 2 — $5,000 MXN
│   └── 🎬 Fase 3 — desde $3,500/módulo
├── 🎯 ¿Es para mí?
│   ├── ✅ Sí, tengo negocio propio → Recomendación
│   └── 🤔 Prefiero delegar → Nota honesta
└── ❓ Otra pregunta → Búsqueda RAG en el FAQ
```

**Notas del presentador:**
Demostrar en vivo cómo se ve esto en el HTML interactivo (index.html). Los asistentes pueden hacer clic en las opciones.

---

## SLIDE 10 — Caso de uso: IDEOFACTO

**Número de sección:** 03 · CASO PRÁCTICO

**Título:** Caso de uso: Chatbot de soporte para IDEOFACTO

**Texto:**
Vamos a mapear cómo construiríamos un chatbot real — desde el FAQ hasta el widget embebido.

---

## SLIDE 11 — El archivo FAQ

**Título:** 📄 Todo empieza con tu base de conocimiento

**Texto:**
El chatbot necesita un documento con toda la información que debe saber:

- ¿Qué es tu producto/servicio?
- ¿Cuáles son las fases o planes?
- ¿Cuánto cuesta?
- ¿Para quién es y para quién no?
- Preguntas frecuentes reales
- Herramientas que se usan

**Formato:** Markdown, PDF, o texto plano. Estructura de pregunta → respuesta funciona mejor.

**Notas del presentador:**
Mostrar el archivo ideofacto-faq.md como ejemplo real. Explicar que este mismo archivo se sube a Chatbase o al Custom GPT.

---

## SLIDE 12 — Flujo del chatbot

**Título:** Flujo del chatbot IDEOFACTO

**Diagrama vertical (4 cajas con flechas):**

🤖 **Mensaje de bienvenida**
"¡Hola! Soy el asistente de IDEOFACTO. ¿En qué puedo ayudarte?"
↓
🌳 **Opciones predefinidas (árbol)**
📋 Fases y precios · 🎴 Kit de tarjetas · 🎯 ¿Es para mí? · ❓ Otra pregunta
↓ el usuario elige o escribe libremente
🔀 **Router inteligente**
Si eligió opción → respuesta predefinida · Si escribió → búsqueda RAG
↓
✅ **Respuesta + siguiente acción**
Responde + ofrece botón: "¿Te gustaría empezar?" → link a Stripe/WhatsApp

---

## SLIDE 13 — System Instructions

**Título:** System Instructions (idénticas para Custom GPT y Chatbase)

**Contenido (puede ir en fuente monospace más pequeña):**

```
Eres el asistente virtual de IDEOFACTO, un sistema de facilitación
que enseña a emprendedores a crear su propio contenido con IA.

IDEOFACTO NO es una agencia. No producimos contenido para el cliente.

PERSONALIDAD
• Tono: profesional, cálido, directo
• Idioma: español latinoamericano
• Respuestas concisas con bullet points

REGLAS
1. Responde SOLO con información del FAQ
2. Si no sabes: "No tengo esa información, contacta a Mónica"
3. Precios siempre en MXN y USD
4. Al final de respuestas sobre fases: "¿Empezar con el Kit?"
5. NUNCA inventes información
6. Soporte técnico → redirige a WhatsApp
7. Respeta pre-requisitos: Kit → F1 → F2 → F3
8. Si no es cliente ideal, sé honesto
```

**Callout:**
💡 System instructions + archivo FAQ = chatbot listo

---

## SLIDE 14 — Plataformas disponibles

**Número de sección:** 04 · OPCIONES

**Título:** Plataformas disponibles

**Layout:** 3 columnas (fila 1) + 3 columnas (fila 2)

**Fila 1:**

| 🤖 Custom GPTs | 💬 Chatbase ★ RECOMENDADO | 🔧 Botpress |
|---|---|---|
| Incluido en ChatGPT Plus | $32/mes (anual) · $40/mes | $0 base + AI Spend |
| El más fácil. Subes archivos y ya. Pero vive dentro de ChatGPT. | Mejor relación facilidad/funcionalidad. Free tier disponible. | Editor visual de flujos. Pago por uso. Pro desde $89/mes. |
| ✓ Setup 10 min | ✓ Embebible con snippet | ✓ Editor visual |
| ✓ Soporta PDFs/URLs | ✓ Branding personalizable | ✓ Árboles built-in |
| ✓ Cero código | ✓ Analytics incluidas | ✓ Multicanal |
| ⚠ No embebible en web | ✓ Suggested messages | ✓ WhatsApp, Web |

**Fila 2:**

| ⚡ Dante AI | 🎙️ Voiceflow | 🌊 Flowise |
|---|---|---|
| Free tier · desde ~$24/mes | Free tier · Pro desde $60/mes | 100% gratis (self-hosted) |
| Widget personalizable, multi-idioma | Visual builder tipo diagrama | Open source. Tú lo hosteas. |

---

## SLIDE 15 — Comparación directa

**Número de sección:** 05 · COMPARAR

**Título:** Comparación directa

| | Custom GPTs | Chatbase ★ | Botpress |
|---|---|---|---|
| **Dificultad** | ⭐ Fácil | ⭐⭐ Fácil | ⭐⭐⭐ Media |
| **Embebible** | ✗ No | ✓ Sí | ✓ Sí |
| **Árbol decisión** | ✗ No | ⚠ Básico | ✓ Completo |
| **RAG / Docs** | ✓ Sí | ✓ Sí | ✓ Sí |
| **Branding** | ✗ ChatGPT | ✓ Total | ✓ Total |
| **Costo** | $0 (con Plus) | $32-400/mo | $0 + AI Spend |
| **Setup** | 10 min | 30 min | 1-2 hrs |

---

## SLIDE 16 — Cómo se inserta en tu web

**Número de sección:** 06 · INSERTAR

**Título:** ¿Cómo se inserta en tu web?

**Texto:** Es literalmente copiar y pegar un fragmento de código.

---

## SLIDE 17 — Código de embed

**Título:** Dos formas de insertar

**Columna izquierda — Script Tag (burbuja flotante)**

```html
<!-- Antes de </body> -->
<script>
  window.chatbaseConfig = {
    chatbotId: "tu-id",
    domain: "www.chatbase.co"
  }
</script>
<script
  src="https://chatbase.co/embed.min.js"
  defer
></script>
```

**Columna derecha — iFrame (chat fijo)**

```html
<iframe
  src="https://chatbase.co/chatbot-iframe/tu-id"
  width="100%"
  height="600"
  style="border: none; border-radius: 12px;"
></iframe>
```

**Nota:**
Script tag → burbuja flotante (esquina inferior derecha)
iFrame → chat fijo dentro de tu página, en un espacio definido

---

## SLIDE 18 — Dónde pegar según plataforma

**Título:** ¿Dónde pego el código?

| Plataforma | Ubicación |
|---|---|
| **WordPress** | Apariencia → Editor de temas → footer.php, antes de `</body>`. O usa el plugin "Insert Headers and Footers" |
| **Wix** | Configuración → Código personalizado → Agregar código → Body-end, todas las páginas |
| **Squarespace** | Configuración → Avanzado → Inyección de código → campo Footer (Planes Business+) |
| **Shopify** | Tienda Online → Temas → Editar código → theme.liquid, antes de `</body>` |

---

## SLIDE 19 — Ejercicio práctico

**Número de sección:** 07 · EJECUTAR

**Título:** Ejercicio: crea tu chatbot en 30 minutos

---

## SLIDE 20 — Pasos 1-4

**Título:** Pasos del ejercicio (parte 1)

| # | Paso | Detalle |
|---|---|---|
| 1 | 📄 **Prepara tu contenido** | Reúne FAQs, servicios, precios, horarios. Formato pregunta → respuesta funciona mejor. |
| 2 | 🔑 **Crea tu cuenta** | Ve a chatbase.co. Trial gratuito disponible para probar. |
| 3 | ⬆️ **Sube tu base de conocimiento** | Crea chatbot, sube tu FAQ. También puedes pegar una URL. |
| 4 | ✍️ **Configura system instructions** | Escribe las instrucciones de personalidad: tono, idioma, reglas, qué hacer si no sabe algo. |

---

## SLIDE 21 — Pasos 5-8

**Título:** Pasos del ejercicio (parte 2)

| # | Paso | Detalle |
|---|---|---|
| 5 | 🌳 **Configura opciones predefinidas** | Agrega "suggested messages" como botones al inicio — tu árbol simplificado. |
| 6 | 🎨 **Personaliza apariencia** | Colores, nombre del bot, avatar, mensaje de bienvenida. |
| 7 | 🧪 **Prueba y ajusta** | Haz preguntas reales Y preguntas que NO estén en tu contenido. |
| 8 | 🚀 **¡Inserta en tu web!** | Copia el snippet y pégalo en tu sitio. Listo. |

---

## SLIDE 22 — ¿Cuál elijo?

**Número de sección:** 08 · DECIDIR

**Título:** ¿Cuál elijo?

**Layout:** 4 cards / cuadrantes

| 🏃 "Quiero probar rápido" | 🎯 "Chatbot en mi web YA" |
|---|---|
| No necesito embed aún | No soy técnico, tengo presupuesto |
| **→ Custom GPT** · 10 min | **→ Chatbase / Dante AI** · 30 min |

| ⚡ "Potencia sin gastar" | 🔧 "Control total" |
|---|---|
| Tengo tiempo para aprender | Soy técnico o tengo dev |
| **→ Botpress** · Gratis, visual | **→ Flowise / Custom** · Self-hosted |

---

## SLIDE 23 — Cierre

**Título:** Recuerda

**Texto central:**
Todas usan la misma tecnología de fondo (RAG + LLM).

La diferencia es quién hace el trabajo técnico: tú, o la plataforma.

**Empieza simple, escala cuando lo necesites.**

---

## SLIDE 24 — Footer / Cierre

**Logo:** LifeStrategics

**Tagline:**
UNDERSTAND · DECIDE · TAKE ACTION

**Créditos:**
LifeStrategics 2026 | Taller por Mónica De Salazar

**Links útiles:**
- chatbase.co
- botpress.com
- chatgpt.com/gpts
- links.lifestrategics.com

---

## NOTAS PARA EL DISEÑO EN GOOGLE SLIDES

**Colores recomendados (LifeStrategics Design System):**
- Fondo: #181818
- Superficie: #202020
- Texto: #f0ece4
- Azul (Comprender): #4A9EFF
- Amarillo (Decidir): #FFD84A
- Rojo (Ejecutar): #FF4A4A
- Verde (Validar): #3db87a
- Muted: #999999

**Tipografía:**
- Font: Wix Madefor Display (disponible en Google Fonts)
- Títulos: 800 weight
- Subtítulos: 700
- Body: 400

**Estilo general:**
- Dark mode (fondo oscuro #181818)
- Bordes sutiles (#2e2e2e)
- Color semántico: azul = entender, amarillo = decidir, rojo = ejecutar, verde = validar
- Cards con border-top de color semántico
