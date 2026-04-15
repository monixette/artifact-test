# Cuestionario de Discovery para Chatbot
## 11 preguntas · 4 bloques · Ninguna es opcional

> Usar ANTES de configurar el bot.
> Las respuestas alimentan directamente el system prompt, el FAQ, y los límites del chatbot.

---

## Bloque 1 — Negocio

| # | Pregunta | Tipo | Para qué sirve |
|---|---|---|---|
| 1 | ¿Qué vende, a quién y cuál es su promesa? | Base | Define la identidad del bot (sección IDENTIDAD del system prompt) |
| 2 | ¿Cuál es el momento donde más duele cuando el servicio falla? | Crítica | Identifica el caso de uso prioritario — el bot debe cubrir este punto primero |

## Bloque 2 — Canales y volumen

| # | Pregunta | Tipo | Para qué sirve |
|---|---|---|---|
| 3 | ¿Por qué canal contacta el cliente hoy — y cuál prefiere la empresa? | No asumir | Define dónde se despliega: web, WhatsApp, Instagram, email |
| 4 | ¿Cuántas conversaciones maneja al día — y cuántas son la misma pregunta? | Define el nivel | Si 70%+ son repetidas → alto ROI de automatización. Define complejidad necesaria |
| 5 | ¿Cuándo se satura el equipo de atención? | ROI visible | Justifica la inversión. Horarios pico = horarios donde el bot debe estar activo |

## Bloque 3 — FAQs y límites

| # | Pregunta | Tipo | Para qué sirve |
|---|---|---|---|
| 6 | ¿Cuáles son las 5 preguntas que el equipo responde todos los días sin pensar? | Núcleo del árbol | Estas se convierten en las opciones predefinidas (Suggested Messages) y el FAQ base |
| 7 | ¿Qué consultas siempre terminan escalando a un humano — y por qué? | Define límites | Establece la regla de handoff: "Si preguntan X → redirigir a humano" |
| 8 | ¿Qué información NO puede dar el bot bajo ninguna circunstancia? | Riesgo legal | Va directo a la sección NUNCA del system prompt. No negociable |

## Bloque 4 — Proyecto y aprobación

| # | Pregunta | Tipo | Para qué sirve |
|---|---|---|---|
| 9 | ¿Qué sistema usa la empresa para gestionar clientes? | Arquitectura | Define integraciones: CRM, WhatsApp Business, Shopify, etc. |
| 10 | ¿Quién aprueba el bot antes de salir a producción? | Proceso | Identifica stakeholder. El bot se prueba con esta persona antes de publicar |
| 11 | ¿Cuál es la métrica que convence a quien toma la decisión? | Estratégica | Define el KPI del proyecto: ¿reducir tickets? ¿aumentar conversiones? ¿tiempo de respuesta? |

---

## Mapeo: Respuestas → Componentes del Chatbot

| Respuesta de... | Alimenta... |
|---|---|
| Pregunta 1 | → Sección IDENTIDAD del system prompt |
| Pregunta 2 | → Prioridad #1 del árbol de decisión |
| Pregunta 3 | → Plataforma de deploy (Chatbase web, WhatsApp, etc.) |
| Pregunta 4 | → Nivel de complejidad (simple FAQ vs. flujos avanzados) |
| Pregunta 5 | → Caso de ROI para justificar inversión |
| Pregunta 6 | → Suggested Messages + FAQ base |
| Pregunta 7 | → Reglas de escalación (handoff a humano) |
| Pregunta 8 | → Sección NUNCA del system prompt |
| Pregunta 9 | → Requisitos técnicos de integración |
| Pregunta 10 | → Checklist de aprobación pre-launch |
| Pregunta 11 | → KPI de éxito del proyecto |
