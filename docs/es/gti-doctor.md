---
lang: es
lang_alt: gti-doctor/
---
# GTI Doctor — Asistente IA

> 🤖 **El asistente IA GTI Doctor ya está EN VIVO.** Hágale preguntas sobre instrumentación geotécnica — especificaciones de sensores, procedimientos de instalación, listas de verificación de aplicación — y responde utilizando citas fundamentadas de los 18 manuales de referencia de esta base de conocimientos (5,032 fragmentos indexados, 12.5 MB de texto).

**Visite**: <https://gti-doctor.henry-phamduc.workers.dev/>

<style>
.chat-iframe-wrapper { width: 100%; min-height: 640px; border: 1px solid var(--md-default-fg-color--lightest); border-radius: 8px; overflow: hidden; background: #fafafa; }
.chat-iframe-wrapper iframe { width: 100%; height: 640px; border: 0; }
.gti-actions { display: flex; gap: 12px; flex-wrap: wrap; margin-bottom: 18px; }
.gti-actions a { display: inline-block; padding: 10px 18px; background: var(--md-primary-fg-color); color: var(--md-primary-bg-color); text-decoration: none; border-radius: 6px; font-weight: 500; }
.gti-actions a:hover { filter: brightness(1.1); }
</style>

<div class="gti-actions">
  <a href="https://gti-doctor.henry-phamduc.workers.dev/" target="_blank">Abrir chat completo ↗</a>
  <a href="#try-inline-chat">Probar chat integrado ↓</a>
</div>

<a id="try-inline-chat"></a>
<div class="chat-iframe-wrapper">
  <iframe src="https://gti-doctor.henry-phamduc.workers.dev/" title="Chat GTI Doctor" loading="lazy"></iframe>
</div>

## Preguntas de Ejemplo

- *¿Qué es un piezómetro de cuerda vibrante y cómo se instala en un sondeo?*
- *Deme la lista de verificación de instrumentación para estabilidad de taludes del manual de FHWA.*
- *¿Cómo funciona el retorno de la red de malla inalámbrica?*
- *¿Qué instrumento usaría para monitorear el movimiento lateral en un muro de contención excavado de 30 m de profundidad?*

## Cómo Funciona

| Componente | Tecnología |
| --- | --- |
| LLM | `@cf/meta/llama-3.1-8b-instruct-fp8` (Workers AI, nivel gratuito) |
| Incrustaciones | `@cf/baai/bge-m3` (multilingüe, 1024 dimensiones) |
| Base de datos vectorial | Cloudflare Vectorize (índice `gti-doctor-embeddings`, 5,032 vectores) |
| Entorno de ejecución del Worker | Cloudflare Workers (con enlaces de Workers AI + Vectorize) |
| Fundamentación | Tubería RAG — incrustar consulta → 8 fragmentos principales → aviso enriquecido con contexto |

El asistente está entrenado **únicamente** en esta base de conocimientos. Si una pregunta está fuera de alcance, lo indicará en lugar de inventar una respuesta.

## API

| Endpoint | Método | Propósito |
| --- | --- | --- |
| `/api/health` | GET | Latido del servicio |
| `/api/info` | GET | Configuración del Worker |
| `/api/chat` | POST | Chat RAG (transmisión vía SSE o JSON por lotes) |
| `/api/search` | POST | Búsqueda semántica pura (sin LLM, solo fragmentos top-K) |

Ejemplo:

```bash
curl -X POST https://gti-doctor.henry-phamduc.workers.dev/api/chat \
  -H "Content-Type: application/json" \
  -d '{"question":"What is a vibrating-wire piezometer?","stream":false}'
```

## Estado

| Componente | Estado |
| --- | --- |
| Ingesta del corpus (18 PDF, 5,032 fragmentos) | ✅ Completo |
| Índice Vectorize creado | ✅ `gti-doctor-embeddings` (1024-dim, coseno) |
| Worker de Cloudflare desplegado | ✅ <https://gti-doctor.henry-phamduc.workers.dev/> |
| Punto final de chat | ✅ Verificado — 200 OK, respuestas fundamentadas con citas |
| Widget de chat integrado en la intranet | ✅ iframe en vivo arriba |
